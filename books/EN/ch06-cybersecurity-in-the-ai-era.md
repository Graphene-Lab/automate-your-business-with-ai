# Chapter 6 — Cybersecurity in the AI Era

## In Simple Words

For most of the history of business computing, security meant one thing: keep strangers out of your building. You had a locked door, a password, a firewall. The bad person was outside. Your data was inside.

Artificial intelligence has blurred that line. Today, when an employee types a customer list, a contract, or a salary sheet into an online AI tool, that text leaves the building. It travels to computers that belong to someone else. It may be stored there. It may be read by support staff. It may be kept for months. In some cases it may be used to make that company's product better. Most people never think about this, because the tool looks like a search box. It is not a search box. It is a service, run by a company, on machines you do not control.

AI changes the security picture in two directions at the same time.

**The attackers got better.** A language model gives a criminal three things that used to be expensive: speed, scale, and polish. A phishing email that once looked like a bad translation can now be written in fluent business German or Japanese in seconds, personalised with details from a public profile. A voice can be copied from a few seconds of a recording, which is how finance clerks in reported fraud cases approved transfers because the caller sounded like their own boss. None of this requires a genius. It requires a subscription.

**Your attack surface got bigger.** "Attack surface" is just a term for the number of places someone can get in. Every AI feature you add is a new door: chat tools, plugins that reach your email, agents that read folders and send messages, models trained on your records, vendors that keep a copy of every prompt and every answer. Two years ago your company had one front door. It may now have forty, and most of them were opened by your own staff without telling anyone.

One more idea organises everything else. Security protects three things, known by three short words.

- **Confidentiality.** Only the right people see the data.
- **Integrity.** The data has not been secretly changed.
- **Availability.** The system works when you need it.

Most owners treat AI security as only a confidentiality problem. It is not. A competitor poisoning your model is an integrity problem. A vendor whose systems go down and stop your payments for weeks is an availability problem, and that one caused the most damage in the story later in this chapter. When you look at any AI tool, ask all three questions.

One warning. The thought "we are too small to be attacked" is not true. Modern attacks are automated: software scans the whole internet for unlocked doors, the way a thief tries every car in a car park. You are not chosen because you are interesting. You are hit because you were easy, and because you hold customer details, bank details, and tax records with very little protection around them.

The good news is that most of the protection you need is not high technology. It is a short list of boring habits, a map of where your data goes, and a few controls in the right place.

The legal side of personal data is in [Chapter 10](ch10-privacy-and-gdpr.md). Staff using AI tools without approval — "shadow AI" — is in [Chapter 9](ch09-third-party-services-and-shadow-ai.md). The step-by-step build is in [Chapter 20](ch20-implementing-ai-securely.md).

## A Bit of History

Security history repeats one lesson: the perimeter moves, and the defenders are slow to notice.

In **1988** the Morris worm disabled something like ten percent of the early internet's connected computers. It was written by a graduate student, not a criminal, and it proved that a self-spreading program could cross the planet in hours. Through the **1990s and 2000s** the standard answer was the perimeter model: a firewall at the edge, antivirus on each PC, data on a server in a cupboard. It worked as long as the data stayed where you put it.

In **2013** the US retailer Target was breached. The attackers did not break into Target. They broke into a small company that supplied heating and cooling equipment for its stores, took that company's login details, and used them to reach Target's payment systems. Around 40 million card numbers were stolen. The lesson was about connection, not code: your risk now includes everyone you plug into.

In **2016** Microsoft put a chatbot called Tay on social media. Within a day, users taught it to post offensive material by feeding it repeated messages, and it was taken down. Nobody broke the program. They broke what the model was reading. That is the seed of prompt injection, although it had no name yet.

In **2017** NotPetya malware spread from Ukrainian accounting software and caused damage measured in the tens of billions of dollars worldwide, hitting shipping giant Maersk, pharmaceutical maker Merck, and many others. One poisoned link in a software supply chain became everyone's problem at once.

In **2020** remote work removed the physical perimeter almost overnight. In **2022** ChatGPT made generative AI a normal office tool within weeks, and staff began pasting real work into tools with no company contract behind them. In **September 2022** the security researcher Simon Willison published a post titled "Prompt injection attacks against GPT-3" and gave a name to a problem people had been seeing but could not describe: instructions hidden inside text that a model reads, which override the instructions you gave it.

