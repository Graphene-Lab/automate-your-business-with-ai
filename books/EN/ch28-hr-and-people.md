# Chapter 28 — HR and People

## In Simple Words

Human resources is where a business meets its people. Hiring, training, helping new staff settle in, and understanding why people leave — these shape the whole company. They are also full of repetitive work: reading hundreds of CVs, answering the same onboarding questions, sorting training by role, and digging through old records to find why staff quit. AI can take the repetitive part of each job and leave the human part — judgment, fairness, and care — where it belongs.

Think of HR as a funnel and a garden at the same time. The funnel is hiring: many people enter at the top, and you narrow them down to a few good fits. The garden is everyone you already have: you water them with training, you watch for signs of trouble, and you try to keep them growing. AI helps at both ends. In the funnel, it sorts and shortlists faster than a person can read. In the garden, it spots patterns in a thousand small signals that no manager could hold in their head.

This chapter covers four jobs: screening CVs and applications, onboarding new hires, personalized training, and turnover analysis. Each is a place where a small business can save time and make better decisions about people.

One honest idea before we start: people are not invoices. A wrong number on an invoice costs money; a wrong decision about a person costs a life, a career, and your reputation. So AI in HR is a *helper*, never the *judge*. It reads, sorts, suggests, and flags. A person still decides who gets the job, who gets the promotion, and why someone is let go. And in Europe, hiring and worker management are treated as high-risk uses of AI, with real legal duties. The full treatment of the EU AI Act lives in [Chapter 5 — Rules and Legal Responsibility](ch05-rules-and-legal-responsibility.md); this chapter shows you what to automate and how, and where the law draws a line. The method for judging whether any of this pays off lives in [Chapter 16 — Goals, Costs, and Return on Investment](ch16-goals-costs-and-return-on-investment.md).

## A Bit of History

**1980s–1990s: the HR database.** The first big change in HR work was the computerized personnel file. Instead of paper folders in a cabinet, employee records lived in a database. Payroll, attendance, and personal details became searchable. This was the first time software touched the core of HR, and it set the pattern: store the data, keep the human in charge of decisions.

**1990s–2000s: the applicant tracking system.** As job applications moved online, companies adopted the applicant tracking system, or ATS — software that collects applications, stores them, and lets recruiters search and sort them. A recruiter could now see every applicant for a job in one place and filter by keywords. This brought order to the flood of online applications, but the filtering was simple: it matched words, not people.

**2000s: e-learning and the learning management system.** Training moved from the classroom to the screen. The learning management system, or LMS, delivered courses online and tracked who completed what. This made training scalable, but early versions were one-size-fits-all: everyone watched the same video, regardless of what they already knew.

**2010s: people analytics.** Companies began to analyze HR data the way they analyzed sales data. They looked at which hires stayed, which teams performed, and which signals predicted someone quitting. People analytics turned HR from a paperwork function into a data function. But it needed large datasets and skilled analysts, so mostly big companies could do it.

**2020s: large language models read and write about people.** Large language models — AI trained on huge amounts of text — can now read a CV and a job description and judge how well they match, draft a personalized training plan, and answer an employee's HR question in plain language. This is the newest step: AI that reads the words people write and reasons about them. It is powerful, and precisely because it is powerful, it is the area where the law is strictest.

The arc: from paper folders, to searchable databases, to keyword filters, to analytics, to AI that reads and reasons about people. Each step took more of the repetitive work off human hands — and each step raised the stakes for fairness, because the decisions are about human lives.

## Curiosity

### 28.5 The law says: tell your workers before AI touches their jobs

Here is a fact every European employer should know before switching on any HR tool that affects staff.

The EU AI Act has a specific rule about workers. In plain words: if you use a high-risk AI system in the workplace — one that affects decisions about your employees — you must tell your workers and their representatives *before* you start using it. The law states it directly in Article 26(7): "Before putting into service or using a high-risk AI system at the workplace, deployers who are employers shall inform workers' representatives and the affected workers that they will be subject to the use of the high-risk AI system."

Two things matter here. First, it is not optional. It is a legal duty, not a courtesy. Second, it is *before*, not after. You cannot roll out an AI screening tool and tell people a month later. You tell them first.

