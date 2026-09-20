# Chapter 10 — Privacy and GDPR: What You Really Need to Know

## In Simple Words

GDPR stands for General Data Protection Regulation. It is the European Union's rulebook for handling personal data — any information about a living person who can be identified. It is one of the strictest privacy laws in the world, and it affects far more companies than most owners expect.

The whole law can be reduced to one idea: **if you hold information about a person, you must handle it fairly, for a clear reason, keep only what you need, keep it safe, and respect what that person asks you to do with it.**

You are affected if you are in the EU, and also if you are outside the EU but offer goods or services to people in the EU, or watch their behaviour. A small online shop in another country that sells to customers in France is inside GDPR's reach. This is called extraterritorial reach, and it surprises many businesses.

Why does this matter for AI? Because AI runs on data, and much of that data is personal. Customer names, support emails, CVs, employee records, website visitors — all personal data. When you feed any of it into an AI tool, you are processing personal data, and the rules apply. If you send that data to a third-party service, the rules follow it out the door. That is the link to [Chapter 9](ch09-third-party-services-and-shadow-ai.md).

This chapter is the deep home for GDPR in this book. It explains the principles, the types of data, the legal grounds, your obligations, and the rights people hold over you. The EU AI Act — a separate law about AI systems themselves — is treated fully in [Chapter 5](ch05-rules-and-legal-responsibility.md); here we look only at where it touches privacy. The security side of protecting data is in [Chapter 6](ch06-cybersecurity-in-the-ai-era.md).

One honest note: this is a plain guide, not legal advice. For real decisions, especially across borders, talk to a data-protection professional.

## A Bit of History

**1995: the first EU rule.** The Data Protection Directive set early standards across Europe, but each country implemented it differently, creating a patchwork.

**27 April 2016: GDPR adopted.** The EU replaced the patchwork with one regulation, designed to apply the same way in every member state and to modernise the rules for the internet age.

**25 May 2018: GDPR applies.** This is the date that matters. From this day, the rules were fully in force, with heavy fines for serious breaches. Companies across the world had to comply or risk them.

**2018 to 2023: the enforcement era.** National data-protection authorities issued fines, some very large, for breaches and poor practice. Privacy became a board-level topic, not just a lawyer's problem.

**2018: the EDPB.** The European Data Protection Board was created to coordinate the national authorities and issue guidance so the law is applied consistently across the EU. Its guidance is where you look when the law is unclear.

**1 August 2024: the EU AI Act enters into force.** A separate law, Regulation (EU) 2024/1689, began its phased rollout. It regulates AI systems by risk. It does not replace GDPR. Where an AI system uses personal data, both laws apply at once.

## Curiosity

### 10.9 What Europe's privacy regulators said about AI models

In December 2024 the European Data Protection Board (EDPB) — the body that coordinates all the EU's national privacy regulators — adopted **Opinion 28/2024**, on the protection of personal data in the context of AI models. It is the most important privacy statement yet on how AI fits with GDPR.

A few points from it matter to a business owner:

**A model can be looked at in three stages.** The EDPB separates the life of an AI model into development (training it), deployment (putting it to work), and use (people interacting with it). Each stage can involve personal data, and each has its own privacy questions. This is useful because it tells you to ask the question at every stage, not only at the start.

**Legitimate interest can be a legal basis, but it is not a free pass.** The opinion says a company may rely on "legitimate interest" to develop or use an AI model, but only if the processing is genuinely necessary and a balancing test shows it does not outweigh people's rights. You cannot simply declare an interest and ignore the people involved.

**A model is only "anonymous" if you cannot get personal data out of it.** This is the sharp part. The EDPB says that for a model to be treated as anonymous — and so outside GDPR — it must be very unlikely that someone could extract personal data from it by asking it questions. If a model can be tricked into repeating personal details it memorised during training, it is not truly anonymous, and the data protection rules still bite.

**Bad training data can follow the model.** The opinion warns that if a model was trained on unlawfully processed personal data, that can affect the lawfulness of deploying it later, unless the model has been properly anonymised. In plain words: a model built on dirty data can stay dirty, and using it can carry that problem into your business.

