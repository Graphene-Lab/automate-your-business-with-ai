# Chapter 8 — Self-Hosting: Keep Your Data Under Control

## In Simple Words

Self-hosting means running software on computers you own or control, instead of renting it from someone else's computers.

You already know both sides of this. Renting a hotel room is cloud: someone else cleans, repairs, and holds a spare key. Owning a house is self-hosting: you fix the boiler yourself, but nobody else has a key.

Applied to AI, self-hosting means the model — the software that does the thinking — runs on a machine in your office or on a server you control. Your questions go in there. The answers come out of there. Nothing travels over the internet to a company you did not choose.

This was not possible for a small business until recently. Until 2022 the best language models lived only inside giant data centres, and you could reach them only through a rented doorway called an API — a standard interface a company opens so other software can ask its systems questions. Every question you typed went through that doorway and landed on their machines.

Then two things changed. First, open models appeared: models whose trained files anyone can download and run. Second, compression techniques became good enough that a compressed model runs on an ordinary powerful desktop computer, with only a small loss in quality.

The trade is a triangle, and you cannot have all three corners at once.

- **Control.** You decide what happens to your data, which model you use, when it changes, and who can see it.
- **Capability.** How good the AI actually is on hard tasks.
- **Cost.** What you pay, in money, time, and attention.

Cloud AI gives high capability for low effort and low control. Self-hosting gives high control, moderate capability, and a cost you pay up front in hardware and then again in ongoing time. The right answer depends on what you are doing.

Two honest sentences before we go further. Self-hosting is not automatically more secure — a badly configured local server is worse than a well-run cloud service. And self-hosting is not automatically cheaper — at small scale, renting usually wins. What self-hosting buys is one specific and valuable thing: your data does not leave, and nobody can change your system without you knowing.

Related topics elsewhere: [Chapter 11](ch11-digital-sovereignty.md) covers the wider idea of controlling your own digital tools, [Chapter 9](ch09-third-party-services-and-shadow-ai.md) covers the opposite pattern of unmanaged third-party services, and [Chapter 6](ch06-cybersecurity-in-the-ai-era.md) covers the security basics that still apply to a machine in your own office.

## A Bit of History

**1990s to 2000s: everything at home.** A small business had a server in a cupboard. Email, files, and accounts all sat on premises. You owned the machine and all of its problems.

**2000s to 2018: the move out.** Broadband got fast, and renting became easier than owning. Email went first, then files, then accounting and customer records. "The cloud" became the default answer. The joke among engineers was accurate: there is no cloud, it is just someone else's computer.

**2013: containers.** Docker arrived and packaged software so it ran the same way everywhere. This quietly made self-hosting easy again, because you no longer needed a specialist to rebuild an application on each new machine.

**2022: AI was only a rental.** The best language models existed only inside a handful of large companies. If you wanted AI, you sent your text to them. There was no alternative worth using.

**2023: the open-model year.** Meta released Llama as a research model in February, then Llama 2 with open weights in July. Mistral AI released a strong seven-billion-parameter model in August. "Open weights" means the trained files are published, so anyone can download and run them. The same year, quantisation — compressing a model so it needs far less memory — became good enough for daily use. Suddenly a capable AI was not only in a data centre.

**8 July 2023: Ollama.** A tool called Ollama was released, open source under the MIT licence, written mainly in Go with some C and TypeScript, by Jeffrey Morgan and Michael Chiang. Its job was to remove all the friction. One command downloads a model and runs it locally, with a simple interface and a local service other programs can talk to. It used the llama.cpp engine for the actual work on your hardware.

**2024: "sovereign" becomes a buying criterion.** Companies in regulated sectors, and several European governments, began asking for AI that stays inside a country and inside their own walls. Cloud providers answered with sovereign-cloud options, and a market for on-premise AI grew quickly.

**2026: an open-source enterprise client.** In April 2026 MZLA Technologies, a Mozilla subsidiary, announced Thunderbolt, an open-source AI client built to be self-hosted. The Curiosity section covers it.