Why does this rule exist? Because people have a right to know when a machine is shaping their working life — whether a tool is reading their application, ranking their performance, or deciding their tasks. Secrecy about AI at work erodes trust and can hide unfairness. Telling people openly is the minimum a fair employer does.

A related warning: the same Act *bans* emotion recognition in the workplace — using AI to read a worker's feelings from their face or voice is prohibited except for medical or safety reasons. A tool that "detects" whether a call-center agent is happy or stressed to score them is squarely forbidden. The full list of banned practices and the staged dates are in [Chapter 5](ch05-rules-and-legal-responsibility.md). The point here is simple: be open about the AI you use on people, and never secretly read their emotions.

## A Real Business Example

**A mid-size firm that automated hiring and onboarding — an illustrative scenario.**

This example is illustrative. It is a realistic composite, not a reported company result, built to show how the four HR jobs fit together and where the human and the law sit.

Imagine a company of 400 people that hires about 80 staff a year, mostly for a few recurring roles: sales, support, and back-office. Every opening brings 200 to 400 applications. The two HR staff were drowning: reading CVs took days, onboarding questions repeated all day, and nobody knew why people left after a year.

They changed three things.

First, **CV screening with a human check.** They used an AI tool to read each application against the job description and produce a shortlist with a short reason for each match. The HR staff did not let the tool reject anyone. They reviewed the shortlist, and they also sampled a batch of rejected applications every week to check the tool was not unfairly dropping good candidates. The tool cut the screening time from days to hours. The decision stayed human.

Second, **an onboarding assistant.** They built a chatbot trained on their own handbook, policies, and FAQs. New hires could ask, "How do I request leave?" or "What is the expense policy?" and get an instant answer, day or night. The two HR staff stopped answering the same ten questions every day and spent their time on the new hires who genuinely needed a human — the nervous ones, the ones with unusual situations.

Third, **a turnover review.** They pulled two years of HR records into a simple analysis: who left, from which role, after how long, and what their last engagement survey said. The pattern was clear — support staff left most often after 12 to 18 months, and their exit comments clustered around pay and no clear path to grow. That one finding gave them a concrete fix: a pay review and a defined promotion path for support. They did not need fancy AI to act on it; they needed the pattern surfaced, which the analysis did.

Notice the shape of it. AI did the reading, the answering, and the sorting. Humans did the deciding, the caring, and the acting. And because the screening tool affected hiring — a high-risk use — the company told its workers and their representatives before switching it on, as the law requires. That is the model to copy.

## How to Do It

### 28.1 CV and resume screening

Screening CVs (résumés) is the classic HR time sink. A single job opening can bring hundreds of applications, and reading each one takes minutes. AI can read them all and produce a shortlist, so a human reviews a manageable pile instead of a mountain.

**What the AI does.** It reads each CV and the job description, then ranks or sorts the applications by how well they match. It looks at skills, experience, and keywords. Modern tools read the meaning, not just the words, so "managed a team of five" can match "leadership experience."

**The high-risk warning.** In the EU, using AI to screen job applications or filter candidates is a **high-risk** use under the AI Act, because it affects a person's livelihood. That brings real duties: transparency, human oversight, and care against bias. Read [Chapter 5](ch05-rules-and-legal-responsibility.md) before you deploy any screening tool. Do not treat a CV screener as "just software."

**Bias is the central danger.** An AI trained on past hires learns the patterns of past hires — including any past unfairness. If your company historically hired mostly men for a role, the tool may learn to down-rank women. If it learned to favor one university, it may drop equally good candidates from elsewhere. This is not hypothetical; it has happened in real systems. Guard against it: review the shortlist and the rejected pile for patterns, test the tool on diverse examples, and never let it auto-reject.

**Keep the human decision.** Use AI to shortlist and to explain *why* it matched. A person makes the call. A shortlist with reasons is far better than a bare ranking, because it lets the reviewer see the tool's logic and catch a bad match.

**Tell candidates and workers.** Be open that AI assists in screening, and tell your workers and their representatives before you switch it on, as the law requires. Candidate data is personal data; handle it under the privacy rules in [Chapter 10 — Privacy and GDPR](ch10-privacy-and-gdpr.md).