The practical message for a small company is clear. When you choose an AI vendor, the privacy question is not only "what do you do with my data now," but "what data was this model trained on, and can personal data be pulled back out of it?" That question belongs in your vendor checklist.

## A Real Business Example

### The HR tool and the access request

A mid-sized firm with 120 staff adopts an AI tool to screen job applications. It uploads CVs and cover letters — all personal data, some of it sensitive, because CVs can reveal health gaps, age, nationality, and union activity. The tool ranks candidates.

Three months later, an applicant who was rejected writes to the firm. She makes a **subject access request**: under GDPR she has the right to know what personal data the firm holds about her and how it was used. The firm must respond, usually within one month and free of charge.

Now the firm must answer hard questions it never asked. Where are her CV and the AI's ranking stored? Can it produce the data and explain the logic? Was there a lawful basis to process her CV with this tool? Did it do a risk assessment first? If the tool was a third-party service, did the contract cover all of this? If the AI's ranking counts as automated decision-making with a serious effect on her, extra rules apply, including her right not to be subject to a purely automated decision with legal or similarly significant impact.

The firm scrambles because it adopted the tool before it thought about the data. The lesson is the order of operations: you must understand the data and the legal basis **before** you switch the tool on, not when a request arrives. The rest of this chapter gives you the pieces to do that.

## How to Do It

### 10.1 GDPR on one page: the basic principles

GDPR rests on a few principles. If you honour these, you are honouring most of the law.

**Lawfulness, fairness, transparency.** You need a valid legal reason to process personal data, you must not use it in ways people would consider unfair, and you must tell people what you are doing.

**Purpose limitation.** Collect data for a clear, stated purpose. Do not reuse it later for something unrelated without a new lawful basis.

**Data minimisation.** Collect only what you actually need. If you do not need a phone number, do not ask for one. This matters for AI: do not dump your whole database into a tool when a small slice would do.

**Accuracy.** Keep data correct and update it. People can demand corrections.

**Storage limitation.** Do not keep personal data longer than you need it. Have a deletion schedule.

**Integrity and confidentiality.** Keep it secure against breaches. The how-to is in [Chapter 6](ch06-cybersecurity-in-the-ai-era.md).

**Accountability.** You must be able to *show* you comply — with records, policies, and documents. This is why the paperwork in the Checklist section is not optional.

### 10.2 Personal data, sensitive data, anonymous data: the differences that matter

**Personal data** is any information about a living person who can be identified, directly or indirectly. A name, an email, a phone number, a photo, an ID number, a location, an online identifier like a cookie ID. Even a combination of details that singles someone out counts. If you can point at a person, it is personal data.

**Sensitive data** (the law calls it "special categories") gets stronger protection. It includes: racial or ethnic origin, political opinions, religious or philosophical beliefs, trade union membership, genetic data, biometric data used to identify a person, health data, and data about a person's sex life or sexual orientation. The rule is that processing these is prohibited unless a specific condition applies, such as explicit consent or a clear legal requirement. In AI, watch for these hiding inside CVs, support tickets, and HR files. A chatbot that learns "this customer is on chemotherapy" has touched health data.

**Anonymous data** is information that can no longer identify a person, even by combining it with other data. Truly anonymous data is outside GDPR, because there is no identifiable person. But true anonymity is hard to achieve. If you could re-identify someone, it is not anonymous. This is the difference that trips people up, and it is the focus of section 10.8.

The practical rule: treat almost everything about a customer, employee, or applicant as personal data by default. Treat anything touching health, beliefs, or identity as sensitive and handle it with extra care. Only call data anonymous if you have genuinely removed the ability to identify anyone.

### 10.3 Consent: when it is needed and when it is not

Consent is one lawful basis for processing, not the only one, and it is often misunderstood.

For consent to be valid, it must be **freely given, specific, informed, and unambiguous**, and given by a clear action. A pre-ticked box is not consent. Buried clauses are not consent. Consent for "marketing and everything else" is not valid consent.

