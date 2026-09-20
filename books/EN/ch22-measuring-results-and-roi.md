# Chapter 22 — Measuring Results and ROI

## In Simple Words

You changed something. Did it work? This chapter is about answering that question with facts instead of feelings.

It is very easy to *feel* like a new AI tool is helping, especially right after you bought it. You are excited, you want it to succeed, so you notice the good moments and ignore the bad. Six months later, nobody can say whether it actually saved time, cut errors, or cost more than it returned. The money is gone and the lesson is lost. Measuring is the habit that prevents this. It turns "I think it is working" into "it cut our processing time by 40%, and here is the number."

The full method for calculating return on investment — the formula, the cost list, the worked example — lives in [Chapter 16 — Goals, Costs, and Return on Investment](ch16-goals-costs-and-return-on-investment.md). That chapter is the home of the ROI method. Do not relearn it here. This chapter builds on it and answers the next set of questions: *what* small set of numbers should you actually watch, how do you keep watching them without drowning in data, and when should you stop a project or correct its course.

A simple image to carry: measuring is like the dashboard in a car. You do not stare at every gauge all the time, but you glance at a few key ones constantly — speed, fuel, engine warning. If you drive with the dashboard covered, you will run out of fuel or overheat the engine and not know why. A business change without a dashboard is driving blind. This chapter helps you build a small, honest dashboard and read it regularly.

One honest warning: numbers can be made to say almost anything if you want them to. You can pick the metric that flatters you, start counting at the best moment, or forget the costs. The whole point of measuring is to find the truth, not to decorate a decision you already made. Build your dashboard to catch you being honest.

## A Bit of History

**Early 1900s: "what gets measured gets managed."** Often credited to management thinker Peter Drucker (though he may not have coined it exactly), this phrase captured a powerful truth: you cannot improve what you do not track. If nobody counts the hours a task takes, it never gets faster. If nobody counts the errors, they never go down. Measurement turned management from guesswork into something you could steer.

**1950s–1970s: metrics spread through industry.** Factories tracked output, defect rates, and downtime. Quality movements like those of W. Edwards Deming made measuring defects central to improving production. The idea spread: pick a few numbers that reflect what you care about, watch them, and act on them.

**1990s: the balanced scorecard.** Kaplan and Norton argued that money alone is a poor measure of health. A company can look profitable while its customers are unhappy and its staff are leaving. They pushed the "balanced scorecard" — a small set of measures covering money, customers, internal processes, and learning. This is the direct ancestor of the simple four-part dashboard you will build in this chapter.

**2000s: dashboards go digital.** Software made it easy to collect and display data, and dashboards became a standard management tool. But ease brought a new problem: people started tracking everything, producing dashboards with fifty charts nobody read. The lesson flipped — the skill was no longer collecting data, it was choosing the few numbers that actually matter and ignoring the noise.

**2010s: the vanity-metric trap.** In the startup world, a term appeared for numbers that look impressive but mean nothing: "vanity metrics." A website with a million visits but no sales. An app with downloads but no active users. The trap is measuring something that feels good instead of something that reflects real value. This is the most common failure mode in AI measurement today — counting how many times a tool was used instead of whether it produced value.

**2020s: AI makes measurement essential and tricky.** AI can produce real, measurable gains, but it also produces plausible-looking output that can be wrong, so measuring quality — not just quantity — is now critical. And because AI projects are easy to start and hard to evaluate, the discipline of measuring, and of knowing when to stop, has never mattered more.

The arc: from "measure to manage" to "measure the right few things, honestly, and keep watching." The tools got easier; the discipline of choosing well and staying honest got harder.

## Curiosity

### 22.5 The company that cut cycle times by 50%

IBM has reported cutting the time spent on certain security and vendor-risk review tasks by roughly **50%** by automating parts of the work with AI — turning a slow, manual review process into a much faster one.

