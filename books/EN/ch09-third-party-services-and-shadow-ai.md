# Chapter 9 — Third-Party Services and Shadow AI

## In Simple Words

A third-party AI service is any AI you use that runs on someone else's computers. You type a question or upload a file. It travels over the internet to their machines. Their software does the work. The answer comes back. You never see the inside.

This is the normal way most companies use AI today. It is easy, it is cheap to start, and it is powerful. That is why almost everyone uses it.

It also has a hidden cost. The moment your text leaves your building, you lose direct control over it. You are now relying on a company you did not design, on rules you did not write, on a server you cannot inspect.

"Shadow AI" is the second half of this story. Shadow AI means employees using AI tools without the company's knowledge, approval, or oversight. A marketing assistant pastes a customer list into a free chatbot. An accountant drops an invoice into a web app to summarise it. Nobody in charge knows it is happening. The data is gone, and there is no record, no contract, and no control.

Think of it like the office printer twenty years ago. Everyone used it. Nobody knew it kept a copy of every page. Shadow AI is the same surprise, but the pages are your customer lists, your contracts, and your prices.

This chapter is about two things: what actually happens to your data when you use a third-party service, and how to stop your own staff from quietly creating risk. The opposite pattern — running AI on your own machines — is covered in [Chapter 8](ch08-self-hosting-keep-your-data-under-control.md). The legal side of personal data is the home topic of [Chapter 10](ch10-privacy-and-gdpr.md). The wider question of controlling your own tools is [Chapter 11](ch11-digital-sovereignty.md).

## A Bit of History

**1990s to 2000s: software moves off the shelf.** You used to buy a program on a CD and run it on your own computer. Then email, calendars, and file storage moved to the internet. You stopped owning the software and started renting access to it.

**2000s to 2015: SaaS becomes normal.** "Software as a Service" meant paying a monthly fee to use someone else's software over the web. Salesforce, Google Workspace, and Microsoft 365 made it ordinary. Convenience won. Most small businesses stopped running their own servers.

**2016 to 2022: the data goes with the software.** Once your customer records, documents, and messages lived in a vendor's cloud, your business data was permanently outside your walls. Most people accepted this because the tools were good and the price was low.

**November 2022: ChatGPT opens the door to everyone.** A powerful AI became available in a free web box. You no longer needed a vendor contract to use AI. You needed only an email address. This is the moment shadow AI began, because a single employee could now send company data to a frontier model without asking anyone.

**2023: the first corporate alarms.** Companies discovered staff were pasting confidential material into public chatbots. The Samsung case in the Curiosity section is the most famous. Several banks and professional firms banned or restricted public AI tools that year.

**2023 to 2026: vendors add "enterprise" tiers.** In response, AI providers sold business plans that promised not to train on your data, to keep data separate, and to add admin controls. The convenience stayed; the promises got better. But a promise is not the same as control, which is why this chapter matters.

## Curiosity

### 9.7 The semiconductor company that pasted its secrets into ChatGPT

In early 2023, Samsung Electronics — one of the largest technology companies on earth — found that its own engineers had put confidential material into a public AI chatbot.

The reporting, first published by the Korean financial daily *Korea Economic Daily* in April 2023 and repeated widely, described three separate incidents inside the semiconductor division. In the first, an engineer pasted faulty source code from a program used to download measurement data from a chip factory, hoping the chatbot would find the bug. In the second, staff uploaded code connected to semiconductor equipment and defect detection. In the third, employees fed recorded meeting transcripts into the tool to get summaries. All of this happened within roughly three weeks of the division first allowing access to the tool.

Once the data was inside the chatbot, it was on machines Samsung did not own. The company could not easily retrieve it, and could not be sure it would not be used or seen by others.

Samsung's response was blunt. It banned generative AI tools, including ChatGPT, on company-owned computers, tablets, phones, and its internal network. Breaking the rule could lead to disciplinary action up to dismissal. Employees using such tools on personal devices were told never to submit company information or personal data that could reveal Samsung's intellectual property. An internal survey found that 65% of respondents believed AI services posed a security risk. At the same time, Samsung said it was building its own internal AI tools for translation, document summarisation, and software development, and working on ways to block uploads of sensitive information to outside services.

