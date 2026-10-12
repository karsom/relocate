# CLAUDE.md — Relocate

Context for any Claude session working in this repo. Read `docs/founder-context.md` and `docs/plan.md` before advising.

## What this is
Relocate is a premium, personalised UK → Dubai relocation service, delivered as a concierge service backed by a private client portal (built no-code).

## Founder (key facts)
- Solo founder. **Has a trusted contact in Dubai for anything**: every step of a move can come with a referral from the founder. Also knows UK contacts (e.g. a tax adviser). Plans to hire a team over time.
- UK tax resident today; spends about half the year in Dubai; holds an Emirates ID and a UAE bank account. **No UK family or home ties.** Will move to Dubai full-time, won't return to the UK, and will move the company to the UAE.
- About £2–3k of savings to start; works on this full-time but doesn't depend on it for income.
- Wants first revenue by Dec 2026 and **£100k/month by Jul 2027**.
- Wants blunt, critical, strategic advice. Don't just agree.

## Clients
- Primary: families worth **£5–15m** with school-age kids.
- Secondary: well-capitalised founders (sold as a Founder add-on).
- Users: the **parents and their PA**. The PA needs restricted views, with no access to financials or investments.

## Scope
Visas, schools, property search and property management, investment introductions, freight/cargo of belongings, banking, healthcare, vehicles, staff, pets, and coordination of the UK exit.

## Revenue
Fee (£7.5k / £15k / +£7.5k Founder add-on / £500–1.5k a month Property Care) **plus disclosed partner commissions**. Property referral splits are the biggest lever.

## Non-negotiables
- **Introduce, never advise,** on regulated areas: investments (FCA/DFSA/SCA/VARA), property sales and management (RERA-licensed partners), visas (licensed PRO), and UK tax and the Statutory Residence Test (UK tax firm).
- Never hold client money. Never store passports or bank documents in Airtable; use an encrypted vault.
- Entity: UK Ltd first. Add a UAE free-zone company once Dubai substance is real, staff are hired, or brokers require it to pay referral fees. Get tax advice first; UK central-management-and-control and controlled-foreign-company rules apply while the founder is UK resident.

## Stack
Airtable + Softr (portal; Parent, PA and Admin roles) + Tally (intake) + Make.com (automation) + Framer (site) + Tresorit or Proton Drive (documents).

## Repo map
- `docs/plan.md`: strategy, offer, revenue path, distribution
- `docs/founder-context.md`: founder facts and decisions log
- `docs/discovery-questions.md`: the 30 discovery questions plus answers so far
- `docs/client-intake.md`: Tally intake form spec
- `docs/airtable-schema.md`: data model and permissions
- `docs/compliance.md`: regulatory guardrails
- `data/task-templates.csv`: master task list (import into Airtable)
- `data/partner-categories.csv`: partner types to recruit
