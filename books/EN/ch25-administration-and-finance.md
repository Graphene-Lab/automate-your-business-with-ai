# Chapter 25 — Administration and Finance

## In Simple Words

Administration and finance are where AI quietly saves the most hours in a small business. Not because the work is hard, but because it is repetitive. Invoices, bank lines, expense claims, monthly reports, cash forecasts — the same tasks, over and over, every single week. Repetition is exactly what software is good at, and AI adds the ability to read messy documents and spot patterns a person might miss.

Think of your back office as a room full of paper that never stops arriving. Every invoice is a small piece of paper that someone must read, type into a system, match against an order, check for errors, and file. Multiply that by hundreds or thousands of pieces a month, and you see where the days go. AI does not get tired, does not lose focus at 4 p.m., and does not mind doing the same task for the thousandth time.

This chapter covers four jobs: reading invoices and documents, matching (reconciling) records, producing reports automatically, and forecasting cash. Each is a place where a small business can save real time and make fewer mistakes.

One important idea before we start: AI in finance is a *draftsman*, not the *decision-maker*. It reads, sorts, matches, and suggests. A person still approves the money movement, signs off the report, and owns the result. Keep a human in the loop for anything that touches real cash. The method for judging whether any of this is worth the cost lives in [Chapter 16 — Goals, Costs, and Return on Investment](ch16-goals-costs-and-return-on-investment.md); this chapter shows you what to automate and how.

## A Bit of History

**1960s–1980s: the spreadsheet revolution.** The first big change in back-office work was the electronic spreadsheet. Before it, accountants kept ledgers by hand and a single change could mean hours of recalculation. Spreadsheets made calculation instant. This was the first time software took over a core finance task, and it set the pattern: automate the arithmetic, keep the human in charge of the meaning.

**1990s: OCR and document scanning.** Optical Character Recognition — software that reads printed text from a scanned image and turns it into editable text — arrived in business tools. Suddenly a paper invoice could become data instead of a stack of paper. Early OCR was slow and made mistakes, so a person still checked everything. But the door was open: paper could become digital.

**2000s: rules-based automation and RPA.** Robotic Process Automation — software "bots" that follow fixed rules to move data between systems — became popular. A bot could copy an invoice total from one screen and paste it into another. This worked on predictable tasks but broke the moment a document looked different: fast but brittle.

**2010s: machine learning reads documents.** Machine learning — software that learns patterns from many examples instead of following fixed rules — changed document reading. Instead of telling the computer exactly where to look, you showed it thousands of invoices, and it learned to find the vendor, the date, and the total on its own, even when the layout changed.

**2020s: large language models and agents.** Large language models — AI trained on huge amounts of text — can now read an invoice, understand what it says, and draft a reply to the vendor. They handle unusual formats that broke older tools. The newest step is the *agent*: AI that takes a whole task, like "process this vendor email," and carries it through several steps on its own, with a human reviewing the result. The Elanco example later in this chapter is exactly this kind of agent.

The arc: from hand-written ledgers, to instant spreadsheets, to scanned text, to rule-following bots, to AI that reads and reasons. Each step took more of the repetitive work off human hands and left humans to do the judging.

## Curiosity

### 25.5 The "human middleware" that AI replaced

For years, Elanco's procure-to-pay team — the people who handle questions and paperwork between buying goods and paying for them — worked as what the company called "human middleware." They manually answered over 30,000 queries a year, and each one took more than ten minutes. Ten minutes here, ten minutes there, multiplied by thirty thousand, is a mountain of hours spent moving information between systems by hand.

That story, with the real numbers and the two-layer AI system that replaced it, is told in full in "A Real Business Example" below. The curiosity here is the phrase itself: "human middleware." It describes a job where a person exists only to carry data from one place to another. That is the kind of job AI is best at removing — and the kind you should look for in your own back office.

## A Real Business Example

**Elanco: a two-layer AI ecosystem for procure-to-pay, cutting query time by about 99%.**

Elanco is a global animal-health company that makes medicines and treatments for pets and farm animals. Its procure-to-pay team — the group that handles everything between ordering goods and paying the vendor — had a chronic problem. The team spent its days as "human middleware," manually answering over 30,000 queries a year. Each query took more than ten minutes: someone would search the finance system, check the order, look up the vendor, and type an answer. The work was slow, repetitive, and error-prone.