You need consent when no other basis fits, and always for sensitive data in most cases, and for certain things like marketing emails to consumers in many EU countries.

You often do **not** need consent when another basis applies. If you process data to deliver a contract you have with the customer, that is the "contract" basis, not consent. If a law requires you to keep records, that is "legal obligation." Asking for consent when you already have a contract can actually create problems, because consent can be withdrawn at any time, and then you cannot deliver what you promised.

For AI, consent is tricky. If you want to use customer data to train a model, a vague "we may use your data to improve our services" is usually not enough. You must be specific, and you must let people say no without losing the service. The safer path is to avoid needing broad consent at all: minimise the data, use it only where a real basis exists, and prefer non-personal or anonymised inputs for training.

### 10.4 Legitimate interest: when you can use data without explicit consent

Legitimate interest is the most flexible and most misused basis. It lets you process personal data without consent when you have a genuine, lawful business reason — but only after a careful test.

The test has three parts. **Purpose:** is your reason legitimate? Improving fraud detection or network security usually is. **Necessity:** is processing the personal data actually necessary to achieve it, or could you do it with less or with anonymous data? **Balancing:** do your interests outweigh the person's rights and expectations? Would a reasonable person be surprised or harmed?

You must document this balancing test. It is not a feeling; it is a written assessment you can show.

For AI, legitimate interest can cover some uses — for example, using customer support data to improve service quality, if it is necessary and balanced. But it does not let you do anything a customer would find intrusive. Training a model on sensitive data under "legitimate interest" is very hard to justify. And as the EDPB opinion in the Curiosity section says, the necessity and balancing tests must genuinely pass.

The rule of thumb: if you would feel uneasy explaining the use to the person out loud, legitimate interest probably does not cover it.

### 10.5 Data subject rights: access, rectification, erasure, portability

People hold rights over their data, and you must be able to honour them. The main ones:

**Right to be informed.** You must tell people, clearly, what data you collect and why, usually in a privacy notice.

**Right of access.** A person can ask what data you hold about them and how you use it. This is the subject access request from the example. You must provide a copy, usually within one month, free of charge.

**Right to rectification.** If the data is wrong, they can have it corrected.

**Right to erasure ("right to be forgotten").** They can ask you to delete their data, and you must, unless a legal reason to keep it overrides — for example, a tax record you are required to retain.

**Right to restriction of processing.** They can pause how you use the data in certain situations while a dispute is settled.

**Right to data portability.** They can ask for their data in a structured, common, machine-readable format so they can move it elsewhere. This connects to the lock-in problem in [Chapter 9](ch09-third-party-services-and-shadow-ai.md).

**Right to object.** They can object to processing based on legitimate interest, and to direct marketing.

**Rights around automated decisions.** Under Article 22, a person has the right not to be subject to a decision based purely on automated processing that has legal or similarly significant effect on them, with limited exceptions, and the right to human involvement. This is critical for AI that screens people for jobs, credit, or services.

Build a simple, written process to receive and answer these requests on time. When you use a third-party AI, make sure the vendor can help you produce and delete the data, or you cannot honour the request.

### 10.6 The EU AI Act: what changes for privacy

The EU AI Act is a separate law from GDPR, and it is treated in full in [Chapter 5](ch05-rules-and-legal-responsibility.md). Here is only the privacy angle, so the two do not get confused.

Think of it this way. **GDPR governs the personal data that flows through an AI system. The AI Act governs the AI system itself — its risk level, its obligations, and how it may be used.** If your AI system uses personal data, both apply at the same time. They are not alternatives; they stack.

For a high-risk AI system that processes personal data, you end up doing two related jobs. Under the AI Act, you follow a risk and conformity process for the system. Under GDPR, you need a lawful basis for the personal data and, where the risk is high, a Data Protection Impact Assessment. The good news is that the work overlaps: understanding your data, documenting your process, and assessing risk serve both laws.

