# Chapter 31 — A Small Manufacturing Business

*This chapter is a representative composite. It is not one real company. It combines the common patterns we see in small machine shops and fabricators that adopt AI. All numbers are illustrative — they show the shape of the decision, not a promise. Replace them with your own.*

## Context

Picture a small precision machining shop. We will call it **Northgate Machining**. It employs about twenty-five people. It makes custom metal parts to order — one-off pieces and short runs for other factories. Nothing sits on a shelf waiting for a buyer. Every part starts as a customer request.

The work begins with an **RFQ**, which stands for "request for quote." A customer emails a drawing — usually a PDF with the shape of the part, its measurements, and the material it must be made from. The shop must look at that drawing, figure out how long each cutting and finishing step will take, add up the cost of the metal and the machine time, and return a price. That price is the quote. If it is too high, the customer goes elsewhere. If it is too low, the shop wins the job but loses money making it.

Two experienced estimators do most of this quoting. They have been doing it for years. They can look at a drawing and roughly know what it costs. But "roughly" is doing a lot of work in that sentence. The shop has no written record of what past quotes actually cost to produce. The knowledge lives in two heads. When those two people are on holiday, quoting slows to a crawl.

Behind the quoting sits the rest of the shop. Raw metal stock — bars, plates, rods — is tracked in a spreadsheet that is updated when someone remembers. Quality control is a final visual check by hand at the end of the job. Weekly reports for the owner are typed by hand from three different spreadsheets. Nothing is connected. Everything depends on people remembering to write things down.

This is a normal, healthy small manufacturer. It is profitable. It is busy. And it is leaving money on the table in four places: quoting, inventory, quality, and reporting.

## The Problem

The owner, Elena, can feel the problems but cannot always see them. Let us name them plainly.

**Quoting is slow and inconsistent.** A simple part takes an hour to quote. A complex one takes half a day. The average is two days from the email arriving to the quote going out. In that window, the customer has already asked two other shops. Speed matters. Worse, the two estimators price the same drawing differently. One is cautious and prices high. The other is aggressive and prices low. Over a year, some jobs are quietly underpriced. The shop wins them, builds them, and discovers later that the machine time cost more than the price covered. These losses are invisible because nobody compares the quote to the actual cost afterward.

**Inventory is guesswork.** The shop buys metal stock when someone notices the shelf is low. Too often, that is too late — a job is delayed because the right bar is not in stock. Just as often, the shop buys too much, and expensive material sits for months, tying up cash. The spreadsheet is never quite right. Nobody trusts it, so people double-check by walking to the shelf, which wastes time.

**Quality defects are caught too late.** A bad part is often found only at the final check, after the whole job is finished. If the error was made on the first cut, the shop may have made fifty bad parts before noticing. That is scrap — material and machine time thrown away. Catching a defect after fifty parts instead of after one is fifty times the loss.

**Reporting eats hours.** Every Friday, someone spends three or four hours pulling numbers from the spreadsheets to build a summary for Elena. That time is pure overhead — it produces no parts and wins no customers.

Each of these is a small leak. Together, they drain real money and real time. If you want to see how these four activities rank against the rest of your business, the impact-and-effort method in [Chapter 12 — Where AI Can Help Your Business](ch12-where-ai-can-help-your-business.md) is the place to score them.

## The Solution

Elena does not try to "use AI everywhere." She picks the four leaks and attacks them one at a time, starting with the biggest and easiest.

**Smarter quoting.** Instead of reading each drawing from scratch, the shop feeds its past jobs into a system. For every past job, it now records two things it never linked before: the original quote and the actual cost to produce. Over time this becomes a reference library. When a new drawing arrives, an AI assistant reads the PDF, pulls out the key features — the dimensions, the tolerances (how exact each measurement must be), the material, the number of pieces — and suggests a price based on similar past jobs. The estimator no longer starts from a blank page. They start from a draft and adjust it. The AI does the first pass; the human makes the call.

**Inventory that predicts.** The shop connects its stock spreadsheet to a simple forecasting tool. The tool looks at how fast each material is used and suggests when to reorder and how much. It does not place the order itself. It raises a suggestion: "You will run out of this aluminium bar in nine days; order now." A person confirms it. The guesswork becomes a prompt.

**Quality checks at the machine.** Instead of checking only at the end, the shop puts a small camera at one machine. A computer-vision system — AI that reads what a camera sees — looks at each part as it comes off and flags anything that looks wrong: a crack, a wrong dimension, a missing hole. The operator sees the flag immediately and stops before making fifty bad copies. The final human check stays; the camera just moves the warning earlier. (The deeper treatment of vision-based quality control and predictive maintenance is in [Chapter 29 — Operations and Production](ch29-operations-and-production.md).)

**Reports that write themselves.** The spreadsheets are connected to a reporting assistant. On Friday, instead of typing, Elena receives a drafted summary: jobs quoted, jobs won, scrap rate, stock levels, cash tied up. She reads it and edits. Three hours become fifteen minutes.

Notice the pattern across all four. The AI never acts alone. It reads, suggests, flags, and drafts. A human decides, confirms, and approves. This is the same "human reviews the machine's draft" pattern that the Elanco case shows in [Chapter 25 — Administration and Finance](ch25-administration-and-finance.md). In a shop where a wrong number can lose real money, that rule is not optional.

## The Tools

None of this required a team of engineers. The tools are off-the-shelf, aimed at small businesses.