According to The Hackett Group, which named this project a winner in the Purchase-to-Pay category of its 2026 Hackett Innovation Awards (announced in a Business Wire release on 24 June 2026), Elanco solved it with a two-layer agent-based AI ecosystem built on ElancoGPT, the company's own secure AI platform. The two layers were:

- **Layer one — AskSAP.** Employees could ask questions in plain language and get answers pulled from the company's SAP enterprise system (the software that runs its finance and operations). Instead of opening several screens and hunting for a number, a person just asked, "What is the status of this purchase order?" and got an answer.
- **Layer two — the procure-to-pay agent.** This agent automatically scans incoming vendor emails, works out what the vendor wants (the "intent"), cross-checks the request against live data in the enterprise system, and drafts a reply. A human employee then reviews the draft before it is sent.

The result was dramatic. Query resolution time dropped to **under 10 seconds** — what The Hackett Group described as **a 99% reduction** from the previous ten-plus minutes. The company also reported that the system eliminated roughly **30% to 40%** of the manual procure-to-pay queries altogether, because many questions simply stopped being asked once employees could find answers themselves through AskSAP.

Two things are worth noticing. First, the human is still there: the agent *drafts*, the employee *reviews*. Elanco did not let AI send money or replies on its own. Second, the biggest win came from giving people a faster way to find answers, which removed the need for the query in the first place. That is a pattern you can copy: the best automation often removes the request, not just the work.

A note on the source: this is a Hackett Innovation Award case, not a Microsoft customer story. The figures above come from The Hackett Group's award announcement. Treat the percentages as the company's reported results, and remember that your own numbers will differ depending on your systems and volume.

## How to Do It

### 25.1 Invoices and documents

Reading invoices and other documents by hand is one of the biggest time sinks in a small business. AI document processing can read an invoice, pull out the key fields, and put them where they belong.

**What the AI extracts.** From a typical invoice, the software pulls the vendor name, the invoice number, the date, the line items, the tax, and the total. It reads PDFs, scanned paper, and email attachments. Modern tools handle many layouts without being told each one in advance.

**How it works in practice.** You point the tool at a folder of incoming invoices, or connect it to your email. It reads each one, extracts the fields, and either enters them into your accounting system or puts them in a queue for a person to confirm. The more invoices it sees, the better it gets at your specific vendors.

**The human check.** Do not let the tool post invoices to your books without review, at least at first. Set it to extract and flag, and have a person approve. Watch the error rate (as Chapter 22 advises). Over time, as accuracy proves itself, you can let the routine, low-value invoices post automatically and route only the unusual ones to a human.

**Where it saves most.** High volume and repetitive formats. If you process hundreds of invoices a month, the saving is large and obvious. If you process ten, the tool may not pay for itself. Match the tool to your volume.

**Watch the high-stakes fields.** The total and the tax are the two fields that must be right, because a wrong number here costs real money. Double-check these until you trust the tool; vendor name and date are lower risk if wrong.

### 25.2 Reconciliations

Reconciliation means matching two sets of records to make sure they agree. The classic example is matching your bank statement against your accounting ledger. If they match, your books are correct. If they do not, something is missing, duplicated, or wrong, and you must find it.

**Why it is painful by hand.** Matching line by line is slow and boring, and boredom causes mistakes. A person scanning hundreds of bank lines will eventually miss a duplicate payment or a missing receipt.

**How AI helps.** AI reconciliation tools match records automatically by comparing amounts, dates, and reference numbers. They link a bank line to the matching invoice, flag the ones that match cleanly, and surface only the mismatches for a human to investigate. Instead of checking everything, you check the exceptions.

**The exception model.** This is the key idea: let the software handle the 95% that matches, and bring the 5% that does not to a person. The person's job changes from "match every line" to "resolve the few that do not match." That is a smaller, more interesting job, and it is where human judgment actually adds value.

**Common mismatches to expect.** A payment that appears twice (a duplicate), a bank fee nobody recorded, a receipt missing for a card payment, a payment made to the wrong vendor. The tool flags these; you resolve them. Over time you learn your own patterns and can add rules to catch recurring ones automatically.

**Keep an audit trail.** Whatever the tool does, make sure it records what it matched and what it flagged. When your accountant or an auditor asks how a figure was reached, you need a clear trail. Good tools produce this; ask before you buy.

### 25.3 Automatic reports