### 28.2 Onboarding

Onboarding is the first real experience a new hire has of your company. A good onboarding makes a person feel welcome, clear, and ready. A bad one leaves them confused and anxious. AI helps by answering the endless routine questions instantly, so the human side of onboarding — the welcome, the introductions, the reassurance — gets more time, not less.

**The onboarding assistant.** A chatbot trained on your handbook, policies, and common questions can answer a new hire at 9 p.m. the night before their first day: "What time should I arrive?", "What do I bring?", "How is payroll set up?" This removes the small confusions that make a first day stressful.

**A guided checklist.** AI can generate a personalized onboarding plan for each role: the accounts to open, the systems to access, the people to meet, the training to finish. Instead of one generic list, each new hire gets a path that fits their job. The tool tracks progress and nudges what is missing.

**Draft the welcome materials.** AI can draft the welcome email, the team introduction, and the first-week schedule, so the manager starts from a good draft instead of a blank page. The manager personalizes it. The human touch stays, but the busywork shrinks.

**What AI cannot replace.** The welcome coffee, the mentor, the manager who checks in on day three. Onboarding is emotional as much as practical. Use AI for the information and the checklist; keep a person for the welcome. A new hire who only ever talks to a bot feels like a number.

**Measure the first 90 days.** Track how long it takes a new hire to become productive and how they feel at 30, 60, and 90 days. If onboarding with AI is working, ramp-up time falls and early satisfaction rises. If it does not, the bot is not the answer — the process is.

### 28.3 Personalized training

Old training was one-size-fits-all: everyone watched the same course. Personalized training uses AI to adapt learning to what each person already knows and what their role needs. It is the difference between a set lecture and a tutor who knows where you are stuck.

**Adapt to the person.** AI can give a short starting quiz, see what a person already knows, and skip what they have mastered. It spends time only on the gaps. This respects the learner's time and makes training faster and more relevant.

**Adapt to the role.** A support hire needs different training than a sales hire, even in the same company. AI can assemble a learning path from your content library that fits the role, the level, and the person's pace.

**Draft the content.** AI can turn your existing documents — a policy, a product guide, a recorded meeting — into a short training module with questions to check understanding. This turns knowledge that already exists into training that people can actually use, without a specialist building every course.

**Answer questions while learning.** A learner can ask the AI about a tricky point and get an explanation in plain words, like a tutor. This is where large language models shine: they explain, rephrase, and give examples on demand.

**Keep it honest and checked.** AI-generated training must be reviewed by a human expert before it goes out. A confident but wrong training module spreads mistakes fast. Check the facts, check the tone, and keep a person available for the questions that matter. Training shapes how people work; it must be right.

### 28.4 Turnover analysis

Turnover means people leaving your company. High turnover is expensive — you lose skills, you re-hire, you re-train. Turnover analysis uses AI to look at your HR data and find *why* people leave, so you can fix the cause instead of guessing.

**What the AI looks at.** It combines records: who left, from which role, after how long, their pay, their manager, their last engagement survey, whether they were promoted, how often they were late. On its own, each fact is small. Together, they form a pattern.

**The pattern is the value.** AI can surface something like: "People in role X who have not been promoted in 18 months leave at three times the normal rate." That is a finding you can act on. No manager could hold a thousand records in their head and see it; the analysis can.

**Predict the risk, not the person.** Some tools flag which current employees show patterns similar to those who left. Use this to *start a conversation* — a check-in, a development plan — never to quietly mark someone as "likely to quit" and treat them differently. A prediction is a reason to care, not a reason to act against someone.

**Watch the small signals.** Engagement surveys, a drop in performance, a missed promotion, a change of manager — these are the small signals that often precede a resignation. AI is good at noticing them across many people at once. The human job is to respond with a real conversation.

**Privacy first.** Turnover analysis uses sensitive personal data. Handle it under the privacy rules in [Chapter 10](ch10-privacy-and-gdpr.md), keep it secure, and use it to improve conditions for the group, not to spy on individuals. The goal is a better workplace, not a surveillance system.

## Ethics and Responsibility

HR is the most sensitive place to use AI, because the output is a decision about a human life. The ethical bar is higher here than anywhere else in this book.