That is the headline. The full IBM case, with the details and the lessons behind the number, is told in [Chapter 30 — IT and Leadership](ch30-it-and-leadership.md), the canonical home of the IBM story. The point for this chapter is one line: a halving of cycle time is a real, measurable benefit — and it is exactly the kind of result a good dashboard is built to reveal and track over time.

## A Real Business Example

*The following is an illustrative composite of common real-world patterns, not a single named company.*

A mid-sized insurance agency adopted an AI tool to draft responses to customer claims inquiries. The owner wanted to know if it was worth it, so she set up a simple dashboard before launch and filled it in every week for six months.

The dashboard had four numbers, each with a "before" baseline and a running "now" value:

- **Time per response.** Before: 22 minutes on average. After six months: 9 minutes.
- **Error rate.** Before: about 6% of responses needed a correction after being sent. After: 4%.
- **Cost per response.** Before: roughly €5.50 in staff time. After: €2.30.
- **Customer satisfaction.** Before: 3.6 out of 5. After: 4.1 out of 5.

Every number moved the right way, and the owner could see it week by week. The tool paid for itself in about three months and kept returning after that. Because she had the numbers, the decision to expand the tool to a second team was easy and confident.

But here is the more interesting part. In month two, the error rate briefly jumped from 6% to 8%. The dashboard caught it immediately. They looked and found the cause: a new type of claim the tool had not been trained on was producing confident but wrong drafts. Because the dashboard flagged it early, they added a rule to route that claim type to a human, and the error rate fell back down. Without the dashboard, those wrong responses might have gone out for weeks before anyone noticed.

The dashboard did two jobs: it proved the value, and it caught a problem early. That is what a good dashboard is for.

## How to Do It

### 22.1 Simple KPIs: time, errors, costs, satisfaction

A **KPI** stands for **Key Performance Indicator** — a plain phrase for "a number that tells you how you are doing." The art is to pick a few that matter and ignore the rest. For almost any AI change, four KPIs cover what you need. They map directly to the four things you care about: is it faster, is it more accurate, is it cheaper, and are people happy.

**Time.** How long does the task take now versus before? This is the most common benefit of AI and the easiest to measure. Measure the time for one unit of work — one invoice, one email, one report — and compare it to your baseline. Time saved is the benefit you can most often turn into money (by valuing an hour at its real cost, as Chapter 16 shows).

**Errors.** How often does the work come out wrong? Count the mistakes that reach the end — a wrong figure in a report, a wrong answer sent to a customer, a claim processed incorrectly. AI can reduce errors, but it can also create new, confident ones. Measuring errors is not optional; it is how you catch a tool that sounds right and is wrong. Track both the error rate and the *type* of error, because the type tells you what to fix.

**Costs.** What does a unit of work cost now, all in? Take the time cost plus the tool's share of subscription and any review time. Compare to the before cost. This is where you see whether the savings are real after you subtract what the tool costs you. Remember the lesson from Chapter 16: count the full cost, including the human review time, or the number lies.

**Satisfaction.** Are the people who use it, and the customers who receive its output, happy? This is the KPI people forget, and it matters. A tool that is fast and cheap but makes staff miserable or customers annoyed is not a success. Measure staff satisfaction with a simple question ("Is this tool helping you, on a scale of 1 to 5?") and customer satisfaction with the feedback you already collect, or a short survey.

Four numbers: faster, more accurate, cheaper, happier. If all four move the right way, you have a clear win. If some move and some do not, that is the interesting signal to investigate. Keep it to these four. A small business does not need a dozen metrics. Four honest ones beat forty vanity ones.

### 22.2 A minimal dashboard

A dashboard is just a single page where your KPIs live, so you can see them at a glance. It does not need software. A spreadsheet, a whiteboard, or a sheet of paper taped to the wall all work. The rule is simple: **one page, four numbers, each with a before and a now.**

Here is the minimal layout. For each KPI, keep three columns:

| KPI | Before (baseline) | Now | Target |
|-----|-------------------|-----|--------|
| Time per unit | 22 min | 9 min | 10 min |
| Error rate | 6% | 4% | 3% |
| Cost per unit | €5.50 | €2.30 | €2.50 |
| Satisfaction | 3.6 / 5 | 4.1 / 5 | 4.0 / 5 |

Three columns per number, and the whole thing fits on one page. The **baseline** is what you measured before you started (never skip this — without a baseline you can prove nothing). The **now** is the current value, updated regularly. The **target** is what you aimed for.

Good dashboard rules:

- **One page only.** If it grows beyond one page, you have too many numbers. Cut some.
- **Always show the baseline.** A number without a "before" is meaningless. "9 minutes" tells you nothing; "down from 22 to 9" tells you everything.
- **Show the trend, not just the snapshot.** A tiny arrow or a simple line showing the last few weeks tells you the direction. A single number tells you where you are but not where you are heading.
- **Make it visible.** Put it where the team sees it — a shared screen, a wall, the start of the weekly meeting. A dashboard nobody looks at is not a dashboard.
- **Keep it cheap to update.** If updating the dashboard takes an hour a week, you will stop doing it. Make it a ten-minute job. If you can pull numbers automatically, good; if not, a quick manual count is fine.

The point of a minimal dashboard is not to look professional. It is to make the truth easy to see and impossible to ignore.

### 22.3 Continuous monitoring

A dashboard you fill in once is a photo. A dashboard you update every week is a live monitor. The value is in the watching over time, because that is where the real signal lives.

**Update on a fixed rhythm.** Pick a cadence — weekly is usually right for a small business — and update the same day every week. The rhythm matters more than the exact frequency. A weekly update catches problems within a week. A quarterly update lets a problem run for three months. Set a recurring reminder and make it a habit.

**Look for the trend, not the single point.** One week's number can be a fluke. Three weeks of the same direction is a signal. If time saved is creeping up week after week, the tool is settling in well. If errors are creeping up, something is drifting. Read the line, not the dot.

**Watch for drift and decay.** AI tools can quietly get worse over time. Data changes, customer questions change, the tool's model may update, and what worked in month one may not work in month six. Continuous monitoring catches this slow decay. A tool that was a clear win at launch can quietly become a liability if nobody keeps watching. This is why monitoring never really ends.

**Set a warning threshold.** Decide in advance what number should trigger action. For example: "If the error rate goes above 7%, we stop and investigate." A pre-set threshold stops you from slowly accepting a worsening number. When the line crosses the threshold, you act — no debate, no "we'll look at it later."

**Review it in the weekly meeting.** Make the dashboard the first item on the team's weekly agenda. Five minutes looking at the four numbers together keeps everyone focused on reality, surfaces problems fast, and shares the wins. It also signals that measurement matters here, which makes people take it seriously.

**Compare to the plan, not to the hype.** Measure against your own baseline and your own target, not against a vendor's promise or a competitor's story. Your numbers are the only ones that describe your business.

### 22.4 When to stop or correct a project

Not every project should continue. Some should be corrected. Some should be stopped. Measuring gives you the honest signal to make that call early, before you have sunk more money and time into something that is not working. There are three possible decisions, and the dashboard tells you which one you are facing.

**Keep going.** All four KPIs are moving the right way, or close to it. The tool is delivering. Continue, and consider expanding it to other tasks or teams. This is the easy decision.

**Correct and continue.** The tool has value, but one or more numbers are off. This is the most common outcome, and it is not failure — it is information. A high error rate on one type of task means: route that task type to a human. A satisfaction score that is low among staff means: the training was weak, retrain. A cost that is higher than expected means: find the hidden cost and cut it. Correct the specific problem and keep going. Most good projects spend some time in "correct and continue."