Monthly and weekly reports — profit and loss, sales by product, expenses by category — are another place where AI saves hours. Instead of a person pulling numbers into a spreadsheet every month, the report can build itself.

**Scheduled reports.** Set the report to generate on a fixed schedule (every Monday, the first of the month) and deliver it to your inbox or a shared folder. The numbers are pulled from your live systems, so the report is always current. Nobody has to remember to make it.

**Plain-language summaries.** Modern AI can read the numbers and write a short summary in plain words: "Revenue rose 8% this month, driven by product X; expenses rose 3%, mostly in shipping." This turns a table of figures into a sentence you can actually read and act on. It is like having a junior analyst write the commentary for you.

**Ask questions in plain language.** Some tools let you ask, "What were our top five customers this quarter?" and get an answer without writing a formula. This is useful for the ad-hoc questions that used to mean "I will look into it later" and then never happened.

**Do not skip the human read.** An automatic report is a starting point, not a finished decision document. Read the summary, check that the numbers make sense, and add your own judgment before you act on it or share it. AI can summarize confidently and still be wrong if the underlying data is messy. Garbage in, confident garbage out.

**Standardize the format.** Once you settle on a report layout, keep it stable. A consistent format is easier to read month over month and easier to spot when something looks off. Change the format only deliberately, not every time.

### 25.4 Cash-flow forecasts

Cash-flow forecasting means predicting how much money will be in the bank in the coming weeks and months. It is different from profit. A business can be profitable on paper and still run out of cash if payments arrive late. Cash is oxygen; profit is food. You can survive a long time without food and only minutes without oxygen.

**Why AI helps.** A good forecast needs to combine many signals: invoices you have sent but not collected, bills you owe, seasonal patterns, and how reliably your customers actually pay on time. AI can look at your history and learn, for example, that customer A usually pays two weeks late, while customer B pays early. It then weights the forecast accordingly.

**Start with the basics.** A simple forecast answers: what cash is coming in, what is going out, and what is the balance, week by week for the next 8 to 13 weeks. Build this even without AI — a spreadsheet works. AI improves it by learning payment patterns and flagging risk.

**Watch the gap.** The most important number is the lowest point in the forecast. If the forecast shows your balance dipping below a safe level in week nine, you have time now to fix it — chase invoices, delay a purchase, arrange a credit line. The whole value of forecasting is seeing the dip before it happens.

**Treat forecasts as ranges, not promises, and update often.** A forecast is an estimate, not a guarantee. Present it as a likely range with a best case and a worst case, and plan so that the worst case is survivable. Cash forecasts go stale fast, so update weekly; a forecast from a month ago is almost useless because so much has changed. The habit of a weekly cash check is one of the most valuable routines a small business owner can build.

## Ethics and Responsibility

Finance is where mistakes cost real money and real trust, so responsibility matters more here than almost anywhere.

**Keep a human in the loop for money movement.** AI should draft, extract, match, and suggest. A person should approve anything that sends money, changes a balance, or signs a report. An agent that reads a vendor email and pays without review is a fraud risk: a fake invoice, a spoofed email, or a misread total can drain cash fast. Elanco's agent drafts and a human reviews — copy that pattern exactly.

**Protect financial data.** Invoices and bank records are sensitive. Use tools that keep your data secure and, where possible, within your own environment. Be careful sending financial documents to public AI services. The security basics are covered in [Chapter 6 — Cybersecurity in the AI Era](ch06-cybersecurity-in-the-ai-era.md) and the self-hosting option in [Chapter 8 — Self-Hosting: Keep Your Data Under Control](ch08-self-hosting-keep-your-data-under-control.md).

**Be honest in reports.** An automatic summary can make a bad month sound fine. Do not let the polish of an AI-written report hide a real problem. Read the numbers yourself and report the truth, especially when it is uncomfortable.

**Mind the audit trail and keep segregation of duties.** Keep records of what the AI extracted, matched, and changed; if an auditor asks how a figure was produced, you must be able to show the path. And remember automation can hide a bad transaction as easily as find one: the person who sets up a vendor should not be the same person who approves its payment. AI does not remove the need for internal controls; it changes what they look like.

## Mistakes to Avoid

**Letting AI move money without review.** The single most dangerous mistake. Always require human approval for payments.

**Automating a bad process.** If your current invoice process is a mess, automating it just makes a faster mess. Clean the process first, then automate.

**Trusting extraction blindly.** AI can misread a total or a tax figure. Check the high-stakes fields until you have proof of accuracy.

