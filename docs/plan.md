# Relocate — UK → Dubai Relocation for £5–15m Families & Founders — Plan v2

## Context
A solo founder with a strong network is building a premium, personalised UK → Dubai relocation service:
- **Clients:** families worth £5–15m with school-age kids, plus well-capitalised founders.
- **Users:** the parents and their PA.
- **Scope:** visas, schools, property search and property management, investment introductions, cargo/freight of belongings, plus the rest of the move.
- **Resources and targets:** £2–3k savings, full-time commitment, first revenue by Dec 2026, £100k/month by Jul 2027.
- **Model and build:** hybrid (founder-run concierge plus a private client portal), built no-code.
- **Repo:** a new private `relocate` repo. `karsom/karsom` is the profile README and stays untouched.

## Founder facts (persist in repo as `docs/founder-context.md`)
- Solo founder; UK resident and UK tax resident; spends about half the year in Dubai.
- £2–3k savings, full-time commitment, doesn't need the income to live on. First revenue by Dec 2026; target £100k/month by Jul 2027.
- Targets: families worth £5–15m with school-age kids, plus well-capitalised founders. Users are the parents and their PA.
- Scope: visas, schools, property search and management, investment introductions, freight/cargo, plus the full move. Delivered through the founder's network of partners.
- Revenue: fee plus commission. Build a team over time.
- Build: no-code MVP (Airtable + Softr + Tally + Make.com).
- Entity: UK Ltd first; UAE free-zone company later (see point 5).

## Hard truths that change the plan
1. **At £5–15m, the earlier £25k/£60k/£150k pricing is wrong.** These clients are rich but not "£150k concierge" rich, and many will compare you to a £3k relocation firm. Realistic fees run £7.5k–£30k.
2. **£100k/month from fees alone is impossible solo.** At about £15k a family, that's 7 new families a month. You can deliver 3–4 at a time, maximum.
3. **The real money is partner commissions, above all property.** Dubai agents earn 2% on a sale. On a £2–5m villa, a referral split of 25–50% is worth £10k–£50k to you. A rental placement is 5% of annual rent. Freight partners pay 10–15%, and insurance and banking intros pay small amounts. Model each family as **fee + commissions = £25k–£70k**. On that basis £100k/month needs 2–4 families a month closing a property purchase. That's hard but not delusional.
4. **Regulated activities you must NOT do yourself:**
   - **Investment opportunities:** promoting or advising is regulated by the FCA (UK), and by the DFSA/SCA/VARA (UAE). You may only *introduce* to licensed firms, under a written introducer agreement. One mis-sold deal will end the business.
   - **Property sales and management:** these need a RERA-licensed brokerage or property manager in Dubai. Partner with one and take a referral split. Don't hold client funds.
   - **Visas:** use a licensed PRO/typing-centre partner. You coordinate.
   - **UK tax exit:** refer to a UK private client tax firm. Never comment on Statutory Residence Test (SRT) days yourself.
5. **Entity (researched):** a UK resident *can* get a UAE free-zone licence remotely (from about AED 5,750, roughly £3–5k realistic with a visa), but there's **no tax benefit while you live in the UK**:
   - If you run the company from the UK, it is UK tax resident under the central management and control test.
   - UK controlled foreign company rules can apply because you own more than 25%.
   - The 0% free-zone tax rate requires substance in the UAE.

   **Decision:** start as a UK Ltd (about £50) acting as coordinator and introducer. Add a UAE free-zone entity only when (a) you move or spend real time in Dubai, (b) you hire Dubai staff, or (c) brokers or partners will only pay referral fees to a UAE-licensed company. Confirm (c) with your first 2 broker partners. Get a 1-hour UK tax adviser sign-off before you set up the UAE entity.
   **Update:** the founder spends about 6 months a year in Dubai. That helps on the ground and makes a UAE entity worth getting sooner. But it doesn't settle UK tax residence: the Statutory Residence Test depends on ties as well as days, so you can easily remain UK resident. If board-level decisions are genuinely made in Dubai, the company could be managed from the UAE. To get that, keep a decision log and hold board meetings in Dubai.
6. **Founders and families are two products.** Founders want speed, company setup, the Golden Visa, banking and investments. Families want schools and homes. Lead with **families**, which are stickier and carry the property commission. Treat founders as a "Founder add-on" (company setup and banking).

## Offer v2
| Package | Fee | Scope |
|---|---|---|
| Landing | £7.5k | Personalised move plan, visas (via PRO partner), school shortlist + applications, rental search, portal, 30-day landing support |
| Family | £15k | + full property search (rent or buy), freight/cargo end-to-end, banking + healthcare + car setup, UK exit coordination (tax partner intro), 90-day support |
| Founder add-on | +£7.5k | Free-zone company setup, corporate banking, Golden Visa route, introductions to licensed investment/wealth partners |
| Property Care | £500–1.5k/mo | Ongoing property management via a RERA partner (recurring revenue; also offered for UK homes being let) |
Partner commissions are disclosed in the engagement letter. Founding clients get 40% off in return for a testimonial and referrals.

