# Chapter 29 — Operations and Production

## In Simple Words

Operations is the engine of a business. It is everything that turns inputs into outputs: making a product, moving it, keeping the machines running, checking the quality, and keeping people safe. Production is the part of operations that actually makes the thing. When the engine runs well, customers get what they ordered, on time, without defects. When it stutters, everything downstream feels it.

Think of your operation as a factory floor, whether you make widgets or deliver services. Machines run, goods move, people work, and something can always go slightly wrong — a machine that is about to fail, a batch with a defect, a delivery that will be late, a worker in an unsafe spot. A good operator sees these things early. AI helps by watching everything at once and flagging the small signals that a tired human eye misses.

This chapter covers four jobs: predictive maintenance (fixing machines before they break), quality control (catching defects automatically), logistics (moving goods and information efficiently), and workplace safety (keeping people out of harm's way). Each is a place where a small business can cut waste, raise quality, and protect its people.

One honest idea first: AI in operations is a *watcher and a helper*, not an autopilot that runs the floor alone. It senses, predicts, and suggests. A person still decides when to stop a line, when to reject a batch, and when to send someone home because it is not safe. The method for judging whether any of this pays off lives in [Chapter 16 — Goals, Costs, and Return on Investment](ch16-goals-costs-and-return-on-investment.md); this chapter shows you what to automate and how. To see where operations sits on the impact-and-effort map for your whole business, look at [Chapter 12 — Where AI Can Help Your Business](ch12-where-ai-can-help-your-business.md).

## A Bit of History

**1900s–1950s: the assembly line and preventive maintenance.** Modern production began with the moving assembly line, which broke work into small repeatable steps. Alongside it came *preventive* maintenance — the habit of servicing a machine on a fixed schedule, like changing a car's oil every few thousand miles, whether it needed it or not. This reduced breakdowns but wasted service on machines that were fine.

**1960s–1980s: automation and quality control.** Factories added automated machines and formal quality control — inspecting products against a standard and sorting the good from the bad. Statistical quality methods caught defects in batches. This raised quality but still relied on humans to inspect and on fixed rules to service machines.

**1990s: sensors and the digital supply chain.** Cheap sensors let machines report their own condition — temperature, vibration, run hours. Supply chains became digital, with software tracking goods from supplier to customer. For the first time, an operator could see, on a screen, what was happening across the floor and across the supply chain. But the data was mostly read by hand.

**2000s: machine learning predicts the failure.** Machine learning — software that learns patterns from many examples — changed maintenance. Instead of servicing on a fixed schedule, you could learn from sensor data when a machine was *actually* about to fail. A rising vibration pattern that a human could not feel became a clear warning days in advance. This was the birth of *predictive* maintenance.

**2010s: computer vision inspects quality.** Computer vision — AI that reads what a camera sees — began to inspect products automatically. A camera could spot a crack, a scratch, or a missing part faster and more consistently than a human inspector, and without getting tired. Quality control moved from sampling to checking every unit.

**2020s: agents run the workflow.** Large language models and AI agents — software that takes a whole task and carries it through several steps — now run parts of the operational workflow itself: reading a request, pulling data from backend systems, and executing the next step. The SOK Finance example below is exactly this: AI agents handling the day-to-day service operations of a financial service center, with humans supervising.

The arc: from fixed schedules, to manual inspection, to sensor data, to AI that predicts and sees, to agents that act. Each step moved the watching and the routine work to software and left humans to decide and to intervene.

## Curiosity

### 29.5 The service center that put AI agents on the front line

When we hear "operations and production," we picture a factory. But operations also means the service center that keeps a business running — the place where requests arrive and someone must act on them fast.

SOK Finance, in Finland, runs a service center called Palveluässä that provides financial management and payroll services for the S Group — a customer-owned Finnish network of retail and service companies with roughly 2,000 outlets. Every day, requests arrive: "Send me a copy of this invoice," "Change the due date on this payment." Routine, high-volume, and time-sensitive.

The curiosity is what the company did with it. Instead of hiring more people to answer the same requests, they put AI *agents* on the front line to handle the routine ones, so the human staff could focus on the cases that needed judgment. That shift — from humans doing every request to agents doing the routine and humans supervising — is the same quiet revolution that happened on the factory floor, now applied to a service center. The full story, with the real source, is below.

## A Real Business Example

**SOK Finance: AI agents running the service-center workflow.**

SOK Finance operates the Palveluässä service center, which provides financial management and payroll services for the S Group, a customer-owned Finnish network of retail and service companies with approximately 2,000 outlets. The service center handles a steady stream of routine requests from across that network — things like asking for a copy of an invoice or changing a payment due date. Each request is small, but together they are a large, repetitive workload that must be handled quickly and consistently.

According to a CGI press release (Helsinki, 23 April 2026), CGI designed, implemented, and deployed a **multi-agent AI solution built on AWS Bedrock** for SOK Finance, bringing AI into live production use in financial administration and customer service. A "multi-agent" solution means several AI agents work together on a task, each handling a step. In this case, the agents process incoming customer-service messages, retrieve the needed data from backend systems, and automatically carry out parts of the process.

The release describes the solution as significantly accelerating routine processes such as **invoice copy requests and due-date changes**, and as improving efficiency and consistency compared with the previous manual handling. CGI was responsible for the design, the implementation, the deployment, and the integration with SOK Finance's key systems.

Two things are worth noticing. First, the human role shifts from *doing every request* to *supervising the agents and handling the exceptions*. The agents take the routine; the people take the unusual and the sensitive. Second, the win is consistency as much as speed — an agent follows the same careful steps every time, where a tired person on a busy afternoon might slip.

A note on the source and the numbers: the figures above come from CGI's published announcement. The release describes the results in qualitative terms — faster processes, better consistency — and does not publish a hard percentage for time saved or cost reduced. Treat the outcome as the company's reported experience, and remember that your own numbers will depend on your volume and your systems. The point of the case is the *pattern*: AI agents running a routine service workflow in production, with humans supervising, at the scale of a 2,000-outlet network.

## How to Do It

### 29.1 Predictive maintenance

Predictive maintenance means fixing a machine *before* it breaks, by predicting the failure from data instead of waiting for it to happen or servicing on a fixed schedule.

**The old way and its cost.** Traditionally you had two choices: run a machine until it failed (and pay for an unplanned stop), or service it on a fixed schedule (and waste money servicing machines that were fine). Both lose. An unplanned breakdown stops production at the worst moment and costs far more than a planned fix.

**How AI predicts.** You put sensors on the machine to measure things like vibration, temperature, sound, and run hours. AI learns the normal pattern and spots the early signs of trouble — a vibration that is slowly rising, a temperature that runs a little hot. Those small changes often appear days before a failure. The AI warns you in time to fix the machine during a planned stop, not in the middle of a run.

**What it saves.** The big saving is avoiding unplanned downtime — the surprise breakdown that halts everything. A planned fix on a Tuesday afternoon is cheap; a breakdown during your biggest order of the month is expensive. Predictive maintenance turns the second into the first.

**Start small.** You do not need sensors on every machine. Start with the one or two machines whose failure hurts most — the bottleneck, the one with the long repair time, the one that stops the whole line. Put a few sensors on it and watch. Prove the value there before you expand.

**The human decides the stop.** AI flags the risk; a person decides when to take the machine down. Do not let the system stop production on its own without a human confirming the call. The warning is the value; the decision stays human.

### 29.2 Quality control

Quality control means checking that a product meets its standard and catching defects before the product reaches the customer. AI changes quality control from *sampling* to *checking every unit*, and from *tired eyes* to *consistent ones*.

**Computer vision inspects.** A camera plus AI can look at each product on the line and spot a crack, a scratch, a missing part, a wrong label, or a bad seam. It checks every unit, not just a sample, and it does not get tired or bored. A human inspector checking thousands of units a day will miss things; the camera will not.

**Consistency is the win.** Humans vary. A person is sharper in the morning, slower after lunch, and easily swayed by what they saw last. AI applies the same standard to every unit, all day. That consistency is worth a lot in a business where a defect reaching a customer costs a return, a complaint, or a reputation.

**Catch it early.** The earlier you catch a defect, the cheaper it is. A defect caught at the machine that made it costs one part. The same defect caught at final assembly costs a rework. Caught by the customer, it costs a return and trust. AI at each station catches problems at the source, not at the end.

**Start with the costly defect.** Do not try to inspect everything at first. Find the defect that costs you the most — the one that causes the most returns or complaints — and put a vision check on that. Prove it catches the expensive problem, then add more checks.

**Keep a human for the judgment call.** AI can flag a suspect unit; a person decides whether it is truly defective, especially for borderline cases. Do not let a vision system scrap good product because it was too strict. Review the rejects and tune the threshold.

### 29.3 Logistics

Logistics is the movement of goods and information: getting the right thing to the right place at the right time, at the lowest cost. It is a puzzle of routes, stock, timing, and suppliers, and AI is very good at puzzles like this.

**Route and delivery optimization.** AI can plan delivery routes that save miles, fuel, and time, taking traffic, delivery windows, and load size into account. For a business with a fleet, even a small saving per route adds up fast across a year.

**Stock and demand forecasting.** AI looks at your sales history and predicts what you will need and when, so you stock enough without over-buying. Too little stock means a missed sale; too much means cash tied up and waste. AI balances the two by learning your patterns and seasonality.

**Spot the bottleneck.** AI can see where goods slow down — a supplier that is always late, a warehouse step that backs up, a route that always runs over. Seeing the bottleneck is the first step to fixing it. The whole value is making the invisible delay visible.

**Connect the systems.** Logistics AI works best when it can see your orders, your stock, and your deliveries together. Connecting AI to the systems you already use — your ordering, your inventory, your tracking — is what makes the picture complete. The how-to for that connection is in [Chapter 19 — Connecting AI to Systems You Already Use](ch19-connecting-ai-to-systems-you-already-use.md).

**Keep a human for the exception.** AI plans the routine; a person handles the surprise — the strike, the storm, the supplier that fails. Do not let an optimized plan run into a real-world disruption without a human ready to override it. The plan is a starting point, not a straitjacket.

### 29.4 Workplace safety

Workplace safety means keeping people out of harm's way. AI can watch for unsafe conditions and unsafe behavior and warn before an accident happens. This is one of the most valuable uses of AI, because the thing it protects is a person.

**Computer vision watches for hazards.** Cameras plus AI can spot a worker without the right protective gear, a person standing in a dangerous zone, a spill on the floor, or a blocked emergency exit. When it sees one, it raises an alert so the danger is fixed before someone is hurt.

**Predict the risky moment.** AI can learn when accidents are most likely — a certain shift, a certain machine, a certain time of day when people are tired — and increase the watch then. It is like having a safety officer who never blinks and sees the whole floor at once.

**A serious legal line: do not read emotions.** AI that infers a worker's *emotions* from their face or voice is prohibited in the workplace under the EU AI Act. Safety vision is about *hazards and gear*, not about how a worker *feels*. Keep the camera on the floor and the machine, not on the person's mood. The full list of banned practices is in [Chapter 5 — Rules and Legal Responsibility](ch05-rules-and-legal-responsibility.md).

**Tell your workers.** If you use AI-based safety monitoring that affects workers, you must inform your workers and their representatives before you start, as the law requires for high-risk AI at the workplace. Be open about what the cameras watch and why. Secrecy breaks trust. The worker-notice rule is covered in this chapter's Curiosity and in [Chapter 5](ch05-rules-and-legal-responsibility.md).

**Use it to protect, not to punish.** Safety data should make the workplace safer — fix the hazard, change the process, train the team. It should not become a tool to discipline individuals for every small slip. Use it to find and remove danger, not to build a case against a worker.

## Ethics and Responsibility

Operations touches safety and the environment, so the ethical stakes are real and concrete.

**Safety decisions stay human.** AI can warn of a hazard, but a person decides when to stop a line or send someone home. Never let a system make a safety-critical decision with no human in the loop. A false "all clear" can hurt someone.

**Respect workers' privacy and rights.** Cameras and sensors in the workplace watch over people. Use them for safety and operations, not for surveillance. Tell workers what is watched and why, and follow the privacy rules in [Chapter 10 — Privacy and GDPR](ch10-privacy-and-gdpr.md).

**Never read emotions.** Emotion recognition in the workplace is banned. Keep monitoring on hazards and gear, never on a worker's feelings.

**Protect operational data.** Sensor data, production schedules, and supply-chain records are sensitive and valuable. Keep them secure and, where it matters, within your own environment. The security basics are in [Chapter 6 — Cybersecurity in the AI Era](ch06-cybersecurity-in-the-ai-era.md), and the self-hosting option in [Chapter 8 — Self-Hosting: Keep Your Data Under Control](ch08-self-hosting-keep-your-data-under-control.md).

**Be honest about results.** A quality or efficiency number that looks too good should be checked before you report it. Report the real figures, including the misses, so you can fix what is still broken.

**Use data to improve, not to punish.** Operational and safety data should make the work better and safer for everyone. When it becomes a stick to beat individuals with, it poisons the workplace and hides the real problems.

## Mistakes to Avoid

**Waiting for the breakdown.** Sticking with run-to-failure when a planned fix was cheap and predictable. Predict and act early.

**Sensors without a plan.** Collecting data you never act on. Start with the machine that hurts most and tie every sensor to a decision.

**Letting AI stop or scrap on its own.** No human check on a line stop or a product reject. Keep the human decision.

**Too-strict vision checks.** A quality system that scraps good product because the threshold is too tight. Review rejects and tune it.

**Inspecting the wrong defect.** Putting vision on a cheap problem while the expensive one slips through. Target the costly defect first.

**A plan that ignores the real world.** Letting an optimized logistics plan run into a disruption with no human override. Keep a person ready.

**Emotion recognition at work.** Using AI to read workers' feelings. It is banned and wrong.

**Secret monitoring.** Not telling workers before AI-based safety or operations monitoring starts. That breaks the law and trust.

**Surveillance creep.** Using safety and operations data to watch and punish individuals instead of removing hazards.

**Automating a broken process.** If the line or the supply chain is a mess, AI makes a faster mess. Fix the process first.

**No baseline.** Not measuring downtime, defect rate, or delivery time before, so you cannot prove the gain. Measure first (see [Chapter 22 — Measuring Results and ROI](ch22-measuring-results-and-roi.md)).

**Over-promising the numbers.** Quoting a vendor's best-case figure as your result. Use your own measured numbers.

## Practical Exercise

### 29.7 Exercise: plan one operations automation

Pick one operations job and plan its AI assistance end to end, with safety and the human decision built in.

**Step 1 — Choose the job.** Pick one: predictive maintenance, quality control, logistics, or workplace safety. Do one, not all.

**Step 2 — Define the goal and the metric.** Less downtime? Fewer defects? Faster delivery? Fewer safety incidents? Pick one number to measure.

**Step 3 — Measure the baseline.** What is that number now? Hours of unplanned downtime, defect rate, on-time delivery, incidents per month. Write it down.

**Step 4 — Find the costly target.** Identify the single most expensive failure in that job — the machine whose breakdown hurts most, the defect that costs the most, the route that always runs late, the hazard that causes the most harm. Target that first.

**Step 5 — Mark each step.** For each step, mark it: **AI does it** (sense, predict, inspect, plan), **human reviews it** (confirm the warning, check the reject), or **human decides it** (stop the line, scrap the batch, send someone home). Every safety-critical decision must be human.

**Step 6 — Check the legal line.** If the job involves monitoring workers, confirm you are watching hazards and gear, not emotions, and plan how you will inform workers and their representatives before you start.

**Step 7 — Connect the data.** Decide which systems the AI needs to see — sensors, inventory, tracking — and how you will connect them (see [Chapter 19](ch19-connecting-ai-to-systems-you-already-use.md)).

**Step 8 — Launch small and measure.** Run it on one machine, one line, or one route first. Compare the metric to the baseline. Scale only what proves it works.

Do one job well. The costly-target analysis in step 4 is valuable on its own — it shows you where your operation actually loses the most money or causes the most harm, which is useful even before you buy any tool.

## Checklist

### 29.8 Operations and production checklist

Before automating any operations task, check these.

- [ ] **You measured the baseline** — downtime, defect rate, delivery time, safety incidents.
- [ ] **You targeted the most costly failure first**, not the easiest one.
- [ ] **A human makes every safety-critical decision** — stopping a line, scrapping a batch.
- [ ] **Predictive maintenance is tied to a real action**, not just collected data.
- [ ] **Quality checks are tuned** so they do not scrap good product.
- [ ] **Logistics AI can see your orders, stock, and deliveries together.**
- [ ] **A human can override the optimized plan** when the real world disrupts it.
- [ ] **Safety monitoring watches hazards and gear, never emotions** (emotion recognition is banned).
- [ ] **You informed workers and their representatives** before any AI monitoring that affects them.
- [ ] **Operational data is kept secure**, not sent to public AI services.
- [ ] **You use data to remove hazards and improve the process**, not to punish individuals.
- [ ] **You fix the broken process before automating it.**
- [ ] **You report your own measured numbers**, not the vendor's best case.

If a box is empty, the risk — to your product, your people, or your trust — is still yours. Fill it before you let AI near the floor.

## Key Takeaways

- AI in operations is a watcher and helper: it senses, predicts, inspects, and plans, while a human keeps every safety-critical decision.
- The SOK Finance case (a CGI announcement) put multi-agent AI on AWS Bedrock into live production at a service center serving a ~2,000-outlet network, accelerating routine requests like invoice copies and due-date changes, with humans supervising the exceptions.
- Predictive maintenance turns a surprise breakdown into a cheap planned fix; computer-vision quality control checks every unit consistently instead of sampling with tired eyes.
- In workplace safety, monitor hazards and protective gear — never workers' emotions, which the EU AI Act bans — and tell workers before any monitoring that affects them.
- Target the most costly failure first, keep a human override for real-world disruptions, and measure your own baseline before you trust any vendor's number.

<!-- BEGIN agentbridge-examples -->

## Try it with AgentBridge

Here is how the same job looks with AgentBridge. Each box shows the finished result and the one line you type to get it.

### Keep stock in order

![An inventory sheet with low-stock items highlighted](../../assets/examples/inventory-list.png)
*An inventory sheet with low-stock items highlighted*

**What you ask:** `Make an inventory spreadsheet with item, quantity, reorder level and supplier, and highlight what is below the reorder level.`

The agent sets up the inventory sheet and marks the items that need reordering. Update the quantities and ask it to re-check any time.

*Tip: A weekly scheduled check can tell you what to reorder before you run out.*

---

### Plan a delivery route

![A delivery route mapped across the stops](../../assets/examples/delivery-route.png)
*A delivery route mapped across the stops*

**What you ask:** `Plan the best route for these five delivery addresses and show it on a map.`

The agent plots the stops on a map in an efficient order and gives you the distance and estimated time. You follow the route and save fuel.

*Tip: Add time windows ('stop B before noon') and the agent factors them in.*

---

### Is it in stock?

![A live stock check answered in seconds](../../assets/examples/stock-check.png)
*A live stock check answered in seconds*

**What you ask:** `Do we have item SKU 3391 in stock, and how many?`

The agent checks the stock in your system and answers with the quantity, so you can promise or promise-against with confidence.

*Tip: Pair with a low-stock alert scheduled daily to avoid surprises.*

<!-- END agentbridge-examples -->