**No exception handling.** If you only automate the easy cases and have no plan for the unusual ones, the unusual ones pile up and break the system. Design for the exceptions from day one.

**Skipping the audit trail.** A tool that cannot show what it did is a liability in an audit. Demand traceability.

**Forecasting the best case and betting on it.** A forecast is a range. Plan so the worst case is survivable.

**Stale forecasts and profit-vs-cash confusion.** A cash forecast from a month ago is useless; update weekly. And remember you can be profitable and still run out of money — forecast cash, not just profit.

**Over-automating low volume.** If you only have ten invoices a month, a tool may not pay off. Match the tool to your volume.

**Sending sensitive data to public AI.** Invoices and bank lines are sensitive. Use secure or self-hosted tools.

**No baseline.** Not measuring how long the task took before, so you cannot prove the saving. Measure before you start (see Chapter 22).

**Hiding bad numbers.** A polished AI report that masks a bad month is dishonest. Report the truth.

## Practical Exercise

### 25.7 Exercise: map your back-office automation

Pick one back-office task and plan its automation end to end.

**Step 1 — Choose the task.** Pick the most repetitive finance or admin task you have: invoice entry, bank reconciliation, the monthly report, or the cash forecast.

**Step 2 — Measure the baseline.** How long does it take now, and how many times a month do you do it? Write both down. This is your "before" number.

**Step 3 — Draw the current steps.** List every step a human does today: receive, read, type, match, check, file. Seeing the steps makes the automation obvious.

**Step 4 — Mark each step.** For each step, mark it: **AI does it** (extract, match, summarize), **human reviews it** (approve, sign off), or **human decides it** (the judgment call). Every money movement must be human-approved.

**Step 5 — Pick the tool.** Choose a tool that fits your volume and your accounting system. Do not buy the biggest one; buy the one that fits.

**Step 6 — Start with extract-and-flag.** Launch with the AI extracting and flagging, and a human approving everything. Do not go fully automatic on day one.

**Step 7 — Set the error threshold.** Decide the error rate that triggers action. For example, "if more than 3% of extracted totals are wrong, we stop and review the tool."

**Step 8 — Plan the cash forecast.** Build a simple 8-to-13-week cash forecast, even in a spreadsheet. Mark the lowest point. Decide what you will do if it dips below your safe level.

Do this for one task first. Once it works and the numbers prove the saving, move to the next task. One well-automated task teaches you more than five half-finished ones.

## Checklist

### 25.8 Administration and finance checklist

Before automating any finance task, check these.

- [ ] **You measured the baseline** — time per task and how often you do it.
- [ ] **A human approves every money movement** — no AI sends money on its own.
- [ ] **You clean the process before automating it.**
- [ ] **You check the high-stakes fields** (totals, tax) until you trust the tool.
- [ ] **You designed for exceptions** — the unusual cases have a clear path to a human.
- [ ] **The tool keeps an audit trail** you can show an accountant or auditor.
- [ ] **Financial data is kept secure**, not sent to public AI services.
- [ ] **Reports are read by a human** before you act on or share them.
- [ ] **You report bad numbers honestly**, not just the polished summary.
- [ ] **You keep segregation of duties** — vendor setup and payment approval are separate people.
- [ ] **You forecast cash, not just profit**, and watch the lowest point.
- [ ] **You update the cash forecast weekly.**
- [ ] **You treat forecasts as a range**, and plan so the worst case is survivable.
- [ ] **You match the tool to your volume** — no over-automation of tiny tasks.
- [ ] **You set an error threshold** that triggers a review.
- [ ] **You keep the money decision separate from the people decision** (see Chapter 16).

If a box is empty, the risk is still yours. Fill it before you let AI near the money.

## Key Takeaways

- Administration and finance are full of repetitive work — invoices, matching, reports, forecasts — and repetition is exactly what AI is good at.
- Keep AI as the draftsman and the human as the decision-maker: let it extract, match, and suggest, but a person must approve anything that moves money.
- The Elanco case (a 2026 Hackett Innovation Award winner) cut procure-to-pay query time to under 10 seconds, about a 99% reduction, by using a two-layer agent that drafts replies for human review and removes many queries entirely.
- Forecast cash, not just profit, update it weekly, and plan so the worst-case dip is survivable.
- Clean the process before you automate it, design for the exceptions, and keep an audit trail you can show.