## Revenue path (Dec 2026 → Jul 2027)
- **Dec–Jan:** 1–2 founding families (fees about £10k plus first commissions).
- **Feb–Apr:** 2–3 families a month. Property Care recurring revenue starts. Hire a freelance ops assistant (Dubai or remote, about £1.5k/month) at family #4.
- **May–Jul:** 3–4 families a month plus founder add-ons. Monthly revenue of £60–120k depends on how many property purchases close.
- **Leading indicator to track weekly:** qualified intro calls. You need about 15–20 calls a month to close 3–4 families.

## Team (later)
Commission plus fee is the revenue model. Hiring order:
1. Dubai-based ops coordinator (at family #4)
2. Business-development person on a partly commission-based package, working the referral partners
3. Second client lead, once you're at 6+ active families

Hire from your network, but pay on contract with clear commission splits written down from day 1.

## Distribution (where £5–15m families actually come from)
- UK private client tax firms and wealth managers. Offer them a reciprocal referral, since they gain from the exit work.
- UK prep schools and their parent networks, plus Dubai school admissions teams.
- Dubai prime brokerages: they want buyers, you bring them.
- Founder channels: exit-focused communities, angel networks, accountants who handle exits.
- Content: a sharp "Moving your family UK → Dubai in 2026" guide, used as the lead magnet behind a private enquiry form.

## MVP Portal (no-code, budget about £100/month)
**Stack:** Airtable (data) + Softr (portal; magic-link login; roles for Parent, PA and Admin) + Tally (intake) + Make.com (automations) + Framer (one-page site) + Tresorit or Proton Drive for passports and financial documents. Never store sensitive documents in Airtable.

**Roles:**
- **Parent:** sees everything for their family and approves decisions.
- **PA:** sees and manages tasks, documents and bookings; can be restricted from financials and investments.
- **Admin:** you.

**Airtable tables:**
- `Families`: package, budget, move date, net-worth band, source/referrer.
- `Members`: parents, children (age, school year, curriculum), staff, pets.
- `Preferences`: areas, commute-to-school limit, villa specs, lifestyle, security.
- `Pillars`: UK exit, visas, schools, property, freight/cargo, banking, healthcare, vehicles, staff, pets, company setup, investments, property care.
- `Tasks`: generated from templates; owner, due date, dependency, status, visible-to role.
- `Partners`: category, licence #, commission %, contact, rating.
- `Referrals`: which partner, which family, deal value, commission due/paid. This is your real P&L.
- `Schools`, `Properties`, `Shipments` (freight quotes, volume, sailing date, tracking), `Updates`.

**Portal pages:** Dashboard (timeline + % complete per pillar), Your Plan, Schools tracker, Property shortlist, Shipment tracker, Documents checklist, Your Team, Weekly update. Admin pages: pipeline, all-tasks board, partner and commission ledger.

**Personalisation:** a Tally intake triggers Make.com, which clones task templates filtered by family attributes (kids' ages/curriculum, pets, staff, buying vs renting, founder add-on, UK home kept, freight volume).

## Step 0 — New repo `relocate` (after approval)
Create a private GitHub repo `relocate`, add it to the session, clone it, then commit and push to `main`:
- `README.md`: positioning, offer, how the repo is organised.
- `CLAUDE.md`: founder facts and key decisions, so future Claude sessions in this repo load the context automatically.
- `docs/founder-context.md`: the founder facts above.
- `docs/plan.md`: this plan (strategy, revenue path, distribution).
- `docs/discovery-questions.md`: the 30 founder questions with answers to date.
- `docs/client-intake.md`: the parent and PA intake form spec (for Tally).
- `docs/airtable-schema.md`: tables, fields, roles and Softr permissions.
- `data/task-templates.csv`: a master task list of about 150 rows (pillar, task, owner type, offset days from move date, conditions such as `has_pets`, `buying`, `founder`). Ready to import into Airtable.
- `data/partner-categories.csv`: partner types to recruit, the licence each needs, and typical commission.
- `docs/compliance.md`: introducer-only rules, licences, professional indemnity cover, GDPR/PDPL, disclaimers.

## Verification
- `task-templates.csv` imports cleanly into Airtable (correct headers and types).
- Dry run with a mock family (2 kids aged 7 and 11, a dog, a nanny, buying a £3m villa, a 40ft container, UK house let out). The intake should produce the right filtered task set, and the PA login must not see investment or financial records.
- Business check by end of Jan 2027: at least 1 paying family and at least 5 signed partners.