The lesson is not that Samsung was careless. It is that if a company with billions in security budget was caught off guard by a free chatbot, a small business with no security team has even less protection. The convenience is real, and so is the leak.

## A Real Business Example

### The agency that lost its client list twice

Consider a small marketing agency, twenty people, no IT department. This is a composite story, but each part happens every week in real firms.

First leak: a senior account manager wants to rewrite a proposal quickly. She opens a free AI chatbot on her laptop and pastes the draft, which includes a client's unreleased product name, budget figures, and contact details. She gets a nicer paragraph. She never thinks about where the text went.

Second leak: the same manager, a month later, signs up for a paid "AI writing assistant" that promises better results. To set it up, she connects it to the agency's email and shared drive so it can "learn the company voice." Now the vendor can read everything: every client, every contract, every internal joke that turns into a strategy note.

Then the evolution problem arrives. A year later the vendor changes its plan. The features she paid for move to a higher tier. The price doubles. The model behind the tool is swapped for a newer one, and the writing style she trained her team on quietly changes. She wants to leave, but everything is wired into that tool. Switching means reconnecting the whole agency somewhere else and retraining everyone. That is lock-in, and it happened without a single bad decision — only a series of convenient ones.

None of this required malice. It required convenience and the absence of a rule. The fix is not to fear AI. It is to decide, in advance, what data may go where, and to give people a good tool so they do not reach for a risky one.

## How to Do It

### 9.1 The convenience of cloud services: why everyone uses them

Third-party AI is popular for honest reasons, and you should name them before you argue against them.

There is no setup. You do not buy hardware, hire an engineer, or install anything. You open a web page and start. For a small business with no technical staff, that is the whole appeal.

There is no up-front cost. Most tools have a free tier or a low monthly fee. You can try an idea for the price of a coffee instead of a capital purchase.

The quality is high. The best models in the world sit behind these services. A two-person firm can use the same capability as a large corporation.

It scales instantly. Need ten times more work done today? The vendor's machines absorb it. You do nothing.

This is why cloud AI spread faster than any technology before it. The point of this chapter is not to take that away from you. It is to make you use it with your eyes open, because every one of those conveniences is bought with a piece of control you did not notice you were selling.

### 9.2 What happens to your data when it leaves the company

When you paste text into a third-party AI, several things may happen, and you usually cannot see which.

Your data crosses the internet to the vendor's servers, often in another country. Once there, it is stored, at least for a while, on hardware you do not control and cannot inspect.

It may be read by automated systems for safety screening. It may be logged for debugging. Support staff in another country may be able to see it. None of this is unusual; it is how large services operate.

Most importantly, it may be used to train the vendor's model. "Training" means the company feeds your text into its system so the model learns from it. If that happens, a fragment of your confidential text can shape answers given to other customers. This is the single biggest reason to be careful.

Some business plans promise not to train on your data. That promise is worth something, but it is a contract term, not a wall. You are trusting the vendor to honour it across every product and every country. The safe rule is simple: treat any third-party AI as if whatever you send could become public. If that thought is unacceptable for a given file, do not send that file.

### 9.3 The transparency problem: you never really know how your data is used

You cannot see inside a third-party AI service. This is the core problem, and it is not going away.

You do not know which model answered you. Vendors swap models without telling you. You do not know where your data was stored, who could access it, or how long it was kept. You do not know whether a subcontractor in another country processed it. You do not know if it was used for training, even when you think it was not.

The vendor's privacy policy is written by lawyers, not engineers, and it describes what they may do, not what they will do in your specific case. Reading it rarely gives a clear answer.

This is why the practical test is so useful. Instead of trying to understand the system, ask one question about the data: *would I be acceptable if this became public tomorrow?* For a public blog post, yes. For a client's salary file, no. That single test replaces a thousand questions you cannot answer.

If you need real transparency, the only honest source is a system you can inspect — your own machine, or open software someone can audit. That is the subject of [Chapter 8](ch08-self-hosting-keep-your-data-under-control.md) and [Chapter 11](ch11-digital-sovereignty.md).

### 9.4 The evolution problem: models change, contracts change, prices change

A third-party service is not a thing you buy; it is a relationship that keeps changing under your feet.