In **2023** open-weight models meant a company could run AI on its own hardware, as [Chapter 8](ch08-self-hosting-keep-your-data-under-control.md) explains. The same year, vendors began shipping "agents" that can act rather than only answer, which raised the cost of every mistake. In **2024** vendor risk became impossible to ignore, as told in the Curiosity section below. From **2025** onward, agents arrived with tools and credentials attached, so the blast radius of one wrong permission is now everything that agent can reach.

Read the timeline as one long argument. Each step moved trust away from a locked door and into a relationship: a contractor, a vendor, a plugin, a model, an agent. Security stopped being a wall and became a question about who, and what, you have connected to.

## Curiosity

### 6.8 The vendor that nearly stopped a healthcare system

On 12 February 2024, attackers got into Change Healthcare, a company that processes medical bills and payments in the United States. According to testimony that UnitedHealth Group's chief executive gave to the US Congress in May 2024, they entered through a remote-access portal that did not require multi-factor authentication — the second check on a login that stops most stolen passwords from working. There was no clever malware at the front door. There was a stolen password and a missing second lock. The attackers spent nine days inside, moving quietly and copying out around six terabytes of data. On 21 February they switched on ransomware and locked systems.

Change Healthcare is a subsidiary of UnitedHealth Group, and it sits in the middle of the American healthcare payment chain. When it stopped, a very large share of doctor claims, pharmacy payments, and insurance authorisations stopped with it. Small clinics could not get paid and ran out of cash within weeks; industry groups reported provider losses running to tens of millions of dollars a day across the affected network. Big names that had nothing to do with the breach — chain pharmacies, regional insurers, a naval hospital — found their own operations blocked, because they all passed data through the same middleman.

UnitedHealth later advanced more than $2 billion in emergency loans to affected providers by mid-March, and more than $6 billion by mid-April. Reporting by Reuters and Wired said a ransom of roughly $22 million in bitcoin was paid to a wallet linked to the criminal group ALPHV, also known as BlackCat, which UnitedHealth confirmed on 29 February as the attacker. In October 2024 UnitedHealth estimated that about 190 million individuals had their data affected, one of the largest breaches ever recorded.

Why does this matter to a small business that will never touch a medical claim? Because of who the real victim was. The hospitals and pharmacies that suffered did not get hacked. Many of them had good security. They were hurt because a company in the middle of their workflow got hacked, and they could not survive without that company. Their security was only as good as the least-protected vendor in their chain.

Now add the analytics angle, because it is closer to home than it looks. In 2024, OpenAI disclosed an incident that was not a breach of its own systems at all. The problem was in Mixpanel, a third-party analytics service used on the developer site for its application programming interface. Analytics services are small pieces of software a company puts on its website to count visits and see how people click. That vendor was breached, and some account holders' names, email addresses, and device details were exposed. Chat content, passwords, and secret keys were not.

The damage there was limited. The lesson is not. When you buy an AI service, you also buy every company that service relies on: its analytics, its hosting, its support tools, its plugins. You inherit a supply chain you never chose and may never have heard of.

## A Real Business Example

### The engineer who asked the chatbot for help

In April 2023 Bloomberg reported that Samsung had banned generative AI tools such as ChatGPT on company equipment. The reason was not a theory about risk. Engineers had pasted confidential source code into a public chatbot while looking for a bug fix, on more than one occasion, in a division working on semiconductors — one of the most closely guarded kinds of code in the world. A memo reviewed by Bloomberg reportedly noted that an internal survey found 65 percent of respondents already believed the tool was a security risk.

Look at this from the engineer's side. Nothing was stolen. Nobody broke in. A person was stuck on a problem, found a tool that solved it in ten seconds, and used it. The tool was excellent. The judgement was poor. The code was not theirs to give away.

This is the single most common AI security failure in existence, and it is not exotic. It happens in law firms when someone pastes a client's contract to summarise it. In accountancy practices with a tax return. In agencies with a client's unreleased campaign. In HR with a stack of CVs. The pattern is always the same: a helpful tool, a rushed person, and a copy-paste that crosses a boundary nobody drew.

Two things follow. First, the fix is not only a ban, because a ban with no alternative does not stop the behaviour; it hides it, which is worse, since now you cannot see the data flowing. Second, the fix is not only training, because a person in a hurry at five in the evening will not remember a forty-page policy. The fix is to make the safe path the easy path: an approved tool that is faster than the unsafe one, plus a control that catches the worst data before it leaves. Both are in the next section.

