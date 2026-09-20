# Chapter 5 — Rules and Legal Responsibility: The EU AI Act

## In Simple Words

Every new tool brings rules. Cars brought traffic laws. Banks brought money-handling rules. AI is now getting its own rulebook, and if you do business in or with Europe, that rulebook is the **EU AI Act**.

This chapter is the plain-English guide to it. No legal training needed. The goal is simple: you should be able to tell whether a tool you want to use is lightly regulated, heavily regulated, or banned outright, and what you must do about it.

Two ideas explain most of the law.

The first is **risk**. The AI Act does not treat all AI the same. It sorts AI systems into levels by how much harm they could cause. A spam filter is barely touched. A system that decides who gets a loan or a job is watched closely. A handful of practices are simply forbidden. The higher the risk, the more you must do.

The second is **your role**. The law separates a **provider** (who builds or brands an AI system and puts it on the market) from a **deployer** (who uses it). Most small and medium businesses are deployers. Your duties differ from the vendor's, but they are real, and they are yours.

A note on scope. The EU AI Act is European law. If you are outside the EU but your AI affects people in the EU, parts of it can still reach you. Check with a professional if you serve European customers.

### 5.1 GDPR in plain words: what you must know

**GDPR** (the General Data Protection Regulation) is the European law on personal data. It has applied since 2018 and it still governs anything you do with information about identified people — including the data you feed into AI.

In one paragraph: if you collect, store, or process personal data of people in the EU, you need a lawful reason to do it, you must tell people what you use their data for, keep it secure, hold only what you need, let people access or delete it on request, and not keep it longer than necessary. Breaches can bring large fines. AI does not change these duties; it just gives you more ways to break them, because models need data and data is personal. The full, detailed treatment of GDPR — lawful bases, data-subject rights, and how to comply — is the home of [Chapter 10](ch10-privacy-and-gdpr.md). Read that chapter before you process any customer data with AI. The point here is only that the AI Act and GDPR apply together, on top of each other, not instead of each other.

### 5.2 Personal data vs sensitive data: the difference that matters

GDPR draws a line that matters a lot for AI, because the higher category carries stricter rules.

**Personal data** is any information about a living person who can be identified, directly or indirectly. A name, an email, a phone number, a location, an online ID. Even a combination of ordinary facts that points to one person counts.

**Sensitive data** (the law calls it "special categories") is a smaller set of more delicate facts: racial or ethnic origin, political opinions, religious or philosophical beliefs, trade-union membership, genetic data, biometric data used to identify someone, health data, and data about a person's sex life or sexual orientation.

Why the line matters for you: processing sensitive data needs a stronger legal ground and more protection. It is also the data most likely to cause discrimination if it shapes an AI decision. Many of the AI Act's strictest rules exist because AI can turn ordinary data into sensitive inferences, or use sensitive data to sort people. For the full definitions and handling rules, see [Chapter 10](ch10-privacy-and-gdpr.md).

## A Bit of History

Europe wrote its privacy rulebook first and its AI rulebook second, and the order explains both.

**GDPR** was adopted in 2016 and became directly enforceable in May 2018. It was the most comprehensive data-privacy law of its time, and because so many global companies deal with Europeans, it set a worldwide standard. Its core idea — that people own their personal data and you need a lawful reason to use it — became the template for privacy laws elsewhere.

For AI, Europe took a principles-first path. In 2018 the European Commission created a High-Level Expert Group on AI, which in 2019 published voluntary ethics guidelines built around "trustworthy AI." The Commission then turned principles into law, proposing the AI Act in April 2021. After years of negotiation, it was published in the Official Journal of the European Union on **12 July 2024** and entered into force on **1 August 2024**. It is the world's first comprehensive, horizontal law on artificial intelligence — "horizontal" meaning it covers AI across all sectors, not one industry at a time.

The law does not start all at once. It switches on in stages, giving businesses time to prepare. That staged calendar is the single most practical thing in this chapter, and it appears in section 5.3. The history shows the direction: from soft ethics guidelines to hard, dated obligations. The debate is over. The clock is running.

## Curiosity

### The first AI law in the world — and fines that beat GDPR

