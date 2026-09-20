# Chapter 11 — Digital Sovereignty: The Right to Control Your AI

## In Simple Words

Sovereignty, in its oldest sense, means the right to govern yourself without someone else telling you what to do. Digital sovereignty takes that idea and applies it to your digital life: the right to control your own data, your own software, and the machines that run them.

Applied to AI, digital sovereignty answers three plain questions about every AI tool you use.

- **Where is my data?** Which country, which company's servers, under whose law?
- **Who can access it?** The vendor's staff, subcontractors, or a foreign government?
- **How is it processed?** On a model I cannot see, or on a system I can inspect and change?

If you cannot answer those three questions, you do not have sovereignty over that part of your business. You have borrowed someone else's, and you can lose it whenever they change their mind.

This is not the same as self-hosting, though they overlap. Self-hosting, covered in [Chapter 8](ch08-self-hosting-keep-your-data-under-control.md), is one way to gain control. Digital sovereignty is the wider goal: control over where your digital capabilities come from and who holds the leash. You can pursue it with your own servers, with open software, with contracts, or with a mix.

A useful analogy is food. You can buy prepared meals from a factory you never see, and most days that is fine. But if you have an allergy, or you simply want to know what is in your food, you start to care about the recipe and the kitchen. Digital sovereignty is caring about the recipe and the kitchen of your AI — not out of fear, but because the stakes are your data, your customers, and your future.

The opposite pattern, unmanaged third-party services and shadow AI, is in [Chapter 9](ch09-third-party-services-and-shadow-ai.md). The legal duties over personal data are in [Chapter 10](ch10-privacy-and-gdpr.md). This chapter is about the strategic choice: how much of your AI you want to truly control.

## A Bit of History

**2000s to 2010s: convenience erases the question.** As businesses moved to the cloud, almost nobody asked where the data went. The tools were good and cheap. Control was not a buying criterion.

**2013: Snowden changes the mood.** Revelations about mass surveillance made governments and companies realise that data stored in another country could be reached by that country's authorities. The question "where is my data" became a security question, not just a privacy one.

**2018: GDPR makes location matter legally.** Europe's privacy law gave people rights over their data and made companies answerable for where it sat and how it was handled. Data residency — keeping data inside a region — became a real requirement, not a slogan.

**2019 to 2022: "sovereign cloud" appears.** Cloud providers began offering sovereign options: data kept in a specific country, operated under local law, sometimes with local partners. Sovereignty became a product feature.

**2022 to 2023: open-weight models open a new path.** When strong AI models became downloadable and runnable by anyone, a company could, for the first time, run a capable model entirely on its own terms. Sovereignty was no longer only a cloud vendor's promise; it became something you could build.

**2024 to 2025: sovereignty becomes a national and corporate strategy.** Countries and blocs began treating AI capability as strategic. Europe launched funded projects to build its own open models, so that European AI would not depend entirely on foreign providers. The Curiosity section covers one of them.

The arc is clear. Convenience made us stop asking who controls our tools. A series of shocks made us ask again. Now control is a design choice you can make deliberately.

## Curiosity

### 11.6 Building your own assistant, and a continent doing the same

**A representative pattern (illustrative).** Consider a mid-sized professional firm — say an engineering consultancy or a law practice — that needs an internal AI assistant to answer questions over its own documents: past reports, standards, contracts, and notes. The data is confidential and cannot leave the building.

Instead of sending that data to a public AI service, the firm does something different. It downloads an open-weight model — a model whose trained files are published for anyone to run — and runs it on its own servers. It connects the model to its documents through retrieval, so the assistant answers from the firm's own files rather than from the open internet. No question leaves the network. No vendor reads the work. The firm chooses the model, controls the data, and can change or replace the system whenever it likes.

This pattern is real and increasingly common, but the specific firm here is a composite, not a single named company, because organisations that do this rarely advertise it — the whole point is that the work stays private. What matters is that the pattern exists and works today with off-the-shelf open tools, exactly as [Chapter 8](ch08-self-hosting-keep-your-data-under-control.md) describes.

**A real, named version at national scale.** The same instinct is now driving whole countries. In Europe, two funded projects aim to build sovereign, open AI models so the continent is not dependent on foreign providers.

