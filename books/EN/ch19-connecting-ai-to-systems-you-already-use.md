# Chapter 19 — Connecting AI to Systems You Already Use

## In Simple Words

Your business already runs on software: the system that tracks your customers, the email you answer, the spreadsheets you live in, the accounting program you invoice from. AI is most useful when it plugs into these existing systems instead of sitting off in a corner doing nothing. This chapter is about that connection — how AI talks to the tools you already have.

The key idea is the **integration**: a link that lets one piece of software pass information to another automatically. When your AI can read your customer list, draft a reply in your inbox, and write a note back into your records, it becomes a real helper. When it cannot connect to anything, it is just a clever chat window you have to copy and paste into.

A good analogy is plumbing. A new water filter is useless if it is not connected to your pipes. The value comes from the connection, not the filter alone. Integrations are the pipes that let AI flow into your daily work. Your job is to understand which pipes exist, which you can connect yourself, and when you need a plumber.

This chapter looks at the common systems AI connects to — management software, CRM, email, spreadsheets. It gives examples of simple automations you can picture. It explains what an **API** is in plain words (it is simpler than it sounds). It tells you when you can do it yourself and when to call a technician. And it warns you about the traps: dependencies that block you, and the maintenance that every connection needs.

The promise: connected AI saves real time every day. The caution: a bad connection can break things or trap you. Do it with a map and a plan.

## A Bit of History

**1960s–1970s: programs that talk to each other.** Early business software had to exchange data — an inventory system feeding an accounting system. Engineers built the first links between programs, often by hand, sharing files in agreed formats. Integration was born out of pure necessity.

**1990s: enterprise integration becomes a profession.** As companies ran many systems at once, connecting them became a whole field. Tools with long names — middleware, enterprise application integration — tried to be the central hub that linked everything. It was powerful, expensive, and usually needed specialists.

**2000s: the API economy.** Software began exposing clean, documented doors for other software to use. These doors are called APIs. Suddenly a small company could connect to big services — maps, payments, messaging — without building them. A whole economy of connected software appeared.

**2010s: no-code and the citizen integrator.** Tools like Zapier and Make let non-programmers connect popular apps by pointing and clicking. You could say "when a new lead lands in my form, add it to my CRM and email me" without writing code. The "citizen integrator" — a business person who builds their own connections — became real.

**2020s: AI as the new connector.** AI tools gained the ability to read, write, and act across systems through their own APIs. Now the AI can be the one doing the connecting: reading your inbox, updating your records, drafting your replies. The plumbing got smarter, and the need to understand it grew just as fast.

The arc: from hand-built file links to a world where software expects to be connected. The connection is no longer a luxury; it is where the value lives.

## Curiosity

### The memo that connected the world

In 2002, the CEO of Amazon, Jeff Bezos, sent a now-famous internal memo to his engineering teams. The details are widely reported in tech history. The core order was blunt: from now on, every team must share its data and functions through a clean, documented interface — an API — and nothing else. No direct access to another team's database. No back-door shortcuts. If a team wanted something from another team, it had to ask through the published interface, or build it itself.

The reason was not tidiness. It was to make Amazon fast and flexible. When every part of the company could be reached through a clean door, teams could change their own systems without breaking everyone else, and new services could be built quickly on top of old ones.

That discipline is widely credited as a foundation of what became **Amazon Web Services (AWS)** — the cloud platform that now powers a huge share of the internet. A rule about how software talks to software inside one company turned into one of the largest technology businesses on earth.

The lesson for a small business is the same in miniature: **clean, documented connections make you flexible; messy shortcuts make you fragile.** When you connect AI to your systems, build clean links, not back-door hacks. The tidy pipe today is the freedom you will thank yourself for tomorrow.

## A Real Business Example

*The following is an illustrative composite of common real-world patterns, not a single named company.*

A small property-management firm ran on three systems that did not talk to each other: a CRM holding tenant contacts, a shared inbox for maintenance requests, and a spreadsheet tracking repair jobs. Every request meant copying details by hand from the inbox into the spreadsheet, then into the CRM. Staff spent hours a day on copy-paste, and details slipped through the cracks.

They connected the three with a simple automation. When a maintenance email arrived, an AI read it, pulled out the tenant name, the property, and the problem, and created a row in the spreadsheet automatically. It also drafted a reply to the tenant confirming the request. A human checked the draft and pressed send. The CRM note was added by the same automation.