Here is a fact worth knowing before any conversation about "compliance is too expensive."

The EU AI Act is the first comprehensive law on AI anywhere. No other major economy has one that matches its breadth. That makes it a test case, and it also gives it a kind of gravity: companies worldwide often build to the strictest rule they might face, so a European rule can quietly become a global default. People call this the "Brussels effect."

The other striking fact is the size of the penalties. GDPR's top fine is up to 4% of a company's total worldwide annual turnover. The AI Act goes higher for the worst violations. For the prohibited practices in section 5.5, fines can reach **up to €35 million or 7% of total worldwide annual turnover, whichever is higher.** For most other breaches of the Act, the ceiling is around €15 million or 3%. For giving inaccurate information to the authorities, around €7.5 million or 1%. (For small and medium enterprises the law caps fines at the lower of the two figures, so the burden is scaled down — but it is still real.)

The lesson is blunt. The practice the law fears most — the banned uses — carries the heaviest fine in European digital regulation, heavier than GDPR. That tells you exactly where the line is, and it tells you that "we didn't know" is not a cheap excuse.

## A Real Business Example

### A small lender that scores credit with AI

This example is illustrative. It is a realistic scenario, not a reported company result, built to show how the tiers work in practice.

Imagine a small consumer-lending firm that wants to use an AI model to decide whether to approve a personal loan.

Step one is to find the tier. The AI Act lists categories of high-risk AI in an annex. One category covers **essential private and public services**, and it explicitly includes **creditworthiness evaluation** — deciding whether a person gets credit. So this lending model is **high-risk**. It is not banned, but it sits in the most heavily regulated working tier.

What that means for the firm, in plain terms:

- It must run a **risk-management system** across the whole life of the model, not just once.
- It must govern its **data**: the data used to train and test the model must be relevant, representative, and as error-free as possible for the purpose. A model trained mostly on one kind of borrower will treat others unfairly.
- It must keep **technical documentation** and **automatic logs** of the system's operation.
- It must design for **human oversight**: a person must be able to review and override a decision.
- It must ensure **accuracy, robustness, and cybersecurity**.
- Before placing it on the market for use, it must complete a **conformity assessment**, draw up an **EU Declaration of Conformity**, attach a **CE marking**, and **register the system in the EU database** for high-risk AI.

Now change one detail and the tier changes. Suppose the firm instead uses AI only to draft friendly reminder emails about existing loans, with no decision about approval. That is not a high-risk function. It falls into a light tier, where the main duty is transparency: people should know automated means are involved where required.

Same company, same technology vendor, two very different legal burdens — because the *use* determines the tier, not the tool. That is the whole logic of the Act in one scene.

## How to Do It

### 5.3 The EU AI Act: what changes for companies

The Act sorts AI into four risk levels, plus a separate track for the big general-purpose models behind chatbots.

**Tier 1 — Unacceptable (prohibited).** A small set of practices is banned outright. See section 5.5. If your use falls here, you cannot do it at all.

**Tier 2 — High-risk.** Systems that can seriously harm health, safety, or fundamental rights. These carry the full compliance regime: risk management, data governance, documentation, logging, transparency to users, human oversight, accuracy and security, conformity assessment, CE marking, and registration. The high-risk uses are listed in two annexes: Annex I (AI as a safety component in regulated products) and Annex III (listed sensitive uses).

**Tier 3 — Limited / transparency risk.** Systems that are not high-risk but that interact with people or generate content. The main duty is disclosure: tell people they are dealing with AI, and label synthetic content. See section 5.6.

**Tier 4 — Minimal risk.** Everything else — spam filters, inventory forecasting, most internal productivity tools. No new obligations beyond existing law.

The **Annex III high-risk categories** are the ones a business owner is most likely to meet. They include: biometrics (where not banned); safety components of critical infrastructure; education and training (admissions, evaluation of learning); **employment and worker management** (recruiting, filtering applications, promotion, termination, task allocation, performance monitoring); **essential services** (eligibility for benefits, creditworthiness, emergency-call triage, insurance risk and pricing); law enforcement; migration and border control; and administration of justice and democratic processes.