**Stop.** The numbers show the tool does not deliver value, and the problems are not fixable. Maybe it is slower than doing the work by hand. Maybe the error rate is too high to trust on any task. Maybe the cost never comes down below the benefit. If honest measurement shows a negative return with no clear path to fix it, stop. Stopping early is a success, not a failure — it means you learned the truth and saved yourself from throwing good money after bad.

**How to decide between correct and stop.** Ask three questions. First, *is the core value there?* If the tool saves real time on most tasks, the core value exists and you should correct, not stop. Second, *is the problem fixable?* A routing rule, a retraining, a cost cut — these are fixable, so correct. If the problem is fundamental (the tool simply cannot do the task well), it is not fixable, so stop. Third, *what is the sunk-cost trap telling me?* Be honest: are you continuing only because you already spent money? That is the sunk-cost fallacy. Decide on the future numbers, not the past spending.

**Set a review date before you launch.** Before you start, decide when you will judge the project — usually three to six months in. At that date, look at the dashboard and make the keep / correct / stop call deliberately. A pre-set review date stops a failing project from drifting on forever by default. It forces the decision while there is still time to recover the investment.

**Stopping well.** If you stop, do it cleanly and learn from it. Write down why it failed — wrong process, bad data, tool could not handle the task, cost too high. That lesson is valuable and reusable. A well-stopped project that teaches you something is worth more than a zombie project that limps along proving nothing.

## Ethics and Responsibility

Measurement is where honesty is tested most, because the numbers can justify decisions that affect real people.

**Measure to learn, not to justify.** Use the dashboard to find the truth, not to prove you were right all along. If the numbers show the tool is not working, that is a finding to act on, not an embarrassment to hide.

**Do not pick flattering metrics.** Choosing a number that only shows the good side — like counting how many times the tool was used instead of whether its output was good — is a lie told with a spreadsheet. Pick metrics that reflect real value, including the ones that might show a problem.

**Do not hide the errors.** It is tempting to undercount mistakes, especially errors the AI made confidently. Report them honestly. A hidden error rate is a loaded gun pointed at a future customer.

**Do not use measurement as surveillance.** Tracking KPIs about a *process* is healthy. Using the same data to spy on individual employees, rank them, and punish them poisons trust and turns measurement into a weapon. Measure the work, not the person. Keep the focus on improving the process.

**Be transparent with the numbers.** Share the dashboard with the team, including the bad weeks. When people see the honest picture, they trust the decisions that come from it. When they only see the polished version, they suspect the whole thing.

**Separate the money truth from the people decision.** A dashboard that shows a tool saves money does not automatically mean "cut staff." As Chapter 16 stresses, the money decision and the people decision are separate. Measure the money honestly, then decide about people humanely and on its own merits.

## Mistakes to Avoid

**No baseline.** Not measuring the "before," so you can never prove the "after" improved anything. Measure before you start.

**Vanity metrics.** Counting usage, clicks, or downloads instead of value. A tool used a thousand times that produces wrong answers is a failure, not a success.

**Measuring only the good.** Reporting the wins and hiding the errors and the bad weeks. A one-sided dashboard is a dishonest dashboard.

**Too many numbers.** A fifty-chart dashboard nobody reads. Four honest KPIs beat forty ignored ones.

**Forgetting the cost side.** Measuring time saved but not the tool's cost and the human review time. The saving looks real until you subtract what it costs.

**Snapshot instead of trend.** Looking at one number once instead of the direction over weeks. A single point is a fluke; the trend is the truth.

**Not watching for decay.** Assuming a tool that worked at launch keeps working forever. Quietly degrading tools need continuous monitoring.

**No warning threshold.** Letting a bad number creep up because there was no pre-set line that says "act now."

**The sunk-cost trap.** Continuing a failing project only because you already spent money. Decide on future value, not past spending.

**No review date.** Letting a project drift forever because nobody scheduled the moment to judge it.

**Measurement as a weapon.** Using process data to surveil and punish individuals. Measure the work, not the person.

