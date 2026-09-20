# Appendix H — AI Risk Assessment

Before you launch an AI project, ask what could go wrong and how bad it would be. This table makes risks visible so you can reduce them, not ignore them. Fill it with your team. Do it early, and revisit it often.

## How to score

Rate each risk on two scales:

- **Likelihood** — How likely is it? **Low / Medium / High**
- **Impact** — How bad if it happens? **Low / Medium / High**

Combine them into a **Risk level**:

| | Impact Low | Impact Medium | Impact High |
|---|---|---|---|
| **Likelihood High** | Medium | High | **Critical** |
| **Likelihood Medium** | Low | Medium | High |
| **Likelihood Low** | Low | Low | Medium |

Treat **Critical** and **High** as must-fix before launch.

## Blank template

| Risk | What could go wrong | Likelihood | Impact | Risk level | Mitigation | Owner |
|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |

## Filled examples

| Risk | What could go wrong | Likelihood | Impact | Risk level | Mitigation | Owner |
|---|---|---|---|---|---|---|
| Wrong data into AI | Staff paste customer personal data into a public tool | High | High | **Critical** | Approved-tools-only list; block public tools on company devices; training | IT lead |
| Wrong output used | AI drafts an invoice with a wrong amount, sent to customer | Medium | High | High | Human review before sending; auto-check totals | Accounts clerk |
| Bias in decisions | Hiring tool favours one group because of skewed training data | Medium | High | High | Human decides; review outcomes for fairness; avoid fully automated hiring | HR lead |
| Vendor leak | Provider is breached and customer data is exposed | Low | High | Medium | Vendor checklist; encrypt data; contract breach-notice clause | IT lead |
| Over-reliance | Staff stop checking and trust AI blindly | Medium | Medium | Medium | Keep human sign-off; spot audits; training on limits | Team manager |
| Prompt injection | A document hides instructions that fool the AI | Medium | Medium | Medium | Treat outside text as untrusted; limit what AI can do with it | IT lead |
| Lock-in | Cannot leave the vendor or export data | Low | Medium | Medium | Data-export clause in contract; keep a copy | Owner |
| Cost overrun | Usage grows and the bill jumps | Medium | Medium | Medium | Set usage alerts; review plan monthly; cap per-task cost | Owner |
| Model drift | Provider changes the model and output quality drops | Medium | Medium | Medium | Spot-check output weekly; keep test cases to compare | Team manager |

## Column guide

- **Risk** — A short name for the risk.
- **What could go wrong** — The concrete scenario, not a vague worry.
- **Likelihood / Impact** — Low / Medium / High.
- **Risk level** — From the grid above.
- **Mitigation** — What you will do to lower the likelihood or the impact.
- **Owner** — The one person who makes sure the mitigation happens.

## Common AI risks to consider

Use this list to spark your own rows:

- [ ] Personal or sensitive data leaked to an outside tool.
- [ ] Incorrect output trusted without review.
- [ ] Bias or unfairness in automated decisions.
- [ ] Vendor security breach.
- [ ] Prompt injection from untrusted documents.
- [ ] Shadow AI (staff using unapproved tools).
- [ ] Over-reliance and skill loss.
- [ ] Cost overrun as usage grows.
- [ ] Lock-in to one provider.
- [ ] Non-compliance with GDPR or the EU AI Act.
- [ ] Customer trust lost after a visible mistake.
- [ ] Model changes silently and output quality drops.

## When to re-run this assessment

Revisit the table when any of these happen:

- You add a new tool, data source, or process.
- Usage grows a lot, or the tool touches more people.
- An incident or near-miss occurs.
- A law or customer requirement changes.
- A vendor changes its terms, model, or where it stores data.

## Two ways to reduce a risk

Every mitigation pulls on one of two levers:

- **Lower the likelihood** — make the bad event less likely to happen. Example: approved-tools-only list makes a data leak less likely.
- **Lower the impact** — make the damage smaller if it happens. Example: human review means a wrong invoice is caught before it reaches the customer.

A good plan often pulls both. Ask for each risk: "What makes this less likely, and what limits the harm if it still happens?"

If a risk stays **Critical** even after mitigation, do not launch. Remove the risky step or redesign the process.

## Rules

- Every Critical or High risk needs a mitigation **and** an owner before launch.
- A mitigation with no owner is not a mitigation.
- Re-run this assessment at each milestone — risks change.
- If a Critical risk cannot be reduced, do not launch. Say so.
