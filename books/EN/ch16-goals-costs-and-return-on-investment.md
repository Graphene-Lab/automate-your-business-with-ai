# Chapter 16 — Goals, Costs, and Return on Investment

## In Simple Words

Before you spend money on AI, you need to answer three plain questions. What do you want to achieve? What will it cost? What will you get back? If you cannot answer these, you are not making a decision — you are guessing. This chapter gives you a simple, honest way to answer them.

The central idea is called **ROI**, which stands for **Return on Investment**. In plain words, ROI measures how much value you get back for every unit of money you put in. If you spend one euro and get three euros of value, that is a good return. If you spend one euro and get fifty cents back, that is a bad one. ROI turns a fuzzy "is this worth it?" into a number you can think with.

This chapter is the **home of the ROI method** for this book. The simple formula, how to use it, and a worked example all live here. When other chapters talk about measuring results or return, they point back to this one. Learn the method here once, and you can apply it to any AI project.

A simple image to carry: ROI is like checking whether a machine in your workshop is worth buying. You ask what it costs to buy and run, and how much money or time it saves you. If it saves more than it costs, it pays for itself and then some. If not, it is an expensive ornament. AI is no different — except that its costs and benefits are sometimes hidden, so you have to look harder for both.

One honest warning up front: numbers can lie if you want them to. It is easy to inflate the savings and shrink the costs to make a bad idea look good. The method here is built to keep you honest. Use it that way, not as a way to justify a decision you already made.

## A Bit of History

**Early 1900s: ROI is born for factories.** A manager named Donaldson Brown, working at DuPont in the 1910s and 1920s, developed a way to compare how well different parts of a business used their money. He expressed it as a ratio of profit to the money invested. This let owners compare one factory against another and decide where to put the next dollar. It was a small idea with huge influence — it made "return" a number you could manage.

**Mid-1900s: payback period.** Businesses added a simpler cousin of ROI: how long until the savings cover the cost? If a machine pays for itself in two years, that felt safe. If it took fifteen, that felt risky. Payback became a quick gut-check for big purchases.

**1980s–1990s: the limits of counting money.** Managers realized that some of the most important things — customer satisfaction, quality, learning, employee morale — did not show up in a simple profit number. The "balanced scorecard," developed by Kaplan and Norton in the early 1990s, tried to capture these alongside the money. The lesson: count what matters, not only what is easy to count.

**2000s: tech projects and the productivity paradox.** Companies poured money into software and sometimes saw little return, leading to a famous joke that computers showed up everywhere in the economy's numbers except in productivity. The cause was rarely the technology. It was vague goals, hidden costs, and poor adoption. Measuring the right things became a discipline of its own.

**2020s: AI forces honest math.** AI can save real time and money, but its costs are easy to underestimate (subscriptions, setup, training, maintenance) and its benefits are easy to overstate (hyped savings, ignored learning curves). A simple, honest ROI method is now essential to separate the tools that pay off from the ones that just sound good.

The arc: from a factory ratio to a modern discipline. The tools changed; the core question never did — did you get back more than you put in?

## Curiosity

### 16.7 The company that cut query-resolution time by 99%

One of the most striking recent examples of AI's effect on a business process is the animal-health company **Elanco**, which reported cutting the time to resolve certain internal information queries by about **99%** after putting a generative-AI assistant to work — turning a search that once took many minutes into a near-instant answer.

That is the headline. The full case, with the details and the lessons behind the number, is told in [Chapter 25 — Administration and Finance](ch25-administration-and-finance.md), the canonical home of the Elanco story. The point for this chapter is one line: a huge saving in time is a real, measurable benefit — and it is exactly the kind of thing a good ROI calculation is designed to capture.

## A Real Business Example

*The following is an illustrative composite of common real-world patterns, not a single named company.*

A logistics firm wanted to "use AI," so it bought a chatbot for customer questions. Nobody set a clear goal first. Six months later, the owner asked, "Is this working?" and nobody could answer. There was no starting number to compare against, so there was no way to tell if anything improved. The tool was probably helping a little, but the firm could not prove it, could not size it, and could not decide whether to expand or stop. The money was spent, and the lesson was lost.

A second firm did the opposite. Before buying anything, it picked one clear goal: cut the time its team spent answering the same ten repeated customer questions. It measured the starting point — about 30 hours a week across the team. It set a target: half that, within three months. It counted the costs honestly, including the time to set up and train. At the end, it had a real before-and-after number and a real cost figure, and it could compute a clear return. The decision to expand was easy because the math was clear.