The AI Act also pushes on data quality for high-risk systems — training and testing data should be relevant and representative, and as free of errors as appropriate. That lines up with GDPR's accuracy principle. And the AI Act's transparency duties — telling people they are interacting with AI — sit alongside GDPR's transparency duties.

The practical point: do not treat the AI Act and GDPR as one checklist. Ask two questions about every AI system. *What is the system's risk under the AI Act?* And *what personal data flows through it, and is that lawful under GDPR?* The first is Chapter 5's job; the second is this chapter's.

### 10.7 Data Protection Impact Assessment (DPIA): when it is mandatory and how to do it

A Data Protection Impact Assessment is a structured review you do **before** starting a processing activity that is likely to be high risk to people. For AI, you will often need one.

You must do a DPIA when processing is high risk. Clear triggers include: systematic and extensive evaluation of people based on automated processing that produces significant effects (this covers AI that scores, ranks, or profiles people); large-scale processing of sensitive data; and large-scale systematic monitoring of publicly accessible areas. New technologies used in new ways also raise the risk.

How to do one, in plain steps:

1. **Describe the processing.** What data, what purpose, how long, who sees it, where it is stored, and whether a third party or AI is involved.
2. **Check necessity and proportionality.** Is this the least intrusive way to reach your goal?
3. **Assess the risks to people.** Not risk to your company — risk to their privacy, fairness, and rights. Think about bias, error, over-collection, and re-identification.
4. **List the measures to reduce those risks.** Minimise data, anonymise where possible, add human review, secure the system, set short retention.
5. **Decide.** If a high risk remains after your measures, you must consult your national data-protection authority before proceeding.
6. **Document and revisit.** Write it down and review it when the system changes.

A DPIA is not a form to tick. It is a thinking exercise that, done honestly, often changes your design for the better.

### 10.8 Anonymization and pseudonymization: what they are and why they matter

These two words sound alike and are very different. Confusing them causes real trouble.

**Pseudonymization** means you replace direct identifiers with a stand-in, like a code, and keep the key that links the code to the person separately and securely. "Customer 4471" instead of "Maria Rossi," with the mapping table locked away. Pseudonymized data is **still personal data** under GDPR, because with the key you can re-identify the person. It is a valuable security measure — it reduces risk if the data is stolen — but it does not take you out of the law.

**Anonymization** means you remove identifying information so thoroughly that no one can re-identify a person, even by combining the data with other sources. The law asks whether re-identification is "reasonably likely," considering cost, time, and current technology. Truly anonymous data is **outside GDPR**, because there is no identifiable person. But true anonymity is genuinely hard. Datasets that look anonymous have been re-identified by cross-referencing other public data.

Why it matters for AI: if you want to train a model on data without GDPR applying, you need real anonymity, not pseudonymization. And as the EDPB opinion warns, even a trained model may not be anonymous if personal data can be extracted from it by clever questioning. So "we anonymised the training data" is a claim you must be able to defend, not just assert.

The safe working rule: treat pseudonymized data as personal data, because it is. Only treat data as anonymous if you have tested that re-identification is not reasonably possible. When in doubt, keep the GDPR protections on.

## Ethics and Responsibility

GDPR is the floor, not the ceiling. Compliance means you avoid fines; ethics means you do the right thing even where the law is silent.

**Respect the person behind the data.** Every record is someone's private life. Ask whether your use would feel fair if you were the one being profiled by an AI.

**Do not hide behind "the model did it."** If an AI makes an unfair decision about a person using your data, you are responsible. Keep a human who owns the outcome, as [Chapter 4](ch04-ethical-ai-doing-the-right-thing.md) sets out.

**Be transparent about AI.** Tell people when an AI touches their data and what it does. Surprises erode trust faster than any technical flaw.

**Minimise as a moral habit.** Collecting less is not just a legal rule; it is respect. Every field you do not collect is a field that cannot be leaked or misused.

**Protect the vulnerable.** Sensitive data about health, beliefs, or finances deserves the highest care. If a tool cannot guarantee it, do not put it in the tool.

## Mistakes to Avoid