**OpenEuroLLM** is a twenty-partner European consortium that began work on 1 February 2025, funded under the EU's Digital Europe Programme with roughly €55 million. It is coordinated by Jan Hajic of Charles University and co-led by Peter Sarlin of AMD Silo AI. Its stated goal is strategic autonomy for Europe in AI — building capability that Europe controls.

Alongside it, the **EuroLLM** project, supported by Horizon Europe, the European Research Council, and the EuroHPC supercomputing organisation, produced **EuroLLM-22B**, a fully open large language model built for all 24 official EU languages. It was trained on European supercomputers — the MareNostrum 5 system — and released as open source on Hugging Face, so anyone can download, inspect, and run it. The work leans on the EuroHPC "AI Factories" initiative, which pools supercomputing capacity across Europe; one call allocated three million GPU hours on the Leonardo Booster at CINECA in Italy for building open training data.

Why tell this story here? Because it shows that "build your own, keep it open, keep it under your control" is not a paranoid hobby. It is now official strategy at the level of nations. The same logic that leads a country to build its own open model leads a small firm to run an open model on its own server. The scale differs; the principle is identical.

## A Real Business Example

### The clinic that could not send its data anywhere

A private medical clinic wants to use AI to summarise patient notes and draft routine correspondence. The data is health data — the most protected kind under the law, as [Chapter 10](ch10-privacy-and-gdpr.md) explains. Sending it to a third-party AI service raises serious legal and ethical problems, and the clinic is not comfortable with it regardless of the law.

So the clinic chooses control. It runs an open model on its own server, inside its own network, behind its own firewall. The model reads only the clinic's notes and answers only clinic staff. Nothing crosses the internet to a vendor. The clinic can say truthfully to patients, regulators, and its own conscience: this data never left our building.

The cost is real. The clinic had to buy hardware and find someone to maintain it. The model is good but not the absolute best available. Some tasks still need a human. But the clinic gained the one thing it could not buy from any vendor: certainty about where its most sensitive data goes.

Now compare the clinic to a firm that did not think about this and pasted patient data into a free chatbot. The difference is not intelligence. It is that one firm asked the three sovereignty questions first, and the other never did.

## How to Do It

### 11.1 What digital sovereignty is: a simple definition

Digital sovereignty is the ability to control your own digital resources and decisions, instead of depending on someone else's.

Broken down, it has three layers.

**Data sovereignty.** You control where your data is stored, who can access it, and under which law it falls. You can move it or delete it.

**Operational sovereignty.** You control the systems that process your data. You can run them, change them, and keep them running even if a supplier disappears.

**Strategic sovereignty.** You control your own direction. Your future is not held hostage by a vendor's pricing, a foreign government's rules, or a supplier's business decisions.

Sovereignty is not all-or-nothing. It is a dial, not a switch. You can be highly sovereign over one process and barely sovereign over another. The goal is to decide, on purpose, where you want the dial set for each part of your business, rather than drifting to whatever is most convenient.

The opposite of sovereignty is dependence you did not choose — a state where a change in someone else's plans forces a change in yours.

### 11.2 Why it matters for companies: knowing where the data is, who accesses it, how it is processed

Sovereignty matters because the three questions have real consequences.

**Where the data is.** Data stored in another country falls under that country's laws. A foreign authority may be able to compel access. A vendor's data centre location is not a minor detail; it sets the legal ground your data stands on.

**Who accesses it.** A third-party service may let its own staff, its support teams, and its subcontractors reach your data, in countries you never agreed to. You may never see a list of them. Sovereignty means you know, or you control, that access.

**How it is processed.** If processing happens inside a closed system you cannot inspect, you cannot verify what it does with your data or whether it is fair. If you run the system, you can look inside.

These matter for three practical reasons. **Compliance:** laws like GDPR require you to know and control data handling. **Security:** every extra party with access is an extra chance of a breach. **Business continuity:** if a vendor fails, raises prices, or is cut off by sanctions, sovereignty is the difference between a setback and a crisis.

Sovereignty is not an ideology. It is risk management for the part of your business that runs on data.

### 11.3 Proprietary models vs open-source models: what really changes

The choice between a proprietary model and an open-source model changes several things at once.

**A proprietary model** is a closed product. You use it through a service or an API. You cannot see how it works, you cannot run it yourself, and you cannot change it. You depend on the owner for access, price, and continuity. The convenience is high; the control is low. If the owner changes terms or stops the service, you adapt or you stop.