**Confusing activity with achievement.** Mistaking "we did a lot with the tool" for "the tool created value." Only the four KPIs tell you which.

## Practical Exercise

### 22.7 Exercise: a dashboard of results

Build a one-page dashboard for one AI change you have made or are planning. Do it before launch if you can; if you already launched, build it now and reconstruct the baseline as best you can.

**Step 1 — Pick the four KPIs.** Write down, for your specific task: the time per unit, the error rate, the cost per unit, and the satisfaction score. If one does not apply, note why and keep the other three.

**Step 2 — Set the baseline.** For each KPI, write the "before" number. If you did not measure before launch, estimate honestly from memory or a quick sample count now, and label it as a reconstruction. Do not skip the baseline.

**Step 3 — Set the target.** For each KPI, write the number you are aiming for. Make it realistic, not a fantasy.

**Step 4 — Build the table.** Make the four-row, three-column table (Before / Now / Target) on a spreadsheet or a sheet of paper. Keep it to one page.

**Step 5 — Set the update rhythm.** Choose a day and time each week to update the "Now" column. Put it in your calendar. Make it a ten-minute job.

**Step 6 — Set the warning thresholds.** For each KPI, decide the number that should trigger action. Write it next to the row. For example, "error rate above 7% = stop and investigate."

**Step 7 — Set the review date.** Pick a date three to six months out when you will look at the whole dashboard and make the keep / correct / stop decision. Write it on the page.

**Step 8 — Make it visible.** Put the dashboard where you and the team will see it weekly. Add it to the top of your weekly meeting agenda.

Now update it every week. Watch the trends. When a line crosses a threshold, act. At the review date, make the call deliberately. This one page is the difference between knowing whether your change worked and guessing.

## Checklist

### 22.8 Measurement checklist

Before and during any AI project, check these.

- [ ] **You measured the baseline** (the "before" number) for each KPI before launch.
- [ ] **You have a small set of KPIs** — time, errors, costs, satisfaction — not dozens.
- [ ] **You set a realistic target** for each KPI.
- [ ] **Your dashboard is one page** with Before / Now / Target for each number.
- [ ] **You are not tracking vanity metrics** (usage, clicks) instead of value.
- [ ] **You count the full cost**, including the tool's price and the human review time.
- [ ] **You track errors, including confident-but-wrong ones**, and note their type.
- [ ] **You measure satisfaction** from both staff and customers.
- [ ] **You update the dashboard on a fixed weekly rhythm.**
- [ ] **You read the trend, not a single snapshot.**
- [ ] **You watch for slow decay** over months, not just the launch result.
- [ ] **You set warning thresholds** that trigger action automatically.
- [ ] **You review the dashboard in the weekly meeting.**
- [ ] **You compare to your own baseline**, not to vendor hype.
- [ ] **You set a review date** (3–6 months) to decide keep / correct / stop.
- [ ] **You avoid the sunk-cost trap** and decide on future value, not past spending.
- [ ] **You report the bad weeks honestly**, not just the wins.
- [ ] **You measure the process, not the person** — no surveillance or ranking.
- [ ] **You keep the money decision separate from the people decision.**

If a box is empty, you are partly driving blind. Fill it. A small, honest dashboard that you actually watch is worth more than any promise a vendor can make.

## Key Takeaways

- Measure to learn the truth, not to decorate a decision you already made — pick KPIs that reflect real value, including the ones that might show a problem.
- Four KPIs cover almost everything: time, errors, costs, and satisfaction; a one-page dashboard with a baseline for each is enough.
- The value is in continuous monitoring — read the weekly trend, watch for slow decay, and act when a number crosses a pre-set warning threshold.
- Measurement gives you three decisions: keep going, correct and continue, or stop; stopping early on honest numbers is a success, not a failure.
- Avoid the sunk-cost trap and the vanity-metric trap — decide on future value and real outcomes, not past spending or impressive-but-meaningless counts.