The result was not magic — it was plumbing. The hours of copy-paste mostly disappeared. Fewer requests were lost, because the same automation flagged anything it could not read clearly for a human. The firm did not replace staff; it removed the boring part of their day so they could handle more properties without more people.

The lesson: the win came from connecting systems that already existed, not from buying something new and dramatic.

## How to Do It

### 19.1 Management software, CRM, email, spreadsheets

These are the four systems most businesses already run, and the four AI connects to most often.

- **Management software (ERP).** A system that runs the core of your business — inventory, orders, production, finance. ERP stands for Enterprise Resource Planning. AI can read reports from it, flag unusual numbers, or draft summaries.
- **CRM.** Stands for **Customer Relationship Management** — the system that holds your customers, leads, and every interaction with them. AI can draft replies to leads, log calls, and pull a customer's history to help you answer faster.
- **Email.** The inbox is where most small-business work lives. AI can sort, summarize, and draft replies here. This is often the single most valuable connection.
- **Spreadsheets.** The universal tool. AI can fill them, read them, and update them from other sources.

Start where the pain is highest. For most small businesses, that is email and the CRM. Connecting AI to those two gives the biggest daily relief. Do not try to connect everything at once — pick the one that hurts most and start there.

### 19.2 Examples of simple automations

Concrete examples help you picture what is possible. Each of these is a small, common connection:

- **Inbox to CRM.** A new inquiry email automatically creates a lead in your CRM, with the sender's details filled in.
- **Form to spreadsheet.** A customer fills a web form; the answers land in a spreadsheet row automatically, and the AI tags the request by type.
- **Email to draft reply.** AI reads a standard request and writes a draft reply in your inbox; you check and send.
- **Document to record.** AI reads an invoice PDF and writes the amount, date, and vendor into your accounting system.
- **Meeting to notes.** AI turns a recorded meeting into a summary and action items, then files them where your team can see them.
- **Ticket to alert.** AI reads incoming support messages and flags the angry or urgent ones to a human first.

Notice the pattern: AI reads from one place, does something useful, and writes to another, with a human check where it matters. That is the shape of almost every good automation.

### 19.3 When you need a technician

You can do a surprising amount yourself with no-code tools. But some jobs need a professional. Know which is which.

**You can likely do it yourself** when: the apps are popular (so no-code connectors exist), the data is simple, the automation is small, and a mistake is cheap. Point-and-click tools cover a lot here.

**Call a technician when:**

- **The connection touches money, legal records, or sensitive data.** A mistake here is expensive or dangerous.
- **The systems are old or custom-built** and have no ready-made connector.
- **You need a reliable, always-on link** that must not fail.
- **Security is involved** — connecting to customer data means getting access control right (see [Chapter 20](ch20-implementing-ai-securely.md)).
- **You do not understand what you are connecting.** Never connect what you cannot explain.

A technician is not an admission of failure. It is the right call for the risky or complex parts, the same way you call a plumber for the main line and fix the tap yourself.

### 19.4 APIs and integrations explained simply

An **API** sounds technical, but the idea is simple. An API is a **menu that one piece of software offers to another.** It is a list of things you are allowed to ask it to do, and how to ask.

Think of a restaurant kitchen. You do not walk in and start cooking. You look at the menu, order from what is offered, and the kitchen brings it. The menu is the API. It tells you what you can request ("get this customer's details," "add a new row," "send this email") and how to request it. You cannot order something off the menu, and you never touch the kitchen directly.

Why this matters for AI: when a system has an API, an AI can use that menu to read and write data safely and predictably. When a system has no API, connecting to it is hard or impossible. So when you choose software, a good question is: **does it have an API?** If yes, AI can likely connect to it. If no, you may be stuck.

An **integration** is the connection you build using one or more APIs — the act of wiring the menu of one system to the needs of another. The API is the door; the integration is the hallway you build through it.

Two plain terms you will hear:

- **Read access** — the AI can look at data but not change it. Safer.
- **Write access** — the AI can change data. More powerful, more risky. Give write access only where you need it.

### 19.5 Avoiding dependencies and blocks

Every connection creates a **dependency** — one thing now relies on another. Dependencies are normal, but too many, or the wrong ones, can block you.

Watch for these traps:

- **A single point of failure.** If one connection breaks and your whole workflow stops, that is a fragile single point. Have a fallback: a way to do it by hand if the link dies.
- **A chain of dependencies.** If A needs B needs C needs D, one broken link stops everything. Keep chains short.
- **A dependency on a tool that can vanish.** If you connect to a small service that shuts down, your automation dies. Prefer stable, established tools.
- **Lock-in through integration.** If all your systems are wired together in a way only one vendor understands, leaving becomes hard. Keep connections clean and documented so you can rewire later. (Lock-in is covered in [Chapter 9](ch09-third-party-services-and-shadow-ai.md).)
- **Undocumented connections.** A link nobody knows how it works is a time bomb. Document every connection.

The rule: **build clean, short, documented connections with a manual fallback.** The Amazon memo lesson again — clean doors, no back-door hacks.

### 19.6 Maintenance and updates

A connection is not "set and forget." It is a living thing that needs tending.

- **Systems change.** Your CRM updates, your email provider changes a format, an API gets a new version. When one side changes, the connection can break.
- **Silent failures.** A connection can stop working quietly, and data stops flowing without anyone noticing. Check that data is actually arriving.
- **New cases appear.** The automation handled the common cases; a new kind of request comes along and it does not know what to do. Review what it is missing.
- **Security updates.** Connections to data need their access checked over time, especially when staff join or leave.

Plan for maintenance: assign someone to watch the connections, check them regularly, and fix breaks fast. Build a simple alert — if no data flows for a day, someone should know. A little tending keeps the plumbing from flooding.

## Ethics and Responsibility

Connecting AI to your systems means connecting it to real people's data. That carries responsibility.

**Connect with consent and care.** If AI will read customer emails or records, know what you are connecting and whether it is allowed. Respect privacy rules (see [Chapter 10](ch10-privacy-and-gdpr.md)).

**Least access.** Give the AI only the access it needs. If it only needs to read, do not give it write. If it only needs one folder, do not give it the whole drive. This limits damage if something goes wrong.

**Keep a human on the send.** For anything that reaches a customer, a human should check before it goes out. Automation that acts alone on customer-facing messages can cause real harm.

**Document for accountability.** When something goes wrong, you need to know what the automation did and why. A documented connection is an accountable one.

**Do not connect what you cannot explain.** If you cannot say in plain words what a connection does to whose data, you should not build it. Complexity you do not understand is risk you cannot control.

Build connections the way you would want your own data handled.

## Mistakes to Avoid

**Connecting everything at once.** Trying to wire every system on day one. Pick the one that hurts most and start there.

**No map.** Connecting without knowing what you have and how it links. Draw the map first.

**Back-door hacks.** Quick, undocumented shortcuts that break later and trap you. Build clean doors instead.

**Too much access.** Giving the AI write access to everything when it only needs to read one thing. Use least access.

**No fallback.** A connection that, when it breaks, stops the whole workflow with no manual plan. Always have a fallback.

**Ignoring silent failures.** Assuming the connection works because no one complained. Check that data actually arrives.

**No maintenance plan.** Wiring it up and walking away. Connections need tending.

**Connecting to a tool that can vanish.** Building on a shaky service that may disappear. Prefer stable tools.

**Letting AI act alone on customer messages.** No human check on what reaches a customer. Keep a human on the send.

**Undocumented links.** Nobody knows how the connection works. Document every one.

**Forgetting staff changes.** Not updating access when people join or leave. Review access regularly.

## Practical Exercise

### 19.7 Exercise: a map of your company systems

You cannot connect what you cannot see. Draw a map of the systems your business runs on.

**Step 1 — List every system.** Write down every piece of software your business uses daily: CRM, email, accounting, spreadsheets, inventory, scheduling, website forms, chat tools. Leave nothing out.

**Step 2 — For each, note four things:**