The difference was not the AI. It was that the second firm defined a goal and measured it before it spent a euro. That is what the rest of this chapter teaches you to do.

## How to Do It

### 16.1 Defining simple and measurable objectives

A goal you cannot measure is a wish, not a goal. "Use AI better" is a wish. "Cut invoice processing time by half by June" is a goal. The first step in any ROI calculation is to turn your intention into something you can measure.

A good objective has four parts:

- **One metric.** Pick a single number that matters — hours spent, cost per item, errors made, response time, sales closed. Not five numbers. One.
- **A baseline.** What is that number *right now*? Measure it before you start. Without a baseline, you can never prove change. If you do not know your current invoice time, go measure it this week.
- **A target.** What do you want it to become? Be specific: "half," "two minutes instead of ten," "ten fewer errors a week."
- **A time frame.** By when? "In three months" gives the goal a deadline and makes it real.

Keep it simple. A small business does not need a dashboard of fifty metrics. One clear metric per project, with a baseline and a target, is enough to drive a real decision.

Write the objective in one sentence: *"By [when], we will change [metric] from [baseline] to [target]."* If you cannot fill in those blanks, you are not ready to spend. Go back and define it. This single habit prevents most wasted AI spending.

### 16.2 Direct and indirect costs

The price tag is not the cost. Most people count the subscription and stop. The real cost is bigger, and the hidden parts are what turn a good-looking project into a money pit. Count both kinds.

**Direct costs** are the obvious ones you pay for:

- **Software and subscriptions.** The monthly or yearly fee for the AI tool.
- **Setup and integration.** The work to connect the tool to your existing systems.
- **Hardware.** Any equipment you need to buy.
- **External help.** Consultants, developers, or trainers you pay.
- **Training.** The cost of teaching people to use it.

**Indirect costs** are the hidden ones people forget:

- **Staff time to set up and run it.** Hours your own people spend configuring, testing, and managing the tool. This is real money, even if no invoice shows it.
- **The learning dip.** When you change how people work, they slow down before they speed up. A few weeks of lower productivity is normal and costs something.
- **Maintenance and updates.** Tools need tending — fixing breaks, updating settings, handling new cases.
- **Review and checking.** The human time to check AI output, which you should never skip.
- **Governance and compliance.** The effort to keep the tool within privacy and legal rules (see [Chapter 10](ch10-privacy-and-gdpr.md)).
- **Switching and exit costs.** What it costs to change tools later if this one disappoints.

A good rule: the visible price is often only half the real cost. Add up every cost you can think of, including your own people's time, and value that time at what it truly costs you (salary plus overhead, not just the take-home pay). Underestimating cost is the most common way people fool themselves.

### 16.3 Quantifiable and non-quantifiable benefits

Benefits come in two kinds. Some you can put a number on. Some you cannot, but they still matter. A good calculation handles both honestly.

**Quantifiable benefits** can be turned into money:

- **Time saved.** Hours not spent on a task, valued at the cost of that time.
- **Errors avoided.** Fewer mistakes means fewer refunds, re-dos, and penalties.
- **Faster cycles.** Quicker invoices get paid sooner; quicker quotes win more deals.
- **More sales or output.** If AI helps you serve more customers or produce more.
- **Lower labor or material costs.** Direct savings you can point to.

**Non-quantifiable benefits** are real but hard to price:

- **Employee satisfaction.** People may enjoy work more when the boring parts are automated.
- **Customer experience.** Faster, clearer service makes customers happier, even if you cannot pin a number on it today.
- **Less stress and fewer late nights.** Quality-of-life gains that do not show in a spreadsheet.
- **Better decisions.** AI can surface insights that improve judgment.
- **Reputation and readiness.** Being a business that uses modern tools well.

How to handle both: **monetize what you honestly can, and write down the rest separately.** Do not force a fake number onto something intangible. Do not pretend the intangible is worth zero either. List it, name it, and weigh it in your judgment alongside the hard numbers. A project with modest money savings but big gains in staff morale and customer happiness may still be worth doing. The point is to see the whole picture, not a false single number.

### 16.4 A simple calculation of ROI

Now the method itself. The core formula is simple.

**ROI = (Net Benefit ÷ Total Cost) × 100%**

Where **Net Benefit = Total Benefit − Total Cost**.

A positive ROI means you gained more than you spent. A negative ROI means you lost money. The higher the percentage, the better the return.

**A tiny worked example.** Suppose an AI tool costs **€10,000** in total for the first year (subscription plus setup plus training). You measure that it saves your team **€25,000** worth of time and errors over that year.