**An open-source or open-weight model** publishes its code or its trained files so you can download and run it yourself. You can inspect it, run it on your own hardware, fine-tune it, and keep using it even if the original creator vanishes. The control is high; the convenience is lower, because you must run and maintain it.

What really changes is **who holds the power and who carries the burden.** Proprietary hands you power to the vendor and carries the burden for you. Open hands you the power and gives you the burden.

Neither is automatically better. Proprietary is right when you want capability with no maintenance and the data is not sensitive. Open is right when you need control, transparency, or independence, and you can support the work. Many businesses use both: proprietary for low-stakes convenience, open and self-run for the data and processes that matter most.

A caution: "open" is a spectrum, and the licence matters. Some open models restrict commercial use or how you may describe your use. Read the licence before you build on it.

### 11.4 The role of open source: transparency, control, community

Open source is the main tool of digital sovereignty, for three reasons.

**Transparency.** Because the code or weights are published, you or a third party can read them and check what the system actually does. You are not asked to trust a black box. This is the same instinct behind the auditing ideas in [Chapter 7](ch07-trustless-trust-without-trusting.md).

**Control.** You can run it where you choose, change it to fit your needs, and keep it as long as you want. No one can take it away from you or force an upgrade you did not ask for.

**Community.** An open project is maintained by many people, not one company's roadmap. Bugs get found by outsiders. The project can survive the original team. You are not alone if something breaks.

Open source also lowers the barrier to entry. A small firm can use the same open model as a large one. That levels the field in a way proprietary products do not.

But open source is not free in the real sense. Someone must install it, update it, secure it, and support it. If you have no one to do that, open source can become a liability. Sovereignty you cannot maintain is worse than comfortable dependence. Use open source where you have, or can hire, the capability.

### 11.5 How to build a sovereign AI infrastructure: the concrete steps

If you decide to gain control, here is a practical path.

1. **Decide what must be sovereign.** List the data and processes that cannot depend on outsiders — sensitive data, core workflows, regulated work. Not everything needs the treatment.
2. **Choose open models.** Pick open-weight models whose licence fits your use. Match the size to your task, as [Chapter 8](ch08-self-hosting-keep-your-data-under-control.md) explains.
3. **Run them on infrastructure you control.** That can be a server in your office, a machine in your own cloud account under your own keys, or a local workstation for a small start.
4. **Keep the data local and connected.** Use retrieval so the assistant answers from your own documents without sending them out.
5. **Control access and keys.** You hold the credentials. No third party has a back door. Log who does what.
6. **Plan for maintenance.** Name who installs, updates, secures, and backs up the system. Write the runbook.
7. **Keep an exit from everything.** Even for the parts you keep proprietary, ensure you can export data and swap tools. Sovereignty includes the ability to leave.
8. **Review the legal ground.** Confirm data residency and the AI Act and GDPR duties for the setup, as [Chapter 5](ch05-rules-and-legal-responsibility.md) and [Chapter 10](ch10-privacy-and-gdpr.md) cover.
9. **Start small and grow.** Pilot one sovereign workflow, prove it works, then extend. Do not rebuild the whole company at once.

The aim is not total independence. It is deliberate control over the parts that matter, with a clear line between what you run and what you rent.

## Ethics and Responsibility

Sovereignty carries its own ethical duties, and it is easy to get them wrong.

**Control is not the same as good.** A sovereign system can still be biased, wrong, or unfair. Running it yourself does not make it ethical. The duties in [Chapter 4](ch04-ethical-ai-doing-the-right-thing.md) still apply.

**Sovereignty must not become secrecy.** "We control it" is not a reason to hide how you treat people's data. You still owe transparency to customers and regulators. Control the system; do not hide from scrutiny.

**Do not use sovereignty to dodge cooperation.** Some problems — fraud, harm, legal requests — require working with authorities. Sovereignty is about protecting the innocent, not blocking legitimate oversight.

**Be honest about your limits.** If you claim full sovereignty but cannot patch, back up, or audit the system, the claim is empty and misleading. Say what you control and what you do not.

**Weigh the collective good.** Open models and shared research benefit everyone. A world where every firm builds a closed silo loses something. The healthiest approach is to control what is sensitive and contribute to what is shared.

