# Appendix P — AI Vendor Due-Diligence Scorecard

Use this to compare vendors with numbers, not gut feel. Each criterion has a **weight** (how much it matters to you). Score each vendor **1–5**. The weighted total gives one number to compare. Fill one scorecard per vendor, then place them side by side.

## How to score

- **Weight** = how important the criterion is. The weights add to 100. Change them to fit your business.
- **Score** = 1 (poor) to 5 (excellent) for how well the vendor meets it.
- **Weighted score** = weight × (score ÷ 5). This keeps the total out of 100.

> **Weighted score = Weight × (Score ÷ 5)**
> **Total = sum of all weighted scores (out of 100)**

## Blank scorecard

**Vendor:** ______________________  **Date:** ____________  **Scored by:** ____________

| Criterion | Weight | Score (1–5) | Weighted score | Notes |
|---|---|---|---|---|
| Security | 20 |  |  |  |
| Privacy & compliance | 20 |  |  |  |
| Transparency | 10 |  |  |  |
| Pricing | 15 |  |  |  |
| Support | 15 |  |  |  |
| Exit & lock-in | 15 |  |  |  |
| References & reputation | 5 |  |  |  |
| **Total** | **100** |  |  |  |

## What each criterion means

- **Security** — MFA, access control, audit logs, breach notice, protection against attacks.
- **Privacy & compliance** — GDPR fit, data not used to train shared models, data location, DPA offered.
- **Transparency** — Clear answers, honest about limits, open about sub-processors and model changes.
- **Pricing** — Clear, predictable as you grow, no hidden fees, fair renewal price.
- **Support** — Real channels, written response times, onboarding, uptime promise.
- **Exit & lock-in** — Easy cancel, data export in a usable format, short first contract, you keep ownership.
- **References & reputation** — Reviews or references from firms like yours, long enough operating to be accountable.

## Filled example

**Vendor:** InvoiceFlow AI (example)  **Date:** 2026-09-15  **Scored by:** Owner

| Criterion | Weight | Score (1–5) | Weighted score | Notes |
|---|---|---|---|---|
| Security | 20 | 4 | 16 | MFA yes, audit logs yes, breach notice 72 hrs. |
| Privacy & compliance | 20 | 3 | 12 | DPA offered, but data stored outside EU — needs review. |
| Transparency | 10 | 4 | 8 | Clear docs, honest about limits. |
| Pricing | 15 | 3 | 9 | Clear now, but renewal jumps 40%. |
| Support | 15 | 5 | 15 | 24/7 chat, 2-hr response, good onboarding. |
| Exit & lock-in | 15 | 2 | 6 | CSV export yes, but 12-month lock-in with fee. |
| References & reputation | 5 | 4 | 4 | Good reviews from similar firms. |
| **Total** | **100** |  | **70** | Good product, weak on exit and data location. |

**Reading the example:** 70/100 is a decent vendor with two real problems — data location (privacy) and a costly lock-in (exit). The owner should not sign the 12-month term as-is. Fix the exit terms and confirm the data location, or look elsewhere.

## How to read the total

| Total | Meaning |
|---|---|
| 85–100 | Strong candidate. Move to a pilot. |
| 70–84 | Good, but fix the low-scoring items first. |
| 55–69 | Weak. Ask more or look elsewhere. |
| Below 55 | Reject. Too many gaps. |

## The override rule

A high total can hide a fatal flaw. **Ignore the total and walk away if any of these score 1:**

- **Security = 1** — They cannot protect your data.
- **Privacy & compliance = 1** — They will misuse or mishandle your data.
- **Exit & lock-in = 1** — You cannot get your data back or leave.

These are not trade-offs. A great price does not fix a vendor who will not let you leave or who leaks your data.

## Comparing two vendors side by side

Put the totals and the override flags together:

| Criterion | Vendor A | Vendor B |
|---|---|---|
| Total (out of 100) | 70 | 66 |
| Any override flag (Sec/Priv/Exit = 1)? | No | Yes (Exit = 1) |
| Decision | Pilot A | Reject B — cannot exit |

Here Vendor A wins even on a small total gap, because Vendor B fails the override rule.

## Tips

- **Set the weights before you score.** Decide what matters first, so the score is not bent to fit a vendor you like.
- **Score with evidence**, not charm. Use the answers from Appendix K and the checklist in Appendix B.
- **Score every vendor the same way.** Consistency is what makes the totals comparable.
- **Re-score after the trial.** Real use often changes the numbers.