**A person decides about people.** AI reads, sorts, and suggests. A human makes every hiring, promotion, and termination decision. Never let a tool auto-reject a candidate or auto-fire a worker. The human must own the outcome and be able to explain it.

**Fight bias actively.** HR AI inherits the biases in its training data. Review outcomes across groups — gender, age, background — and look for unfair patterns. Test the tool before you trust it, and keep testing it after. Fairness is not a setting you turn on once; it is a habit you check.

**Be open with workers.** Tell your workers and their representatives before any high-risk AI touches their jobs, as the law requires. Secrecy about AI at work breaks trust and hides unfairness. Openness is both the law and the right thing.

**Never read emotions at work.** Emotion recognition in the workplace is prohibited under the EU AI Act. Do not buy or use a tool that scores staff by reading their faces or voices. It is banned, and it is wrong.

**Protect personal data.** HR data is among the most sensitive data a company holds — pay, health notes, performance, personal circumstances. Guard it, limit who sees it, and follow [Chapter 10](ch10-privacy-and-gdpr.md). Do not feed employee data into public AI tools without checking the security implications (see [Chapter 6 — Cybersecurity in the AI Era](ch06-cybersecurity-in-the-ai-era.md)).

**Use data to help, not to punish.** Turnover predictions and engagement data should make you a better employer — better pay, better growth paths, better conditions. They should never become a tool to watch, rank, or punish individuals. Measure the workplace, not the person as a target.

**Keep the human in the welcome.** In onboarding and in daily HR, AI handles information; humans handle care. A company that outsources all human contact to a bot loses the trust that makes a workplace work.

## Mistakes to Avoid

**Letting AI reject candidates.** The worst HR mistake. A tool that auto-rejects hides bias and kills good hires. Always keep a human decision.

**Ignoring bias.** Not checking whether the tool treats groups unfairly. Past hiring bias becomes future hiring bias if you do not look. Test and review.

**Switching on a high-risk tool in secret.** Not telling workers and their representatives before using AI that affects them. That breaks the law and trust.

**Buying an emotion-recognition tool.** It is banned in the workplace. A vendor pitch for "mood detection" on staff is a trap.

**Treating a prediction as a verdict.** Acting against an employee because a model flagged them as "likely to quit." A prediction is a reason to talk, not to punish.

**Surveilling staff.** Using HR data to watch and rank individuals instead of improving conditions for the group. This poisons trust.

**A bot-only onboarding.** A new hire who never talks to a human feels like a number. Keep the welcome human.

**Unreviewed AI training.** Publishing AI-generated training that is confidently wrong. A human expert must check it.

**Automating a bad HR process.** If your hiring or onboarding is broken, AI makes a faster broken process. Fix the process first.

**Leaking employee data.** Putting sensitive HR data into insecure AI tools. Check security and privacy first.

**No baseline.** Not measuring time-to-hire, ramp-up time, or turnover before, so you cannot prove the improvement. Measure first (see [Chapter 22 — Measuring Results and ROI](ch22-measuring-results-and-roi.md)).

**Forgetting the law is the floor.** Complying with the AI Act does not make a hiring tool fair. Ethics sits above compliance, and you own it (see [Chapter 4 — Ethical AI](ch04-ethical-ai-doing-the-right-thing.md)).

## Practical Exercise

### 28.7 Exercise: plan one HR automation responsibly

Pick one HR job and plan its AI assistance end to end, with the human and the law built in.

**Step 1 — Choose the job.** Pick one: CV screening, onboarding, training, or turnover analysis. Do one, not all.

**Step 2 — Define the goal and the metric.** Faster time-to-hire? Faster new-hire ramp-up? Lower turnover? Pick one number to measure.

**Step 3 — Measure the baseline.** What is that number now? How long does screening take? How long to ramp up? What is your turnover rate? Write it down.

**Step 4 — Classify the risk.** Is this a high-risk use under the AI Act? Screening and worker management are. If yes, you have legal duties: transparency, human oversight, bias care. Note them (see [Chapter 5](ch05-rules-and-legal-responsibility.md)).