- **What it holds** (what data lives there).
- **Who uses it** (which people or roles).
- **Does it have an API?** (Check the vendor's site or ask; mark yes / no / unknown.)
- **How sensitive is the data?** (Low / medium / high.)

**Step 3 — Draw the current links.** On paper, draw lines between systems that already pass data today, even if a human carries it by copy-paste. Mark which links are manual.

**Step 4 — Spot the pain.** Circle the manual links that eat the most time or cause the most errors. These are your best automation candidates.

**Step 5 — Mark the risk.** For each candidate, note the sensitivity. High-sensitivity links need a technician and a human check; low-sensitivity ones you can try yourself.

**Step 6 — Pick one.** Choose the single highest-pain, lowest-risk link as your first integration. Pilot it (see [Chapter 18](ch18-your-first-pilot-project.md)).

Keep the map on one page. Update it as systems change. The map is your plan and your defense against connecting blindly.

## Checklist

### 19.8 Integration checklist

Before you connect AI to a system, and after, check every box.

- [ ] **I have a map of all my systems and what data each holds.**
- [ ] **I know which systems have an API and which do not.**
- [ ] **I know how sensitive the data in each system is.**
- [ ] **I picked the highest-pain, lowest-risk link to connect first.**
- [ ] **I used a clean, documented connection, not a back-door hack.**
- [ ] **I gave the AI only the access it needs (least access).**
- [ ] **I know the difference between read and write access and used write only where needed.**
- [ ] **A human checks anything that reaches a customer.**
- [ ] **I have a manual fallback if the connection breaks.**
- [ ] **I checked the connection is stable and not a single point of failure.**
- [ ] **I built a way to detect silent failures (alert if no data flows).**
- [ ] **I documented how the connection works and who maintains it.**
- [ ] **I assigned someone to maintain and watch the connection.**
- [ ] **I reviewed access for current staff and will review it when staff change.**
- [ ] **I ran the connection as a pilot before trusting it fully.**

If a box is empty, the connection is not ready. Fill it first. A connected AI is a powerful helper; a blindly connected one is a liability.

## Key Takeaways

- AI's value comes from connecting to the systems you already run — the connection is the plumbing, and the value flows through it.
- An API is simply a menu one software offers another; if a system has an API, AI can likely connect to it, so ask "does it have an API?" when choosing software.
- Use least access — give the AI only what it needs, prefer read over write, and keep a human on anything that reaches a customer.
- Build clean, short, documented connections with a manual fallback; back-door hacks and silent failures are the traps that break you.
- Connections are living things that need maintenance, monitoring, and access reviews — set them up and never walk away.

<!-- BEGIN agentbridge-examples -->

## Try it with AgentBridge

Here is how the same job looks with AgentBridge. Each box shows the finished result and the one line you type to get it.

### Check a supplier before you commit

![A due-diligence summary of a supplier](../../assets/examples/due-diligence.png)
*A due-diligence summary of a supplier*

**What you ask:** `Research this supplier and tell me their reputation, how long they have been around, and any red flags.`

The agent gathers what is publicly available and gives you a balanced picture with sources, so you decide with your eyes open.

*Tip: Ask it to list what it could not find, so you know where to dig further.*

---

### Check an order in your system

![An order status pulled from the business system](../../assets/examples/order-status.png)
*An order status pulled from the business system*

**What you ask:** `What is the status of order 4821?`

The agent looks up the order in your connected system and tells you its status in plain words — no menu hunting.

*Tip: This works once your business system is connected. See the book's connecting chapter.*

---

### The same assistant in your browser

![The AgentBridge web chat in a browser window](../../assets/examples/web-chat.png)
*The AgentBridge web chat in a browser window*

**What you ask:** `(browser) Draft a thank-you note to our regular customers.`

Open the web address and chat in the browser. Same tools, same documents, same memory — just a different window.

*Tip: Handy when you are on a different machine but still want your own assistant.*

---

### Plug it into your own tools

![The HTTP API lets other programs use the assistant](../../assets/examples/http-api.png)
*The HTTP API lets other programs use the assistant*

**What you ask:** `POST /v1/chat/completions  { "model": "default-agent", "messages": [...] }`

Your own programs can call the assistant through a standard web API, the same way they would call any online service. One integration, many uses.

*Tip: This is for the technical step — the book's connecting chapter walks through it.*

---

### Connect other AI tools to it

![AgentBridge connected to other AI tools via MCP](../../assets/examples/mcp-connector.png)
*AgentBridge connected to other AI tools via MCP*

**What you ask:** `(MCP) Connect AgentBridge as a tool server.`

Other AI applications can use AgentBridge's tools through the MCP standard, so your whole toolkit works together.

*Tip: MCP is for connecting tools; for everyday use the chat is all you need.*

<!-- END agentbridge-examples -->