The shape of this history is a loop. We started self-hosting, moved out for convenience, and are now moving back for control — with far better tools than the first time.

## Curiosity

### 8.7 Mozilla's open-source AI client for "AI you control"

In April 2026, MZLA Technologies Corporation — a wholly owned subsidiary of Mozilla, the non-profit behind Firefox — announced **Thunderbolt**. It is an open-source, cross-platform AI client built for organisations that want to run AI on their own terms.

The details that matter for this chapter:

- **Self-hostable.** It runs on the customer's own infrastructure. The project describes support for on-premise, sovereign-cloud, and air-gapped setups — meaning a network physically disconnected from the internet.
- **Model-agnostic.** It works with any agent that speaks the Agent Client Protocol, and with any model that offers an OpenAI-compatible API. In practice that means you can point it at a local model, your own server, or a commercial provider, and switch without changing your tools.
- **Everywhere.** Web, Windows, macOS, Linux, iOS, and Android.
- **Connected to your systems.** It integrates with enterprise systems through the Model Context Protocol — a standard way to let an AI tool reach your internal data and actions — and supports reusable automations and an extensible API.
- **Auditable.** Because the code is open, you or a third party can read it and check what it actually does. The project has said it is going through a security audit.
- **A partner for European sovereignty.** It pairs with deepset's Haystack, an open-source orchestration platform, for sovereign deployments in Europe.
- **Support included.** Enterprise support and forward-deployed engineering are offered, which is the part most open-source projects leave you to solve alone.

The positioning is worth noticing. The framing is "AI you control," and the argument is that AI is too important to outsource entirely. That is the same argument a small business owner makes when they decide to keep payroll files on their own machine rather than in a service they never inspected.

A smaller, older example of the same idea sits in an email app many people already use. The ThunderAI add-on for Thunderbird added support for local models through Ollama in version 2.1.1, released in August 2024. With that setup the model runs on your own computer, so the email text never leaves the machine, and no cloud account or API key is needed. It is a small feature, and it makes the point clearly: local AI is no longer a research project. It is an option inside a free email client.

## A Real Business Example

### Even Apple built its own cloud

Apple is a company that could rent almost anything. In June 2024 it announced a system called Private Cloud Compute, built for the AI features in its devices when a task is too large for the phone itself. What it chose to do with that system is the lesson.

Apple built its own servers around its own chips with a hardened operating system. It designed the system for stateless inference — process the request, return the answer, keep nothing. And it made an unusual promise: it would publish the software image of every production build so that outside security researchers could inspect exactly what is running, and check that the machine they are talking to really is what it claims to be. In October 2024 Apple published a security guide and invited researchers to attack the system.

Three things follow for a small business.

First, notice the reasoning. Apple did not build a cloud because it could not rent one. It built one because renting would have meant keeping user data on someone else's terms, and its whole brand is that it does not. Control of the machine was worth real money to them.

Second, notice the verification idea. Publishing the software so outsiders can check it is the same instinct as open-source auditing. Trust is reduced by making the system inspectable, not by promising to be good.

Third, notice the size of the gap. Apple spent a fortune to reach "we keep nothing." Most small businesses cannot copy that. But you can copy the question: *who runs the machine my data goes to, what do they keep, and can anyone check?* If you cannot answer those three questions about a tool, you should not put sensitive data in it. And if the honest answer is "we cannot check," a model running on your own machine becomes a serious option.

## How to Do It

### 8.5 How to start: from open-source tools like Ollama to local models

**Step 1: Pick one task and one person.**
Do not buy hardware first. Choose one repeated task that involves sensitive data — summarising contracts, drafting replies to standard enquiries, turning meeting notes into action lists. Give it to one curious person with a good computer.

**Step 2: Install Ollama.**
Ollama runs on Windows, macOS, and Linux. After installing, one command pulls a model and starts a chat in your terminal. Under the hood it starts a small service on your own machine, on port 11434, that other programs can talk to. That local service is what lets you connect the model to your own tools later.

**Step 3: Choose the model by size, not by name.**
Model sizes are counted in parameters, a rough measure of how big and capable the model is. As a rule of thumb:

- **1 to 3 billion** — fast and light, runs on an ordinary laptop. Good for short summaries and simple drafting.
- **7 to 9 billion** — the practical middle. Good general quality, needs a decent machine with enough memory.
- **70 billion and above** — much stronger, but needs serious hardware and a lot of memory. Usually not a small-business starting point.

Look for **quantised** versions. Quantisation compresses the numbers inside the model so it needs far less memory and runs faster, at the cost of a small drop in quality. For most office tasks that drop is acceptable.

**Step 4: Add a friendly interface.**
The terminal is fine for testing. For daily use, add a chat interface that runs locally, or plug the model into an app people already use — the Thunderbird add-on mentioned above is one example. The goal is that a non-technical colleague can use it without help. If only one person can drive it, it will never be adopted.

**Step 5: Keep it actually local.**
This is where people fail. The local service must listen only on your own machine, not on the whole network. Security researchers have found many Ollama servers exposed to the public internet because they were set to accept connections from any address. So: keep the default local binding, put a firewall in front, never open port 11434 to the internet, and do not run it with administrator rights. A local tool is not automatically a safe tool.

**Step 6: Let it read your own files.**
The most useful next step is retrieval, often called RAG. In plain words: instead of retraining the model, you put your documents into a searchable index. When someone asks a question, the system finds the relevant passages and hands them to the model along with the question. The model answers from your documents. Nothing is trained on your data, and the whole thing can run on your own machine. This is how you get "ask our handbook" without sending the handbook anywhere.

**Step 7: Scale only when the test worked.**
If the pilot is useful, then buy hardware. A workstation with a strong graphics card is the usual answer, because graphics memory is what limits how large a model you can run. Apple machines with unified memory are a common choice for the same reason. A small server makes sense when several people need it at the same time.

**Step 8: Decide the split.**
Most companies end up hybrid. Sensitive data and routine high-volume tasks run locally. Hard reasoning, very long documents, and specialist features use a cloud service under a proper contract. Write the rule down: which data goes where, and who decides.

### 8.6 Ideal use cases

**Sensitive personal data.** Health records, HR files, payroll, applicant CVs, client financial details. If the data must not leave, local processing removes the question entirely.

**Proprietary information.** Designs, drawings, source code, tender and bid documents, pricing models, strategy plans. These are the files that would hurt most if a vendor kept them or leaked them.

**Regulated sectors.** Healthcare, legal practices, banking and insurance, government and defence, and any business under data-residency rules that require data to stay inside a country or region. Self-hosting turns a hard compliance conversation into a simple one.

**Poor or no connectivity.** Field sites, factories, ships, mines, remote offices, emergency response. A local model works when the internet does not.

**High-volume repetitive work.** Thousands of tickets, invoices, or documents. A price per request hurts at volume; a fixed machine does not grow.

**Cheap experimentation.** Trying ideas without a meter running. Useful before you commit budget.

**Where it fits badly:** frontier-level reasoning, very long documents, advanced image generation, and any team with no technical support at all. If nobody can maintain it, do not start it.

## Ethics and Responsibility

Self-hosting solves one ethical problem and creates others. Be clear about which is which.

**What it solves.** Your customer data stops travelling to companies you did not choose, and cannot be used to train someone else's product without you. That is a real gain in respect for the people whose data you hold.

**What it does not solve.** The model can still be wrong, biased, or confidently misleading. Running a biased model on your own hardware does not make it fair. The duties in [Chapter 4](ch04-ethical-ai-doing-the-right-thing.md) still apply, and so do the disclosure rules in [Chapter 5](ch05-rules-and-legal-responsibility.md).

**What it adds.** You are now the operator. Patching, access control, logging, and backups are your job. If an unpatched local server leaks data, that is on you in a new and very direct way.

**Employee monitoring.** If you log prompts to a local system, you now hold a detailed record of what your staff asked. Have a written policy on what is kept, why, who reads it, and for how long. Keep it proportionate, and tell people.