**Step 5 — Mark each step.** For each step, mark it: **AI does it** (read, sort, draft, surface), **human reviews it** (check the shortlist, review the training), or **human decides it** (the hire, the promotion, the fix). Every decision about a person must be human.

**Step 6 — Build the bias check.** Decide how you will test for unfair patterns across groups, and how often you will review the rejected pile and the outcomes.

**Step 7 — Plan the worker notice.** Write how and when you will inform workers and their representatives before switching the tool on, as the law requires.

**Step 8 — Launch small and measure.** Run it on one role or one team first. Compare the metric to the baseline. Scale only what proves it helps and treats people fairly.

Do one job well. The bias check and the worker notice you build in steps 6 and 7 are valuable on their own — they force you to see your own hiring patterns, which is useful even beyond the tool.

## Checklist

### 28.8 HR and people checklist

Before using AI on people, check these.

- [ ] **You measured the baseline** — time-to-hire, ramp-up time, turnover rate.
- [ ] **A human makes every decision about a person** — no auto-reject, no auto-fire.
- [ ] **You classified the risk** — screening and worker management are high-risk under the AI Act.
- [ ] **You told workers and their representatives before switching on** any high-risk AI that affects them (Art. 26(7)).
- [ ] **You test for bias** across gender, age, and background, and review the rejected pile.
- [ ] **You never use emotion recognition** on workers — it is prohibited.
- [ ] **The tool explains its matches** so a reviewer can see the logic.
- [ ] **Onboarding keeps a human welcome** — the bot answers, a person welcomes.
- [ ] **AI-generated training is reviewed by a human expert** before it goes out.
- [ ] **Turnover predictions start a conversation**, not a punishment.
- [ ] **HR data is kept secure** and follows privacy rules (see [Chapter 10](ch10-privacy-and-gdpr.md)).
- [ ] **You use data to improve conditions for the group**, not to surveil individuals.
- [ ] **You fix the HR process before automating it.**
- [ ] **You treat compliance as the floor** and your own fairness as the standard above it.

If a box is empty, a person may feel it — and the law may reach it. Fill every box before you let AI near your people.

## Key Takeaways

- AI in HR takes the repetitive work — reading CVs, answering onboarding questions, sorting training, surfacing turnover patterns — and leaves the deciding, the caring, and the acting to humans.
- Hiring and worker management are high-risk uses under the EU AI Act: a person must decide, you must guard against bias, and you must inform workers and their representatives before switching on any high-risk AI that affects them.
- Emotion recognition in the workplace is banned; never buy or use a tool that scores staff by reading their feelings.
- Use HR data to make the workplace better for the group, never to surveil or punish individuals, and keep the human welcome in onboarding.
- Measure the baseline, keep a human in every people decision, and treat the law as the floor and fairness as the standard above it.

<!-- BEGIN agentbridge-examples -->

## Try it with AgentBridge

Here is how the same job looks with AgentBridge. Each box shows the finished result and the one line you type to get it.

### A simple staff handbook

![A friendly staff handbook, ready to share](../../assets/examples/employee-handbook.png)
*A friendly staff handbook, ready to share*

**What you ask:** `Write a short employee handbook covering working hours, holidays, remote work rules and who to ask for help.`

The agent writes a clear, friendly handbook in plain language, with each topic on its own page. Update it any time by asking — 'add a line about the new parking rule'.

*Tip: Keep it in your documents area so the agent can answer questions from it later.*

---

### A weekly timesheet

![A weekly timesheet with totals per person](../../assets/examples/timesheet.png)
*A weekly timesheet with totals per person*

**What you ask:** `Create a weekly timesheet with people, projects, hours per day and a total per person.`

The agent builds the timesheet grid with daily columns and automatic totals. Fill it in or attach your rough hours and let it sort them.

*Tip: Multiply hours by each rate and you have a billing sheet too — just ask.*

---

### Train your team fast

![A step-by-step training slide](../../assets/examples/training-deck.png)
*A step-by-step training slide*

**What you ask:** `Make a training deck on how to handle a customer refund, step by step.`

The agent turns the process into clear slides, one step each, easy to follow. Use it for onboarding and refreshers.

*Tip: Add a final slide with 'who to ask' so people know where to get help.*

<!-- END agentbridge-examples -->