The model changes. Today's tool may run on a different model next quarter. The answers change. The style changes. Something that worked well in your workflow can get worse, or simply different, with no warning and no way to stay on the old version.

The contract changes. Terms you agreed to at signup can be updated. Features you relied on can move behind a higher plan. The promise about training data can be reworded.

The price changes. A cheap tool that you have now wired into your business can raise its price, and you face a painful choice: pay more, or rip everything out.

This is the hidden risk of convenience. You build on ground that someone else controls, and they can move the ground whenever they like. The defence is to keep your important data and your core workflows portable, and to never let a single vendor become the only place your work can happen.

### 9.5 Lock-in: how hard it is to switch vendors later

Lock-in means leaving a vendor is so costly, in time, money, or disruption, that you cannot realistically do it. You are "locked in."

It happens in three ways. **Data lock-in:** your data is stored in a format only that vendor reads well, or you cannot export it cleanly. **Workflow lock-in:** your daily process is built around that tool, so switching means retraining everyone and rebuilding templates. **Integration lock-in:** the tool is connected to your email, your CRM, your files, and pulling it out breaks all of those links.

Lock-in gives the vendor power over you. They know leaving is hard, which weakens your position when they raise prices or change terms.

To stay free, insist on three things from the start. First, your data must be exportable in a plain, common format. Second, keep your core data somewhere you control, and let the vendor work on a copy. Third, design your workflow so the AI is a step, not the whole machine, so you can swap the step. The goal is not to avoid vendors. It is to be able to leave one in a week, not a year.

### 9.6 Shadow AI: when employees use unauthorized tools

Shadow AI is the risk you cannot see, because it is created by your own trusted staff.

It happens because good official tools are slow to approve, while risky free tools are instant. An employee under time pressure pastes a customer email into a free chatbot to draft a reply. Nobody stops them, because nobody knows.

Why it is dangerous: the data leaves with no contract, no review, and no record. You cannot tell the customer, you cannot find the data later, and you cannot prove what happened. If the tool trains on that data, your confidential information may end up shaping a public model.

How to spot it: unusual charges on corporate cards for AI subscriptions; staff complaining that approved tools are too slow; sudden "magic" improvements in output that no approved tool explains.

How to stop it: do not only ban. A ban with no good alternative just pushes the behaviour underground. Give people an approved tool that is fast and good enough, and they will use it. Then make the rule clear, train on it, and monitor lightly. The full policy side is in section 9.8 and in the company AI-policy templates in the book's appendices.

### 9.8 How to mitigate the risks: due diligence, contracts, internal policy

You reduce the risk with three layers. Do all three.

**Layer 1: Due diligence — check before you buy.**
Before adopting any AI vendor, ask the hard questions. Where is data stored, and in which countries? Do you train on customer data, and can you guarantee in writing that you will not? Who can access it, including subcontractors? How long is it kept, and how is it deleted? Is it encrypted in transit and at rest? What certifications do you hold? Get the answers in writing, not in a sales call. A vendor who cannot answer clearly is telling you something. A scored version of these questions is in the vendor due-diligence scorecard in the appendices.

**Layer 2: Contracts — put the promises on paper.**
A verbal assurance is worthless. In the contract, require: no training on your data; data residency in a country you accept; the right to export all your data in a usable format; the right to deletion; a duty to tell you about breaches and about major model or term changes; and limits on subcontractors. If the vendor will not sign these, that is your answer.

**Layer 3: Internal policy — tell your people the rules.**
Write a short, plain AI policy. State which tools are approved. State what data may never go into any external AI — client personal data, financial records, contracts, source code, passwords. Give staff a fast approved tool so they do not reach for a risky one. Train everyone on the rule in one short session. Review the list of approved tools every quarter. A template lives in the appendices.

The order matters. Check first, contract second, policy third. Most companies skip the first two and wonder why they got exposed.

## Ethics and Responsibility

Third-party AI raises a duty you owe to two groups: the people whose data you hold, and your own staff.

**To your customers and employees.** When a customer gives you personal data, they trust you to protect it. Sending that data to a third-party AI you have not vetted can break that trust, even if nothing bad happens. You are responsible for where their data goes. The legal duties are set out in [Chapter 10](ch10-privacy-and-gdpr.md); the ethical principle is simple — do not put someone's private information somewhere you would not put your own.

