# Airtable Schema + Softr Permissions

## Tables

### Families
`Family Name` (primary) · `Package` (single select: Landing, Family) · `Founder Add-on` (checkbox) · `Status` (Lead, Discovery, Proposal, Active, Landed, Property Care, Closed) · `Move Date` (date) · `Move Type` · `Net Worth Band` (5–10m, 10–15m, 15m+) · `Fee` (currency) · `Referred By` (link → Partners) · `Lead Parent` / `PA` (link → Members) · filter flags: `has_kids`, `has_staff`, `has_pets`, `ship_car`, `buying`, `uk_home`, `freight`, `high_value`, `investments`, `property_care`, `uk_storage`

### Members
`Name` · `Family` (link) · `Role` (Parent, Child, PA, Staff, Pet) · `DOB` · `Year Group` · `Curriculum` · `Nationality` · `Email` · `Portal Role` (Parent, PA, None)

### Preferences
`Family` (link) · `Areas` (multi-select) · `Budget AED` · `Bedrooms` · `Must-haves` · `Max Commute Min` · `Lifestyle Notes` · `Ten-out-of-Ten` (long text)

### Task Templates
Imported from `data/task-templates.csv`.

### Tasks
`Task` · `Family` (link) · `Pillar` · `Owner Type` (Founder, Partner, Client, PA) · `Partner` (link) · `Due Date` (formula from Move Date + Offset Days) · `Status` (To do, In progress, Waiting on client, Done) · `Visible To` (Parent, PA, Internal) · `Depends On` (link → Tasks) · `Notes`

### Partners
`Name` · `Category` · `Licence #` · `Regulator` · `Commission %` · `Agreement Signed` (checkbox + attachment) · `Contact` · `Rating`

### Referrals (commission ledger)
`Family` · `Partner` · `Deal Type` (Sale, Rental, Freight, Insurance, School, Investment intro, Banking) · `Deal Value` · `Commission %` · `Commission Due` (formula) · `Status` (Expected, Invoiced, Paid) · `Paid Date`

### Schools
`School` · `Curriculum` · `KHDA Rating` · `Annual Fee AED` · `Area` · `Admissions Contact` · per-family applications as a linked table, `School Applications` (`Child`, `School`, `Status`, `Assessment Date`, `Offer`, `Deposit Due`)

### Properties
`Family` · `Address/Community` · `Rent or Sale` · `Price AED` · `Broker` (link → Partners) · `Viewing Date` · `Client Rating` · `Status`

### Shipments
`Family` · `Mover` (link) · `Volume` · `Quote GBP` · `Packing Date` · `Sailing Date` · `ETA Jebel Ali` · `Customs Cleared` · `Delivered` · `Tracking URL`

### Updates
`Family` · `Week Of` · `Summary` · `Visible To`

## Softr roles & visibility
| Data | Parent | PA | Admin |
|---|---|---|---|
| Dashboard, plan, tasks (Visible To includes role) | ✅ | ✅ | ✅ |
| Schools, properties, shipments | ✅ | ✅ | ✅ |
| Fees, invoices, Referrals ledger | Own fees only | ❌ | ✅ |
| Investment introductions | ✅ | ❌ | ✅ |
| Partners directory (contact only) | ✅ | ✅ | ✅ (incl. commissions) |
| Other families | ❌ | ❌ | ✅ |

Every Softr list must filter on `Family = Logged-in user's Family`. **Test this with two dummy families before launch.**

## Make.com scenarios
1. **Intake → Family:** Tally submission → create Family, Members and Preferences records.
2. **Generate plan:** for each Task Template where all conditions match the family's flags → create a Task with Due Date = Move Date + Offset Days.
3. **Weekly digest:** every Friday → email the Parent and PA a summary of Done / Next / Waiting on you.
4. **Commission chase:** a Referral marked Expected and more than 14 days past its deal date → remind the admin.