## Mistakes to Avoid

### 11.7 Sovereignty for its own sake

The most common mistake is chasing sovereignty as an ideal instead of a tool.

Sovereignty costs money, time, and skills. If you pursue it everywhere, you spend heavily to control things that never needed control. You might build an expensive on-premise system for data that was never sensitive, while a cheap, contracted service would have served you fine and freed your people for real work.

The test is not "can I control this?" It is "what do I lose if I cannot control this?" If the answer is little, do not spend to control it. Save your sovereignty budget for the data and processes where losing control would actually hurt — sensitive data, regulated work, and the systems your business cannot run without.

Sovereignty is a means, not an end. Buy it where the risk justifies the cost, and be comfortably dependent where it does not.

Beyond that trap, watch for these:

1. **Building a fortress you cannot maintain.** Sovereignty without a maintainer becomes a broken system and a false sense of safety.
2. **Confusing open source with free.** Someone must run it. Budget for that.
3. **Ignoring the licence.** Open does not always mean you may use it however you like.
4. **Assuming local equals safe.** A sovereign server still needs security, as [Chapter 6](ch06-cybersecurity-in-the-ai-era.md) covers.
5. **Cutting off all vendors out of principle.** Many vendors earn their place. Total independence is rarely worth it.
6. **No exit plan for the parts you keep rented.** Sovereignty includes the ability to leave any single provider.
7. **Overpromising to customers.** Do not claim control you do not have.
8. **Ignoring that open models can still leak.** A model trained on bad data can still expose personal data, as [Chapter 10](ch10-privacy-and-gdpr.md) notes.

## Practical Exercise

### 11.8 Define your desired level of sovereignty

Take one hour and map your AI uses onto a simple control dial.

List each AI use in your business. For each, answer three questions and set a target level.

- **How sensitive is the data?** Low (public or harmless), Medium (internal), High (client-confidential, regulated, or personal).
- **How critical is the process?** Low (nice to have), Medium (used daily), High (the business stops without it).
- **What is the cost of losing control?** Low, Medium, or High.

Now set a target for each:

- **High sensitivity or high criticality → aim high.** Run it yourself or under a contract that gives you real control and an exit.
- **Low sensitivity and low criticality → aim low.** A convenient third-party service is fine; do not waste money controlling it.
- **Mixed → aim middle.** Use a vendor but keep the data exportable and the workflow swappable.

Write one sentence per use: *"For [use], I want [high/medium/low] sovereignty because [reason]."*

The result is your sovereignty map. It should show a deliberate mix, not a single answer. If everything is "high," you are over-spending. If everything is "low," you are exposed on the things that matter. Adjust until the map matches your real risk.

## Checklist

### 11.9 The pillars of digital sovereignty

Use this to check whether a given AI setup gives you real control.

- [ ] **You know where the data is stored** — the country and the operator.
- [ ] **You know who can access it** — vendor staff, subcontractors, and any government reach.
- [ ] **You can move or delete the data** whenever you choose.
- [ ] **You can export your data** in a common, usable format (no lock-in).
- [ ] **You know how the data is processed** — or you run the processing yourself.
- [ ] **You use open models where control matters**, and you have read their licences.
- [ ] **You hold the keys and credentials** to the systems that matter.
- [ ] **You have a named maintainer** for anything you run yourself, with a written runbook.
- [ ] **You have an exit plan** for every vendor, so no single provider can hold you hostage.
- [ ] **You have checked the legal ground** — data residency, GDPR, and the AI Act.
- [ ] **You have set a deliberate sovereignty level** for each use, not a default.
- [ ] **You can verify your own claims** — if you say the data stays in, you can prove it.

If a pillar is missing for a high-stakes use, that is your priority to fix.

## Key Takeaways

- Digital sovereignty means controlling where your data is, who accesses it, and how it is processed — and being able to answer those three questions for every AI tool.
- It is a dial, not a switch: set it deliberately high for sensitive and critical work, and low where convenience is harmless.
- Open-source and open-weight models give you transparency, control, and community, but only if you have the capability to run and maintain them.
- Sovereignty is a means, not an end; chasing it everywhere wastes money, so buy it only where losing control would actually hurt.
- Real sovereignty always includes an exit: keep your data exportable so no single vendor can hold your business hostage.