## How to Do It

### 6.7 How to protect yourself: AI firewalls, filters, monitoring

Do this in order. Each step depends on the one before it.

**Step 1: Draw the map before you buy anything.**
Take one sheet of paper. List every AI tool that touches your company, including free ones on staff phones. For each: what data goes in, what comes out, where it is stored, who the vendor is, and whether you have a signed contract. You will find tools you did not know about. This is the most valuable security document you will produce this year.

**Step 2: Put one door between your people and AI services.**
An "AI gateway" or "AI firewall" is a single point all AI traffic passes through, so you can see it and control it. Mainstream products do this: content-safety and prompt-shielding services from the big cloud platforms, guardrails built into cloud model services, AI-aware gateways, and data-loss-prevention tools that inspect what employees send. You need to know the category exists and what it buys: one place to allow or block tools, inspect content, and keep logs.

**Step 3: Filter what goes out.**
The highest-value control on this list. Configure your gateway or data-loss tool to block or warn on the categories that must never leave: national ID and tax numbers, bank and card numbers, health information, payroll files, signed contracts, source code, and client-confidential documents. A pop-up that says "this looks like personal data, are you sure?" stops a large share of accidents by itself, because most of them are accidents.

**Step 4: Filter what comes in.**
This is the prompt-injection defence, and it has one golden rule: **never let an AI tool act on instructions it finds inside a document, an email, a webpage, or a spreadsheet.** A model that reads your inbox should summarise, not obey. Where a tool must act, require a human to confirm before it runs. Treat every external document as untrusted input, the way you treat an attachment from a stranger.

**Step 5: Give agents the least power possible.**
Decide an agent's permissions on paper before you connect it. Read-only where you can. Its own service account, never a shared administrator login. One folder, not the whole drive. A spending cap on anything that costs money. A time limit. A named human owner. If it does not need to delete, do not let it delete. Give the tool the smallest set of keys that still lets it do the job.

**Step 6: Log everything and read the logs.**
Record who used which AI tool, when, and roughly what for — then review it. A weekly fifteen-minute look shows you unapproved tools, unusual volume, and patterns you can turn into policy. No logs means no investigation: after an incident you will be guessing.

**Step 7: Keep a human checkpoint on anything irreversible.**
Any action that cannot be undone — sending money, deleting records, emailing a customer list, signing something — needs a human approval step. Not a notification. An approval.

**Step 8: Do not neglect the boring basics.**
AI does not replace ordinary security; it sits on top of it. Multi-factor authentication on every account that can reach company data, including vendor portals. A password manager so nobody reuses passwords. Prompt updates. Tested backups kept offline. Endpoint protection on every machine. If these are weak, no AI-specific control will save you.

**Step 9: Train with one rule, not a manual.**
Give staff one sentence they can carry: *if you would not put it in an email to a stranger, do not put it in an AI tool.* Then tell them what to do instead, and make that alternative easy. Rules without alternatives get ignored.

**Step 10: Plan for the vendor being down.**
Ask every AI vendor: what happens if you are unavailable for a week? Have a manual fallback for any process you have made dependent on them. Availability is a security property, and the healthcare story above is the proof.

## Ethics and Responsibility

Security is an ethical matter before it is a technical one. When customers give you their address, their health detail, or their payment information, they trust you to hold it safely. Losing it is not an accident that happened to you; it is a harm done to them. That is the same duty of care discussed in [Chapter 4](ch04-ethical-ai-doing-the-right-thing.md), applied to systems rather than to decisions.

Three duties follow. **Duty of competence:** deploying a tool you do not understand is not neutral. If you cannot say where your data goes, you cannot protect it, and "we did not know" is a weak defence in front of a regulator, a customer, or a court. The literacy duty in the EU AI Act, covered in [Chapter 5](ch05-rules-and-legal-responsibility.md), makes this explicit. **Duty to disclose:** if you are breached, tell the people affected promptly and clearly. Hiding it to protect your reputation transfers the cost of your problem onto the people who trusted you; the legal deadlines are in [Chapter 10](ch10-privacy-and-gdpr.md). **Proportionality in monitoring:** logging AI use protects the company, and it also means reading what your staff type. Set a written policy saying what is logged, why, who can see it, and for how long. Monitor the data flow, not the person. Secret surveillance damages trust and often breaks local law.