- Net Benefit = €25,000 − €10,000 = **€15,000**
- ROI = (€15,000 ÷ €10,000) × 100% = **150%**

A 150% return means for every euro you spent, you got your euro back plus €1.50 extra. That is a strong return.

**Payback period** is the companion number: how long until the savings cover the cost? If you save €25,000 a year, that is about €2,083 a month. To cover a €10,000 cost takes about **4.8 months**. After that, the savings are pure gain.

How to read the result:

- **ROI clearly positive and payback short** (a few months) — a strong case to proceed.
- **ROI positive but payback long** (several years) — think carefully; the margin is thin and risks could erase it.
- **ROI near zero or negative** — the tool does not pay for itself on the numbers you have. Either find more benefit, cut cost, or walk away.

Two honest habits make this method trustworthy. First, use your real baseline and your full cost, not optimistic guesses. Second, run the calculation over a clear period (usually one year) and repeat it after launch with actual numbers, not projections. The first calculation is an estimate to decide; the second is the truth to learn from.

### 16.5 Example: automating invoices

Here is the full method applied to a common case — automating invoice processing. *All numbers are illustrative; replace them with your own.*

**The setup.** A small firm handles **2,000 invoices a month** (24,000 a year). Right now, staff do them by hand.

**Step 1 — Baseline.** Each invoice takes about **10 minutes** by hand. That is 240,000 minutes a year = **4,000 hours a year**. At a fully-loaded staff cost of **€25 per hour**, the manual work costs about **€100,000 a year**.

**Step 2 — What the AI changes.** The tool fully automates about **80%** of invoices, cutting each of those from 10 minutes to about 2 minutes of human review. So it saves 8 minutes on 19,200 invoices (80% of 24,000). That is 153,600 minutes = **2,560 hours a year saved**. At €25/hour, the **gross benefit is about €64,000 a year**.

**Step 3 — Total cost.** Software subscription **€12,000/year**, one-time setup **€8,000**, training **€2,000**. First-year total cost = **€22,000**. In steady years after, cost drops to about **€14,000** (subscription plus maintenance).

**Step 4 — ROI, first year.**
- Net Benefit = €64,000 − €22,000 = **€42,000**
- ROI = (€42,000 ÷ €22,000) × 100% ≈ **191%**

**Step 5 — Payback.** Monthly savings ≈ €64,000 ÷ 12 ≈ €5,333. To cover the €22,000 first-year cost takes about **4 months**.

**Step 6 — Steady state (year two).**
- Net Benefit = €64,000 − €14,000 = **€50,000**
- ROI = (€50,000 ÷ €14,000) × 100% ≈ **357%**

**Reading it.** The first year returns about 191% and pays for itself in roughly four months. After that, the return climbs because the one-time costs are gone. This is a clear, strong case — and you can see exactly why, because every number came from a measured baseline and a full cost list. Now imagine doing this with *your* invoice count, *your* time per invoice, and *your* costs. That is the calculation that decides your real choice.

## Ethics and Responsibility

ROI is a tool for honest decisions, and it can be misused.

**Do not inflate savings to justify layoffs.** The easiest way to make a bad project look good is to overstate the savings and then cut people. Use honest numbers, and decide about people separately and humanely (see [Chapter 15](ch15-people-roles-and-culture.md)).

**Count the human cost.** The learning dip, the stress of change, the time people spend adapting — these are real costs. Leave them in the math. A clean number that hides a messy reality is a dishonest number.

**Do not game the baseline.** If you make the starting point look worse than it was, the improvement looks bigger than it is. Measure the baseline honestly, before you have a stake in the result.

**Value the non-quantifiable.** Do not treat staff morale, customer happiness, and reduced stress as zero just because they lack a number. They belong in the decision, even if only in your judgment.

**Be transparent with stakeholders.** If you report ROI to a board, a partner, or a lender, show your assumptions and your method, not just the headline number. Let others check your work.

**Separate the money decision from the people decision.** A positive ROI does not automatically mean "cut staff." It means the tool pays for itself. What you do with the freed time and money is a separate, human choice.

An honest ROI calculation protects you from fooling yourself and protects your people from being a line item in a rigged number.

## Mistakes to Avoid

### 16.6 Errors of evaluation

**No clear objective.** Spending without a measurable goal, so you can never tell if it worked. Define the metric first.

**No baseline.** Not measuring the starting point, so any change is unprovable. Measure before you start.

**Ignoring indirect costs.** Counting only the subscription and forgetting setup, staff time, the learning dip, and maintenance. The hidden costs are where projects die.