- **A document-reading assistant** that opens the drawing PDF and extracts dimensions and features into a structured form. This is the same class of tool that reads invoices in [Chapter 25](ch25-administration-and-finance.md).
- **A quoting assistant** built on top of that, which compares the extracted features to past jobs and proposes a price. This can be a low-code tool bolted onto the shop's existing quoting spreadsheet, connected as described in [Chapter 19 — Connecting AI to Systems You Already Use](ch19-connecting-ai-to-systems-you-already-use.md).
- **A forecasting add-on** for the inventory spreadsheet or the shop's basic ERP (enterprise resource planning) system. Many inventory tools now include a "suggest a reorder" feature.
- **A camera plus a computer-vision inspection tool** at one machine. These are sold as small, self-contained units for quality checks.
- **A reporting assistant** that reads the connected spreadsheets and drafts the weekly summary in plain language.

How to choose among these without being fooled by glossy demos is covered in [Chapter 17 — Choosing Tools Without Being Fooled](ch17-choosing-tools-without-being-fooled.md). One caution specific to a machine shop: **drawings are confidential.** A customer's part drawing is their intellectual property. Before you feed drawings into any cloud tool, check where the data goes and who can see it. For some shops, keeping the AI on their own computers — self-hosting, explained in [Chapter 8 — Self-Hosting: Keep Your Data Under Control](ch08-self-hosting-keep-your-data-under-control.md) — is the safer choice. The risks of sending sensitive files to third-party services are in [Chapter 9 — Third-Party Services and Shadow AI](ch09-third-party-services-and-shadow-ai.md).

## The Costs

Here is an illustrative first-year budget for a shop like Northgate. These are made-up numbers to show the shape. Use your own.

**Direct costs.**
- Quoting and document assistant: about €9,000 a year in subscriptions.
- Forecasting add-on: about €3,000 a year.
- Camera and vision inspection unit: about €6,000 one-time, plus €1,200 a year.
- Reporting assistant: about €2,400 a year.
- Setup and integration (external help to connect the tools to the spreadsheets and the machine): about €10,000 one-time.
- Training the estimators and operators: about €3,000 one-time.

First-year total: roughly **€34,600**. In steady years after, the one-time costs drop away and the recurring subscriptions come to about **€15,600**.

**Indirect costs.** These are the ones people forget.
- The estimators spend hours learning the tool and checking its drafts. That is real time, valued at their loaded hourly cost.
- The learning dip: for the first few weeks, quoting is slower, not faster, while people trust the new system.
- The vision camera needs occasional recalibration when lighting or the part changes.
- Someone must review the AI's suggested quotes and reorder points every day. Never skip this.

The full method for counting these costs honestly, and for turning the savings into a return figure, lives in [Chapter 16 — Goals, Costs, and Return on Investment](ch16-goals-costs-and-return-on-investment.md). Do not run the math in your head. Write it down.

## The Results

After a year, measured against the baseline Elena recorded before starting, the illustrative outcome looks like this. Remember: your numbers will differ. These show what a good fit can look like, not what yours will be.

- **Quoting time** fell from an average of two days to a few hours for most parts. The estimator reviews a draft instead of building from zero.
- **Fewer underpriced jobs.** Because the quote is anchored to what similar jobs actually cost, the gap between quoted price and real cost narrowed. The shop stopped quietly losing money on jobs it won.
- **Win rate improved.** Faster quotes meant Northgate answered more RFQs inside the window where the customer is still choosing.
- **Scrap dropped.** Catching a defect at the machine instead of at the end cut wasted material and machine time. Instead of fifty bad parts, the operator caught it at the first or second.
- **Stock turns improved.** Fewer stockouts meant fewer delayed jobs. Less over-buying meant less cash frozen on the shelf.
- **Reports** went from three or four hours of typing to about fifteen minutes of reading and editing.

The honest caveat: none of this happened on day one. The quoting assistant was rough for the first month because the library of past jobs was thin. The vision camera gave false alarms until it was calibrated. The savings ramped up over weeks, exactly as the learning-curve warning in [Chapter 16](ch16-goals-costs-and-return-on-investment.md) predicts. Elena measured the real numbers after the ramp, not during it.

## Lessons Learned

**Start with quoting.** Of the four leaks, quoting was the highest impact and the lowest risk to try. A wrong quote is caught by the estimator before it goes out. That made it the perfect first project — the same "high impact, high ease first" rule from [Chapter 12](ch12-where-ai-can-help-your-business.md).

**Your past jobs are the fuel.** The quoting assistant was only as good as the record of past quotes and their real costs. The single most valuable thing Elena did was start linking every quote to its actual production cost. Without that data, the AI had nothing to learn from. Data readiness is covered in [Chapter 14 — Data: The Raw Material](ch14-data-the-raw-material.md).

**The AI drafts; the human decides.** Not one quote went out without a person approving it. Not one reorder was placed without a person confirming it. In a shop where a wrong number is real money, the human check is the safety, not a delay.

**Drawings are confidential.** Treat every customer drawing as sensitive intellectual property. Decide where it may go before you feed it anywhere. For some shops that means self-hosting; for others it means a vetted vendor with a clear contract.

**Calibrate the camera; do not trust it blindly.** The vision system was not plug-and-play. It needed tuning to tell a real defect from a shadow. Budget for that, and keep the final human check in place.

**Expect the ramp.** The first month was slower and messier than the twelfth. Judge the project after the learning curve, not during it.

**Connect, do not replace.** Northgate did not throw away its spreadsheets or its ERP. It bolted AI onto what already worked, as described in [Chapter 19](ch19-connecting-ai-to-systems-you-already-use.md). The shop kept its systems and added a smarter layer on top.

The small manufacturer's lesson is the same as every other sector's: find the leak, pick the easiest high-value one, let AI draft and flag, keep a human on the decision, and measure honestly. A shop with twenty-five people and no engineers can do this. The tools are ready. The only thing missing is a clear look at where the money is leaking.