**To your staff, about shadow AI.** Be careful not to turn protection into surveillance. If you monitor AI use, tell people what you monitor and why. A clear rule plus a good tool is fair. Secret monitoring of trusted staff damages morale and trust. Aim for guardrails, not a police state.

**Be honest about what you do not control.** If a client asks whether their data trains an external model, you should be able to answer truthfully. If you do not know, say so, and fix it. Overclaiming safety is worse than admitting a gap.

## Mistakes to Avoid

1. **Reading the demo, not the data flow.** A slick demo tells you nothing about where your data goes. Ask the storage and training questions first.
2. **Trusting a verbal "we don't train on your data."** If it is not in the contract, it does not exist.
3. **Connecting a tool to your whole drive.** "Learn our voice" often means "read everything." Give the tool the least it needs.
4. **Banning shadow AI with no alternative.** A ban without a good approved tool just hides the behaviour.
5. **No written policy.** If the rule is not written and trained, it is not a rule.
6. **Ignoring the country question.** Data stored under a different legal system can be accessed differently. Know where it sits.
7. **Assuming a paid plan equals safe.** A paid consumer plan is not the same as a contracted enterprise plan with the right terms.
8. **No export plan.** If you cannot get your data out, you are locked in from day one.
9. **Treating the privacy policy as a guarantee.** It lists what they may do, not what they will do for you.
10. **Forgetting the human.** The leak almost always starts with one person under time pressure. Fix the pressure and give a safe path.

## Practical Exercise

### 9.9 Analyze your current AI vendors

Take one hour and do this for every AI tool your company uses today, including the ones staff quietly use.

Make a table. One row per tool. Columns:

- **Tool name** and who signed up for it.
- **What data goes in.** Be specific: customer emails, invoices, contracts, code, public text.
- **Where it is stored,** if you know. If unknown, write "unknown."
- **Do they train on our data?** Yes / No / Unknown.
- **Is there a contract,** or just a click-through?
- **Can we export our data?** Yes / No / Unknown.
- **Risk level** for the data you actually put in it: Low / Medium / High.

Now read the High-risk rows. For each, ask: would it be acceptable if this data became public? If no, you have three choices — stop putting that data in it, move to a vendor that signs the right terms, or move that task to a tool you control (see [Chapter 8](ch08-self-hosting-keep-your-data-under-control.md)).

Finally, ask around. Send one honest message to your team: "What AI tools do you use for work that we have not talked about?" The answers are your real shadow-AI list. Do not punish the honesty; fix the gaps it reveals.

## Checklist

### 9.10 Questions to ask every AI vendor

Before you put any real data into a third-party AI service, get a written answer to each of these.

- [ ] **Where is our data physically stored,** and in which countries?
- [ ] **Do you train your models on our data?** Can you commit to "no" in the contract?
- [ ] **Who can access our data,** including employees and subcontractors, and from where?
- [ ] **How long do you keep our data,** and how do we get it deleted?
- [ ] **Is our data encrypted** both in transit and while stored?
- [ ] **Can we export all of our data** at any time, in a common, usable format?
- [ ] **Will you notify us** of a data breach, and within what time?
- [ ] **Will you tell us** before you change the model, the price, or the terms?
- [ ] **What security certifications** do you hold, and can you show them?
- [ ] **Are there subcontractors,** and are they bound by the same terms?
- [ ] **What is our legal recourse** if you misuse our data?
- [ ] **Is there an admin console** so we can see and control usage?

If a vendor cannot answer these clearly and in writing, treat the tool as high-risk and keep sensitive data out of it.

## Key Takeaways

- A third-party AI service runs on someone else's computers, so the moment your data leaves, you trade control for convenience.
- The biggest risk is that your confidential data may be used to train a model that serves others, and you often cannot see or stop it.
- Vendors change models, contracts, and prices under your feet, and lock-in makes leaving expensive — so keep your data exportable and your workflow swappable.
- Shadow AI is your own staff using unapproved tools; stop it with a good approved tool plus a clear written rule, not with bans alone.
- Protect yourself in three layers: check the vendor first, put the promises in a contract second, and set an internal policy third.