A useful exception: an Annex III system is **not** high-risk if it only does a narrow procedural task, improves something a human already did, detects patterns without replacing human assessment, or does a purely preparatory step. But it is **always high-risk if it profiles a person.** Profiling means using data to evaluate or predict aspects about an individual.

**Your role decides your duties.** A provider carries the heavy build-side obligations. A deployer (most businesses) carries use-side duties: use the system as instructed, ensure human oversight, monitor, keep certain logs, and in some cases run a fundamental-rights check. If you only *use* a vendor's high-risk tool, you do not do the conformity assessment — the provider does — but you still must deploy it correctly and responsibly.

**The staged timeline.** Memorize these dates if you touch AI in Europe:

| Date | What applies |
|---|---|
| 1 Aug 2024 | Act enters into force |
| 2 Feb 2025 | Prohibited practices (Art. 5) and AI-literacy duty (Art. 4) apply |
| 2 Aug 2025 | Rules for general-purpose AI models, governance bodies, and penalties framework |
| 2 Aug 2026 | High-risk obligations for Annex III uses (employment, credit, education, essential services, etc.) |
| 2 Aug 2027 | High-risk obligations for Annex I products (AI safety components in regulated products) |

The EU has proposed some simplifications since, sometimes called a "digital omnibus," and dates or details can shift. Treat the table as the working baseline and confirm current dates against the official text before you rely on a deadline.

### 5.4 Obligations for high-risk systems: conformity assessment and technical documentation

If your use is high-risk, these are the concrete things required. You do not need to perform all of them yourself as a deployer, but you must understand them to choose a vendor and to deploy correctly.

**Risk management.** A continuous process, across the system's whole life, that finds, assesses, and reduces risks to health, safety, and fundamental rights. Not a one-time form.

**Data governance.** The training, validation, and testing data must be relevant, representative, and as free of errors and complete as the purpose allows. This is where bias is caught or missed.

**Technical documentation.** A written record showing the system complies and letting authorities check it. It covers how the system works, what it was trained on, how it was tested, and how to use it. Keep it, along with any assessment decisions and approved changes.

**Record-keeping (logging).** The system should automatically record events relevant to risks and to changes, so its behavior can be reviewed later. Logs are your evidence.

**Transparency to deployers.** Clear instructions for use so the people operating the system can comply with their own duties.

**Human oversight.** The system must be designed so a human can understand it, monitor it, interpret its output, and step in or stop it.

**Accuracy, robustness, cybersecurity.** The system must hit appropriate levels of all three and be resilient to error and attack.

**Quality management and accessibility.** A system to keep compliance going over time, and accessibility requirements met.

**Conformity assessment, CE marking, registration.** Before a high-risk system is placed on the market, the provider runs a **conformity assessment** (an independent check by a "notified body" where the law requires it). On passing, the provider draws up an **EU Declaration of Conformity**, attaches a **CE marking**, and **registers the system in the EU database**. As a deployer, you should ask to see these before you buy. If a vendor cannot show a conformity path for a high-risk use, that is a serious red flag.

### 5.5 Prohibited practices: what you absolutely cannot do with AI

These are banned across the EU since 2 February 2025. If a use case matches, drop it. The fines here are the heaviest in the law.