**Overestimating savings.** Believing the vendor's best-case promise instead of your own measured reality. Be conservative.

**Counting gross instead of net.** Reporting the total benefit without subtracting the cost. ROI is about the *net* gain.

**Double counting.** Counting the same saving twice, or counting a benefit that overlaps with one already counted.

**Ignoring the learning curve.** Assuming full savings from day one. Real savings ramp up over weeks.

**Too short a time horizon.** Judging a tool after two weeks, before the benefits show. Give it a fair period, usually a year.

**Ignoring maintenance.** Forgetting that costs continue after launch. A tool that needs constant tending may never pay off.

**Treating the non-quantifiable as zero.** Discarding real benefits because they lack a number. List them and weigh them.

**ROI theater.** Doing the math backward to justify a decision already made. Use the method to decide, not to decorate.

**Never re-running the numbers.** Staying on the projection and never checking against reality. Re-measure after launch and learn.

## Practical Exercise

### 16.8 Calculate the ROI of one activity

Pick one activity in your business that AI could help with — answering emails, processing invoices, summarizing documents, scheduling. Run the full method on it.

**Step 1 — Define the objective.** Write one sentence: *"By [when], we will change [metric] from [baseline] to [target]."* If you do not know the baseline, go measure it this week before continuing.

**Step 2 — Measure the baseline.** How much time or money does this activity cost you now, per month or per year? For time, multiply hours by a fully-loaded hourly cost (salary plus overhead). Write the number down.

**Step 3 — List all costs.** Direct costs (subscription, setup, hardware, external help, training) plus indirect costs (your staff's time to set up and run it, the learning dip, maintenance, review time). Add them into a first-year total and a steady-year total.

**Step 4 — Estimate the benefit.** How much time or money will AI realistically save? Be conservative. Use a fraction of the baseline you measured, not a fantasy. Convert saved time to money at your hourly cost.

**Step 5 — Compute ROI.** Net Benefit = Total Benefit − Total Cost. ROI = (Net Benefit ÷ Total Cost) × 100%.

**Step 6 — Compute payback.** Divide the total cost by your monthly savings to see how many months until it pays for itself.

**Step 7 — List the non-quantifiable benefits.** Write down the benefits you cannot price — morale, customer happiness, less stress. Note them beside the number.

**Step 8 — Decide.** Is the ROI clearly positive with a short payback? Strong case. Thin margin? Be cautious. Negative? Walk away or find more benefit.

Write the whole thing on one page. That page is your decision. Keep it, and after you launch, fill in the *actual* numbers and compare. The gap between your estimate and reality is the lesson you will carry to the next project.

## Checklist

### 16.9 Economic checklist

Before spending on any AI project, check these.

- [ ] **You have one clear, measurable objective** with a single metric.
- [ ] **You have measured the baseline** (the current number) before starting.
- [ ] **You have a specific target and a time frame.**
- [ ] **You have listed all direct costs** — subscription, setup, hardware, external help, training.
- [ ] **You have listed all indirect costs** — staff time, learning dip, maintenance, review, compliance.
- [ ] **You valued staff time at a fully-loaded rate**, not just take-home pay.
- [ ] **You estimated savings conservatively**, not from vendor hype.
- [ ] **You computed Net Benefit** (total benefit minus total cost).
- [ ] **You computed ROI** = (Net Benefit ÷ Total Cost) × 100%.
- [ ] **You computed the payback period** in months.
- [ ] **You listed the non-quantifiable benefits** and weighed them in your judgment.
- [ ] **You used a fair time horizon** (about a year), not a few weeks.
- [ ] **You did not double count** any benefit.
- [ ] **You will re-run the numbers with actual results** after launch.
- [ ] **You kept the money decision separate from the people decision.**

If a box is empty, the economics are not settled. Fill it before you spend. A number you can trust is worth more than a promise you cannot check.

## Key Takeaways

- ROI = (Net Benefit ÷ Total Cost) × 100%, where Net Benefit = Total Benefit − Total Cost; a positive number with a short payback is a strong case to proceed.
- Define one measurable objective with a real baseline before you spend — without a starting number, you can never prove the change.
- The visible price is only half the cost; count indirect costs like staff time, the learning dip, and maintenance, or you will fool yourself.
- Monetize what you honestly can and write down the rest — non-quantifiable benefits like morale and customer happiness still belong in the decision.
- Use the method to decide, not to decorate: honest numbers protect you from bad choices and your people from being a rigged line item.