One last rule: do not use AI tools to attack other systems, and do not test your own defences on live data or live customer accounts. Use a separate test environment.

## Mistakes to Avoid

1. **Treating an AI tool like a search engine.** A search engine indexes public pages. An AI service receives your text, stores it, and processes it on someone else's computers.
2. **Granting broad permissions "to make it work."** Convenience today is a breach tomorrow. Grant the minimum and widen only on a proven need.
3. **Letting an AI read everything.** Pointing an assistant at a shared drive that holds payroll, legal files, and client records turns one compromised account into total exposure.
4. **No logging.** Without records you cannot find out what happened, or prove you were in control.
5. **Accepting "enterprise-grade" as an answer.** Ask instead: do you train on my data, how long do you keep prompts, who are your sub-processors, where is data stored, will you tell me if you are breached.
6. **Ignoring the free consumer plan.** Staff on personal accounts means your data goes somewhere with no contract and no controls.
7. **Blocking everything.** A ban with no approved alternative does not stop usage; it hides it.
8. **Confusing confidentiality with integrity.** Poisoning and tampering are not leaks. Guard only against data leaving and you will miss data being corrupted.
9. **Trusting a vendor because they are big.** The largest healthcare payment breach in history started with a missing second login factor.
10. **Treating security as a one-time project.** Threats, tools, and staff change. Review the map every quarter.

## Practical Exercise

### 6.9 Map your vulnerability points

Set aside ninety minutes with one colleague who knows the daily work. Do not do this alone.

**Part A — List the data (20 minutes).** Write down every category of sensitive information your company holds. Typical rows: customer names and contacts, payment or bank details, national ID or tax numbers, employee and payroll records, CVs and applicant data, health or insurance information, contracts and quotes, source code or designs, strategy and financial plans.

**Part B — Trace each one (40 minutes).** For each row answer five questions in writing:

1. Where does it live? (system, folder, spreadsheet, paper)
2. Who can reach it? (roles, named people, contractors)
3. Which AI tool touches it, if any?
4. Does it leave our building? Where does it go, and under what contract?
5. Can we see it happening? (logging, yes or no)

**Part C — Score and pick (30 minutes).** Mark each row:

- **Red** — sensitive data that leaves the company with no contract and no logging.
- **Amber** — sensitive data that stays inside but is widely reachable, or leaves under a contract you have not read.
- **Green** — low-sensitivity data, or sensitive data with a contract, a filter, and logs.

Every red row is an action for this month. Pick the top five and write one owner and one deadline next to each. A typical first five: multi-factor authentication on vendor accounts, an approved AI tool for staff, a data-loss rule for ID numbers, shared-drive access cut down to the folders each role needs, and a one-page acceptable-use rule. Keep the map on one page, and update it every quarter and whenever you add a new AI tool.

## Checklist

### 6.10 The 10 minimum security actions

- [ ] **Every account has multi-factor authentication**, including vendor portals, email, banking, cloud storage, and administrative logins.
- [ ] **A written map exists** of every AI tool in use, what data goes into each, and where that data is stored.
- [ ] **An approved AI tool exists and is easier to use** than the unapproved alternatives.
- [ ] **Outbound filtering is in place** for ID and tax numbers, payment details, health data, payroll, contracts, and source code.
- [ ] **No AI tool acts on instructions found inside documents it reads**; actions need human confirmation.
- [ ] **Every AI agent runs with least privilege**: its own account, read-only where possible, capped spending, no administrator rights.
- [ ] **Logs exist for AI use, and someone reviews them weekly.**
- [ ] **Irreversible actions require a human approval step**, not just a notification.
- [ ] **Vendor due diligence is done in writing**: training on your data, retention period, sub-processors, data location, breach notification terms.
- [ ] **Backups are tested and kept offline, and a manual fallback exists** for any process that depends on an AI vendor.

## Key Takeaways

- AI makes attacks cheaper and faster, and it multiplies the number of doors into your business; both change at once.
- The most common leak is not a hack — it is a helpful employee pasting confidential data into a tool they never checked.
- Guard all three properties: confidentiality (data leaving), integrity (data being poisoned), and availability (a vendor going down).
- The core defences are a data map, one controlled gateway, outbound filtering, least privilege for agents, and logs someone actually reads.
- Your risk includes your vendors' risk, and their vendors' risk too; ask who they rely on before you rely on them.