1. **Subliminal or manipulative techniques** that go beyond a person's awareness and materially distort their behavior in a way that causes, or is likely to cause, significant harm.
2. **Exploiting vulnerabilities** of people because of age, disability, or social or economic situation, to distort their behavior and cause significant harm.
3. **Social scoring** by public authorities — systematically scoring people on social behavior or personal traits in ways that lead to harmful treatment unrelated to the context, or disproportionate to the behavior.
4. **Untargeted scraping of facial images** from the internet or CCTV to build facial-recognition databases.
5. **Emotion recognition in the workplace and in education** — inferring the emotions of workers or students, except for medical or safety reasons. (A tool that "reads" a call-center agent's mood to score them is squarely in this ban.)
6. **Biometric categorisation that infers sensitive attributes** — using biometric data to guess race, political opinions, trade-union membership, religious or philosophical beliefs, sex life, or sexual orientation.
7. **Real-time remote biometric identification in public spaces for law enforcement**, banned except for a few narrow, authorized situations such as searching for missing persons or preventing a specific imminent serious threat.

Most small businesses will never touch these. But two catch people by surprise: **emotion recognition at work** and **manipulative design that exploits vulnerability**. If a vendor pitches "AI that detects customer or employee emotions," know that in a workplace or school setting it is prohibited.

### 5.6 Transparency obligations: when you must inform customers and employees

For systems that are not high-risk but that interact with people or create content, the main duty is to be open. These transparency rules apply from 2 August 2026.

**Tell people they are talking to AI.** If an AI system interacts directly with a person — a chatbot, for example — that person must be made aware they are dealing with an AI, unless it is obvious. A customer-service bot should say so.

**Label synthetic and deepfake content.** AI-generated or manipulated audio, images, video, or text must be marked as artificially generated or manipulated. This targets deepfakes and machine-made media.

**Disclose emotion recognition and biometric categorisation.** Where such systems are lawfully used (outside the banned workplace and education cases), the people exposed to them must be informed.

A small grace note: systems already placed on the market before 2 August 2026 have a short window into late 2026 to meet the synthetic-content labeling rule. Plan to comply regardless.

For a business, the practical move is simple and cheap: put a clear notice in your chatbot ("You're chatting with an automated assistant"), label any AI-generated media you publish, and never run hidden emotion or biometric analysis on people.

### 5.7 Documenting important decisions

Across every tier, one habit protects you: **write down your decisions and your reasoning.**

Good documentation is not bureaucracy. It is your memory and your defense. When a regulator, a customer, or a court asks why you used a system a certain way, the written record is your answer.

For each AI system, keep a simple file that records:

- **What it does and who owns it.** The use case, the tier you placed it in, and the named owner.
- **Why you chose it.** The business reason and the alternatives you considered.
- **How you assessed risk.** The ethical and legal risk review, including any bias check and any fundamental-rights check.
- **What controls you put in place.** Human oversight, logging, transparency notices, data limits.
- **What you tested and when.** Test results, dates, and who reviewed them.
- **Changes over time.** Any modification to the system or its use, with the reason and the date.
- **Incidents and fixes.** Anything that went wrong and what you did about it.

This file connects directly to the ethics work in [Chapter 4](ch04-ethical-ai-doing-the-right-thing.md). The risk assessment you do there becomes part of your legal record here. One document, two purposes.

A rule of thumb: **if it mattered and you did not write it down, be prepared for it to be questioned and for you to have no answer.**

## Ethics and Responsibility

Compliance is the floor, not the ceiling. Meeting the letter of the AI Act does not make a use ethical, and it does not remove your responsibility. The law tells you what you must not do and what high-risk uses require. It does not tell you whether a use is fair or wise. That is your judgement, covered in [Chapter 4](ch04-ethical-ai-doing-the-right-thing.md). A system can be fully compliant and still harm trust if you deploy it carelessly.

Your role shapes your duty. As a **deployer**, you are responsible for using a system as instructed, keeping a human in control where required, monitoring how it behaves, and being honest with the people it touches. You cannot point at the vendor and walk away. A practical stance: **treat every legal requirement as the minimum, and let your own ethics set the standard above it.** When you can show you did more than the minimum, you gain credibility — and for a small business, credibility is worth more than any single automation.

## Mistakes to Avoid

**Mistake 1: Assuming your tool is "just a chatbot" and unregulated.** The tier depends on what it decides, not what it is called. A chatbot that influences credit or hiring is high-risk.

**Mistake 2: Not knowing your role.** Provider and deployer have different duties. If you only use a vendor's high-risk tool, you still have deployer duties. Know which you are.

**Mistake 3: Missing the staged dates.** The prohibitions and the AI-literacy duty are already live (February 2025). High-risk duties arrive in 2026 and 2027. Do not treat the whole law as "later."

**Mistake 4: Buying a high-risk tool with no conformity path.** If a vendor cannot show a conformity assessment, a Declaration of Conformity, and registration for a high-risk use, do not buy it.

**Mistake 5: Running emotion recognition at work.** It is prohibited in workplaces and schools. A vendor pitch for "mood detection" on staff is a trap.

**Mistake 6: Forgetting the AI-literacy duty.** Article 4 is law now. You must take reasonable steps to train the people who use your AI.

**Mistake 7: Confusing GDPR with the AI Act.** They are separate laws that stack. Complying with one does not cover the other. Read [Chapter 10](ch10-privacy-and-gdpr.md) for the privacy side.

**Mistake 8: Not documenting.** No written record means no defense when you are asked to explain a decision.

**Mistake 9: Treating compliance as the finish line.** The law is the floor. Ethics and trust sit above it, and you still own them.

## Practical Exercise

### 5.8 Your compliance checklist

Take one AI system you use or plan to use and classify it. This takes about an hour and tells you which rules bind you.

**Step 1 — Is it prohibited?** Read the seven banned practices in section 5.5. If your use matches any, stop. Do not proceed.

**Step 2 — Is it high-risk?** Check the Annex III categories: biometrics, critical infrastructure, education, **employment and worker management**, **essential services (credit, benefits, insurance)**, law enforcement, migration, justice. Does your use fit one? If yes, it is high-risk unless the narrow exception applies — and it is always high-risk if it profiles a person.

**Step 3 — Is it a transparency case?** Does it interact with people or generate content? If yes, you must disclose AI use and label synthetic content.

**Step 4 — Minimal?** If none of the above, you are in the minimal tier. No new AI-Act duties, but existing law and your own ethics still apply.

**Step 5 — What is your role?** Provider or deployer? Write it down. List the duties that follow for that role.

**Step 6 — If high-risk, gather the vendor's proof.** Ask for the conformity assessment, the EU Declaration of Conformity, the CE marking, and the EU database registration. Note what is missing.

**Step 7 — Map your deployer duties.** Human oversight, monitoring, logging, transparency notices, and any fundamental-rights check that applies to you.

**Step 8 — Check the calendar.** Which of your obligations are already live (literacy, prohibitions) and which arrive in 2026 or 2027? Put dates on them.

**Step 9 — Open the file.** Start the documentation file from section 5.7 with your classification and your plan.

If you cannot place a system into a tier with confidence, that is itself the finding: get expert help before deploying.

## Checklist

### 5.9 Your legal policy for AI

- [ ] I know the four risk tiers: prohibited, high-risk, transparency, minimal.
- [ ] I can name the Annex III high-risk categories, especially employment and essential services (credit, insurance).
- [ ] I know that profiling a person makes an Annex III use always high-risk.
- [ ] I know the seven prohibited practices and that emotion recognition at work/school is one.
- [ ] I know my role for each system: provider or deployer.
- [ ] I know the staged dates: prohibitions and AI literacy live since 2 Feb 2025; high-risk Annex III in Aug 2026; Annex I products in Aug 2027.
- [ ] For high-risk tools, I require the vendor's conformity assessment, Declaration of Conformity, CE marking, and EU database registration.
- [ ] I disclose AI interaction to customers and label AI-generated content.
- [ ] I keep human oversight and logging where the tier requires it.
- [ ] I have a plan to meet the AI-literacy duty for staff who use our systems.
- [ ] I understand GDPR applies on top of the AI Act, and I have read [Chapter 10](ch10-privacy-and-gdpr.md).
- [ ] I keep a documentation file for each system: use, tier, owner, risk assessment, controls, tests, changes, incidents.
- [ ] I treat compliance as the floor and my own ethics as the standard above it.
- [ ] I get expert help for any system I cannot confidently classify.

## Key Takeaways

- The EU AI Act sorts AI by risk — prohibited, high-risk, transparency, minimal — and the higher the risk, the more you must do.
- Employment and essential services like credit and insurance are high-risk; profiling a person always makes an Annex III use high-risk.
- Seven practices are banned outright, including emotion recognition in workplaces and schools, and they carry the heaviest fines in European digital law.
- The law switched on in stages: prohibitions and the AI-literacy duty are already live, and high-risk duties arrive in 2026 and 2027.
- As a deployer you still carry real duties — oversight, transparency, literacy, and documentation — and compliance is the floor, not the end of your responsibility.
