# Appendix D — Data Inventory

You cannot protect data you cannot find. This inventory lists every important data item your business holds, where it lives, and who can reach it. Fill it before you connect any AI tool. If data is not on this list, do not feed it to AI.

## How to use it

1. Walk through your tools: email, drives, accounting, CRM, HR systems, spreadsheets.
2. Add one row per data item (a customer list, a payroll file, a contract folder).
3. Mark each item **Personal** (relates to a person) or **Sensitive** (special categories — see below).
4. Check access: who can open it today, and who *should* be able to.
5. Review before any AI project. This list tells you what is safe to use and what is not.

## Blank template

| Data item | Where stored | Owner | Personal / Sensitive? | Who can access | Backup status | Retention |
|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |

## Filled example

| Data item | Where stored | Owner | Personal / Sensitive? | Who can access | Backup status | Retention |
|---|---|---|---|---|---|---|
| Customer contact list | CRM (cloud) | Sales manager | Personal (names, emails, phones) | Sales team (edit), Finance (read) | Daily, off-site | Keep while active + 3 years |
| Payroll file | Shared drive, folder "HR" | HR lead | Sensitive (salary, ID, bank) | HR only | Weekly, off-site | 10 years (legal) |
| Supplier contracts | Paper cabinet + scanned folder | Owner | Neither (business-confidential) | Owner, Finance | Partial (scans only) | Life of contract + 6 years |

## Where to look for data

Walk through each of these. Data hides in plain sight:

- [ ] Shared email inboxes and personal mailboxes.
- [ ] Shared drives and network folders.
- [ ] Cloud tools: CRM, accounting, HR, project tools.
- [ ] Spreadsheets and attachments (often the messiest).
- [ ] Paper files, cabinets, and scanned copies.
- [ ] Backups and old exports.
- [ ] Chat tools and messaging history.
- [ ] Phones and laptops of staff.
- [ ] Third-party tools staff signed up for on their own (shadow copies).

## What counts as "Sensitive"

Under GDPR, these special categories need extra care. Mark them clearly:

- Health data
- Racial or ethnic origin
- Political opinions
- Religious or philosophical beliefs
- Trade-union membership
- Genetic and biometric data (for identification)
- Sex life or sexual orientation

Also treat as sensitive even if not "special category": bank details, ID numbers, passwords, children's data, and anything that could harm a person if leaked.

## Column guide

- **Data item** — A plain name for the thing (not the file name).
- **Where stored** — System and location: cloud tool, drive path, paper cabinet.
- **Owner** — One person accountable for it.
- **Personal / Sensitive?** — Personal, Sensitive, or Neither.
- **Who can access** — Roles or people, and whether they can read or edit.
- **Backup status** — How often it is backed up, and where. Note if there is **no** backup.
- **Retention** — How long you keep it, and why (legal rule or business need).

## Red flags to fix now

- [ ] Sensitive data with no owner.
- [ ] Sensitive data anyone in the company can open.
- [ ] Important data with no backup.
- [ ] Data kept "forever" with no reason.
- [ ] Personal data in a tool you do not control (shadow AI, personal email).
- [ ] The same data in many places with no master copy.

## Retention rules of thumb

- Keep data only as long as you need it. Longer is not safer — it is more risk.
- Check legal minimums: tax and payroll records often have fixed years. Ask your accountant.
- For customer data, keep it while the relationship is active, then a short, stated period.
- Delete or anonymize data you no longer need. Do not let it pile up.
- Write the reason for each retention period, so no one has to guess later.

## Keeping the inventory current

- Review it every 6 months, and before any new AI project.
- Add a row the day a new tool or data source appears.
- Name one owner per item; owners keep it honest.
- Treat it as a living document, not a one-time chore.

## Rule for AI projects

Before any data goes into an AI tool, check this inventory. If an item is **Sensitive**, you need a clear reason, a safe tool, and often a DPIA. When unsure, leave it out.
