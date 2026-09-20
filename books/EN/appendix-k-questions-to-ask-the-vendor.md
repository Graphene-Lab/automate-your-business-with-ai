# Appendix K — Questions to Ask the Vendor

Use this in a live call or by email. These are pointed questions, not polite ones. Each has a short note on **why it matters**, so you know what a good answer sounds like. Write the vendor's answer down. Vague answers are information too.

**Tip:** Send the questions before the meeting. A vendor who answers plainly in writing is usually a vendor who operates plainly.

## Data & privacy

- **Exactly what data do you collect from us, and what do you store?** — You cannot protect what you do not know they hold.
- **Where is our data stored — which country or region?** — Location decides which privacy laws apply and who can demand access.
- **Is our data used to train your shared model?** — If yes, your private data could shape answers other customers see. Get a clear "no" or a written opt-out.
- **Can we delete our data, and do you prove it was deleted?** — "We delete it" without proof is a promise, not a fact.
- **Who else (sub-processors) touches our data?** — Every extra company is another place a leak can start.
- **Is our data encrypted both at rest and in transit?** — "At rest" = stored; "in transit" = moving. Both must be protected.

## Security

- **Do you support multi-factor login (MFA)?** — A password alone is the weakest door. MFA closes it.
- **Can we control access per person, so not everyone sees everything?** — Least access limits the damage one stolen account can do.
- **Do you keep an audit log of who did what, and can we read it?** — Without a log, you cannot trace a problem after the fact.
- **What is your breach-notification promise — how fast do you tell us?** — You need to know before your customers find out from the news.
- **How do you handle prompt injection, where a hidden instruction fools the AI?** — Tools that read outside text can be tricked; ask how they guard against it.
- **Do you run third-party security audits, and can we see the summary?** — An outside audit is stronger proof than a self-written promise.

## Pricing

- **What is the full price, and what is not included?** — Surface hidden costs now, not on the invoice.
- **How does cost grow as we grow — per user, per task, per message?** — A cheap plan can become expensive fast if it scales badly.
- **What happens if we exceed our plan limits?** — A surprise cap or overage fee can break a budget.
- **What is the renewal price, not just the intro price?** — Intro discounts end; the renewal is your real cost.
- **Is there a cheaper tier that still meets our core need?** — Do not pay for features you will never use.

## Integration

- **What systems do you connect to out of the box?** — Built-in links save time; missing ones cost custom work.
- **Do you have an API and webhooks for custom connections?** — An API means you can wire the tool to your own stack.
- **How long does setup usually take for a business like ours?** — A realistic timeline beats a sales promise.
- **Does it work with the tools we already use (email, CRM, files)?** — A tool that fights your workflow will be abandoned.
- **Who does the setup — you or us?** — Know the work and the cost before you sign.

## Support

- **What support channels exist, and what are the hours?** — Chat, email, or phone — and when a human is actually there.
- **What are your response-time commitments, in writing?** — "We try to reply fast" is not a commitment.
- **Is there onboarding or training to get staff started?** — Poor onboarding is the top reason tools go unused.
- **What uptime do you guarantee?** — An uptime promise (for example 99.9%) tells you how reliable they aim to be.
- **Can we reach a real human when it really matters?** — Bots are fine until something breaks badly.

## Contract & exit

- **How much notice do we need to cancel, and is there a penalty?** — A heavy exit fee is a trap door welded shut.
- **Can we export all our data, in a usable format, at any time?** — If you cannot leave with your data, you do not own it.
- **Who owns our content and data — us or you?** — You must keep ownership of your own work.
- **What is the contract length for a first commitment?** — Start short. Do not lock in for years on trust.
- **If we leave, in what format do we get our data back?** — A usable format (CSV, JSON) means you can move; a locked format means you cannot.

## Compliance

- **How do you comply with GDPR?** — If you handle EU personal data, this is not optional.
- **If our use is higher-risk under the EU AI Act, what extra support do you provide?** — Higher-risk uses need records, human oversight, and transparency.
- **Do you offer a data-processing agreement (DPA)?** — The standard contract GDPR requires between you and a vendor.
- **Can you support a DPIA if our project needs one?** — A DPIA is a formal privacy review some projects must do.
- **Do you tell us when your terms, model, or data location change?** — Silent changes can break your compliance without warning.

## How to read the answers

| Answer pattern | What it means |
|---|---|
| Clear, specific, in writing | Good sign. Move forward carefully. |
| Vague or "we'll get back to us" | Weak. Push for a written answer. |
| Avoids data, security, or exit | Red flag. Walk away or escalate. |
| Over-promises, no proof | Distrust. Ask for audits or references. |

**Rule:** The vendor's answers to the hard questions tell you more than their answers to the easy ones. Judge them on the awkward ones.