1. **"We are too small for GDPR."** Size does not exempt you. If you process personal data of people in the EU, the rules apply.
2. **Thinking consent is always needed, or never needed.** It is one basis among six. Use the right one and document why.
3. **Confusing pseudonymization with anonymity.** Pseudonymized data is still personal data and still in scope.
4. **Dumping your whole database into an AI tool.** That breaks data minimisation and spreads risk.
5. **No lawful basis for training on personal data.** "Improve our services" is usually not enough.
6. **Ignoring sensitive data hiding in CVs and tickets.** Health, beliefs, and union activity can be inside ordinary documents.
7. **No DPIA before a high-risk AI rollout.** Do it before, not after a complaint.
8. **No process for access and deletion requests.** If you cannot find and delete the data, you cannot honour the right.
9. **Losing control of data to a third party.** If the vendor cannot help you delete or export, you are exposed. See [Chapter 9](ch09-third-party-services-and-shadow-ai.md).
10. **Treating the law as a one-time project.** GDPR is ongoing. Retention, breaches, and requests keep coming.

## Practical Exercise

### 10.10 Your GDPR compliance checklist for AI

Take a half-day and work through this for one AI use case that touches personal data.

1. **Map the data.** List exactly what personal data flows into the AI. Name each field. Mark any sensitive category. (A data inventory template is in the appendices.)
2. **Name the lawful basis.** For each use, write which of the six bases applies and why. If you cannot name one, stop and reconsider.
3. **Check for sensitive data.** If any special-category data is present, confirm a specific condition allows it, or remove it.
4. **Apply minimisation.** Cut every field you do not strictly need.
5. **Decide the destination.** Does the data go to a third party? If so, run the vendor questions from [Chapter 9](ch09-third-party-services-and-shadow-ai.md).
6. **Do a DPIA.** If the use is high risk — profiling, large-scale sensitive data, automated decisions — complete the DPIA steps in section 10.7.
7. **Plan the rights.** Write how you will handle access, correction, and deletion requests for this data, including data held by the vendor.
8. **Set retention.** Decide how long you keep the data and when you delete it.
9. **Check automated-decision rules.** If the AI decides about people with significant effect, ensure a human review path exists.
10. **Document everything.** Write the answers down. Accountability means you can show your work.

If any step leaves a blank you cannot fill, that blank is your to-do list.

## Checklist

### 10.11 The documents you must have

For an AI system that touches personal data, keep these documents ready and current.

- [ ] **Privacy notice** that clearly explains what data you collect, why, and how AI is involved.
- [ ] **Record of processing activities** describing each use of personal data.
- [ ] **Lawful basis statement** for each processing purpose, written down.
- [ ] **Data inventory** listing every personal-data field and where it lives.
- [ ] **DPIA** for any high-risk AI processing, with the residual-risk decision.
- [ ] **Balancing test** if you rely on legitimate interest.
- [ ] **Data Processing Agreement** with every vendor that handles your data.
- [ ] **Retention schedule** stating how long each data type is kept and when it is deleted.
- [ ] **Subject-request procedure** for access, rectification, erasure, and portability, with a one-month clock.
- [ ] **Breach response plan** including notifying the authority within 72 hours and affected people when required.
- [ ] **Automated-decision safeguards** with a human review path for significant decisions.
- [ ] **Data Protection Officer contact**, if your processing requires one.

Keep these alive. A document you never update is a document that will fail you when a regulator or a customer asks.

## Key Takeaways

- GDPR applies to any personal data about identifiable people in the EU, including when it flows through an AI tool, and it reaches companies outside the EU that serve EU customers.
- You need a lawful basis for every use; consent is only one of six, and sensitive data needs a specific condition on top.
- People hold real rights — access, correction, erasure, portability — and you must be able to honour them, including for data held by a third-party vendor.
- Pseudonymization is not anonymity; only data that cannot reasonably be re-identified leaves GDPR, and a model that leaks personal data is not anonymous.
- For high-risk AI, do a DPIA before you start, and remember the AI Act and GDPR apply together, not instead of each other.