**Do not oversell sovereignty.** "Sovereign" is a marketing word as much as a technical one. If you claim control but cannot patch, back up, or audit, the claim is empty. Say what you actually have, and say plainly what you do not.

**Energy.** A machine running models all day uses power. Local is not automatically greener than a large, efficient data centre. If you claim an environmental benefit, check it first.

## Mistakes to Avoid

1. **Buying hardware before testing a task.** Test with a rented or borrowed setup first. Hardware bought on hope sits unused.
2. **Exposing the local AI service to the internet.** This is the most common and most serious self-hosting error. Keep it local, firewall it, do not open the port.
3. **Assuming local equals secure.** You now own the security of that machine, including the parts you never thought about.
4. **No backups.** The machine, the models, the configuration, and the document index all need backing up.
5. **Choosing the biggest model.** Bigger is slower, hungrier, and often no better for your actual task.
6. **Ignoring model licences.** Open-weight models come with different terms, including rules on commercial use and on how you may describe your use. Read the licence before you build on it.
7. **One-person dependency.** If one person knows how it works and leaves, the system stops. Write down the setup, the restart, and the restore steps.
8. **Self-hosting the wrong workload.** If the task needs frontier quality, local will disappoint, and you will wrongly conclude the technology is useless.
9. **Never updating, or updating without testing.** A new model version changes answers. Re-run your sample tasks after every change.
10. **Treating it as all or nothing.** A hybrid setup is usually the right answer, not a total move in either direction.

## Practical Exercise

### 8.8 Evaluate whether self-hosting suits your company

Score each line 0, 1, or 2. Be honest.

| Question | 0 | 1 | 2 |
|---|---|---|---|
| How sensitive is the data? | Public | Internal | Client-confidential or regulated |
| Technical support available | None | Part-time IT help | Someone who can maintain a server |
| Hardware budget | None | One good workstation | Workstation plus a small server |
| Task complexity | Summaries and drafting | Questions over documents | Complex reasoning, very long documents |
| Connectivity | Unreliable | Fine | Fine |
| Volume | Occasional | Daily | High and growing |

Read the score line by line, because the lines do not all push the same way.

- **Sensitivity 2** and **Volume 2** both push toward self-hosting.
- **Technical support 0** pushes strongly against it, whatever the other scores say.
- **Task complexity 2** pushes against it, because local models lag on hard reasoning.

Now run a one-day test before you spend anything. Take twenty real tasks from your list. Do ten with a mid-size local model and ten with a cloud service. Compare three things: was the answer good enough to use as it stood, how long did it take, and what would it have cost the other way. Write the results down.

If the local answer was usable for most tasks, self-hosting is worth the investment. If it was usable for only a few, keep those local and leave the rest in the cloud under a contract. Either way you now have evidence instead of an opinion.

## Checklist

### 8.9 What you need to start

- [ ] **One named task** that involves sensitive data and repeats often.
- [ ] **One named person** who can install, restart, back up, and update the system — or a plan to hire one.
- [ ] **A machine with enough memory**, chosen after a test, not before.
- [ ] **A model chosen by size and quantisation**, matched to the task rather than to the largest available.
- [ ] **A local interface** a non-technical colleague can use without help.
- [ ] **The service bound to the local machine only**, firewalled, with no port open to the internet.
- [ ] **A written licence check** for the model you pick, including commercial-use terms.
- [ ] **A backup plan** for the machine, the models, the configuration, and the document index.
- [ ] **A patch routine** with a set date, and a re-test of sample tasks after every change.
- [ ] **A written split rule** stating which data stays local and which may use a cloud service, and who decides.

## Key Takeaways

- Self-hosting means the AI runs on machines you control, so your data does not leave them.
- It became practical for small businesses when open-weight models and good compression arrived in 2023, and tools like Ollama removed the setup friction.
- You trade capability and convenience for control: the triangle is control, capability, and cost, and you cannot have all three.
- Local is not automatically safe or cheap; a misconfigured local server is a real risk, and maintenance is now your job.
- Start with one task, one person, and a one-day test before buying any hardware.
