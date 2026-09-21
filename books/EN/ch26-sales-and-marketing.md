# Chapter 26 — Sales and Marketing

## In Simple Words

Sales and marketing are where AI can help you find more customers, talk to them better, and spend less time guessing. The work here is full of small, repeated jobs: sorting which leads are worth calling, writing emails, answering the same questions on your website, and trying to understand what your customers want. AI is good at all of them.

The core idea is *personalization at scale*. A good salesperson remembers each customer, tailors the message, and follows up at the right moment. A small team cannot do that for thousands of people. AI can. It can look at each lead and guess how likely they are to buy, write an email that sounds like it was written for that person, answer a visitor's question at 2 a.m., and spot which customers are about to leave.

This chapter covers four jobs: scoring leads (guessing who is most likely to buy), writing emails and content, running chatbots and assistants, and analyzing customers to understand what they want and who is at risk of leaving.

One honest warning before we start: AI is a powerful amplifier. It will make a good message reach more people, and it will make a bad message reach more people too. It can also push you toward spam — sending too much, too often, to people who did not ask. The goal is not to blast everyone; it is to reach the right person with the right message at the right time. The method for judging whether any of this pays off lives in [Chapter 16 — Goals, Costs, and Return on Investment](ch16-goals-costs-and-return-on-investment.md); this chapter shows you what to automate and how.

## A Bit of History

**1990s: mass marketing and the mailing list.** Marketing automation began with simple email lists. A business could send one message to thousands of people at once. It was cheap and wide, but blunt — everyone got the same message, whether it fit them or not. This was the era of "spray and pray."

**2000s: the CRM and the funnel.** Customer Relationship Management (CRM) software — a database of every customer and every interaction — arrived. Marketers started thinking in a "funnel": many people enter at the top, fewer make it to a purchase at the bottom. The CRM let you track where each person was in the funnel and follow up. Data entered the picture.

**2010s: segmentation and personalization.** With more data, marketers learned to split their audience into groups (segments) and send each group a different message. "People who bought X also bought Y." Personalization made messages more relevant and more effective. But it was still mostly rule-based: if a customer did this, send that.

**Late 2010s: machine learning scores leads.** Machine learning — software that learns patterns from many examples — started scoring leads. Instead of a person guessing who to call first, the model looked at hundreds of signals (company size, what pages they visited, how they found you) and ranked leads by how likely they were to buy. Sales teams stopped wasting time on cold leads.

**2020s: generative AI writes and chats.** Large language models — AI trained on huge amounts of text — can now write emails, ad copy, and product descriptions that sound human. Chatbots built on the same technology can hold a real conversation, answer questions, and guide a customer through a purchase. The chatbot moved from a frustrating menu of buttons to something that actually understands what you typed.

**Now: agents that work the whole journey.** The newest step is the agent — AI that carries a task across several steps. A customer-facing agent can answer a question, check stock, and guide a purchase. An internal agent can take a support request and create the ticket. The mobilezone example below uses exactly this: two agents, one for customers and one for the internal team.

The arc: from one message to everyone, to tracked funnels, to segments, to scored leads, to AI that writes and chats. Each step made marketing more personal and less of a guessing game.

## Curiosity

### 26.5 The chatbot that became two agents

When mobilezone, a Swiss telecom retailer, replaced its old chatbot, it did not build one better bot. It built two different agents for two different jobs: one facing customers, one facing its own staff. That split is the interesting idea. The same AI technology served two audiences in two very different ways — a friendly shopping guide on the website, and a ticket-writing helper inside the company. The story, with the real numbers, is below.

## A Real Business Example

**mobilezone: two Copilot agents, one for customers and one for IT.**

mobilezone is a Swiss telecommunications retailer with more than 125 physical stores, selling phones, plans, and connected devices. It had two separate problems. On the customer side, its old website chatbot was rigid and frustrating — it could only follow a fixed menu and often failed to answer real questions. Inside the company, staff had to fill out clunky forms to report IT issues, which slowed everyone down.

According to a published Microsoft customer case study, mobilezone rebuilt both sides using Microsoft Copilot Studio — a tool for building conversational AI agents — together with Dynamics 365 (its CRM) and the Power Platform (Microsoft's low-code automation tools). It built two agents:

- **Mia — the customer-facing agent.** Mia is a multilingual assistant on the website. It answers high-volume customer questions, helps visitors find the right product or plan, and guides them through a purchase. Because it understands natural language, it handles the questions the old menu-based bot could not.
- **Supporto — the internal IT agent.** Supporto is a helper for mobilezone's own staff. Instead of filling out a rigid form, an employee tells Supporto what is broken in plain words, and the agent creates the IT ticket automatically.

The reported results: the agents now handle **more than 1,600 chats a month**, and the internal IT agent **cut IT resolution time by about 50%**. Just as important, the agents reduced the load on mobilezone's external contact center (the outsourced phone support), and the customer agent improved online conversion by guiding shoppers through product discovery.

Two lessons stand out. First, the same technology served two very different jobs — external sales and internal support — which shows how flexible these agents are. Second, mobilezone did not replace humans; it moved the easy, repetitive conversations to the agent so its people could focus on the harder ones. That is the realistic promise: AI handles the volume, humans handle the value.

A note on the source: the figures above come from Microsoft's published customer story on mobilezone. Treat them as mobilezone's reported results; your own numbers will depend on your volume and setup.

## How to Do It

### 26.1 Lead scoring

A *lead* is a person or company that has shown some interest — they filled a form, downloaded something, or asked a question. You do not have time to call every lead with the same effort. Lead scoring means ranking leads by how likely they are to buy, so your team calls the hottest ones first.

**How AI scores a lead.** A machine-learning model looks at many signals at once: the size of the lead's company, the job title of the person, which pages they visited, how many times they came back, whether they opened your emails, and how they found you. From past deals that closed, the model learns which signals go together with a sale, and it scores each new lead accordingly.

**Why it beats guessing.** A person scoring leads by gut feel is slow and biased — they tend to favor the leads that "feel" friendly, not the ones that actually convert. AI scores consistently and fast, and it can weigh hundreds of signals a person cannot hold in their head.

**Start simple.** You do not need a perfect model on day one. Start with a few clear signals — company size, role, and what they downloaded — and score leads by hand in your CRM. As you collect more closed deals, a real model can learn from them and improve.

**Feed the loop.** The model gets better when you tell it which leads actually became customers. Make sure your CRM records the outcome of every deal, so the scoring learns from real results, not guesses.

**Do not over-trust the score.** A score is a hint, not a verdict. A high score means "call soon," not "guaranteed sale." A low score might still be a good customer the model has not learned yet. Use the score to set priority, not to ignore people.

### 26.2 Email and content

Writing emails, ad copy, and product descriptions takes hours. Generative AI — AI that produces text — can draft them fast, and a person can edit them to sound right.

**Draft, do not ship.** Use AI to produce a first draft, then edit it. AI is excellent at getting words on the page quickly and terrible at knowing your exact voice, your brand, and your customer's feelings without guidance. The draft is 70% there; your edit is the last 30% that makes it yours.

**Personalize at scale.** AI can take one template and adapt it for many people: insert the recipient's name, reference what they looked at, tailor the offer to their segment. This is the personalization-at-scale idea from earlier — a message that feels written for one person, sent to thousands.

**Match the channel.** An email, a social post, and a product page need different lengths and tones. Tell the AI the channel and the goal, and edit accordingly. A long email does not work as a tweet; a tweet does not work as a landing page.

**Keep the human voice.** AI text can sound flat, generic, or too eager. Read every draft aloud. If it does not sound like something you would say, rewrite it. Your customers can tell when a message is generic.

**Never let AI send without review.** An unreviewed AI email can contain a wrong price, a wrong name, or an inappropriate line. Always have a human read before it goes out. This is the same rule as in finance: AI drafts, human approves.

**Watch the volume.** AI makes it easy to send more emails than you should. More is not better. Sending too much to people who did not ask is spam, and it burns your list and your reputation. Send less, but make each one count.

### 26.3 Chatbots and assistants

A chatbot is a program that talks with a customer on your website or app. Modern chatbots, built on large language models, understand what a person types and reply in plain language — a huge step up from the old "press 1 for sales" menus.

**What a good chatbot does.** It answers common questions instantly (price, hours, shipping, returns), guides a visitor to the right product, captures contact details for a follow-up, and hands off to a human when it cannot help. The handoff is critical: a chatbot that never hands off frustrates people and loses sales.

**Design the handoff first.** Before you build the bot, decide when it should pass the conversation to a person. When the bot is unsure, when the customer asks for a human, when the topic is sensitive — hand off. A bot that knows its limits is trusted; one that bluffs is not.

**Train on your real questions.** Feed the bot the questions customers actually ask, with the answers you want. The more it knows your specific products and policies, the more useful it is. A generic bot gives generic answers that frustrate.

**Let it speak many languages.** One of the biggest wins of a modern chatbot is multilingual support. It can answer a customer in their own language without you hiring translators. This is exactly what mobilezone's Mia does.

**Measure what it handles and what it fails.** Track how many conversations the bot resolves on its own, how many it hands off, and what it could not answer. The failures are gold — they tell you what to teach it next. (The same chatbot ideas, applied to support rather than sales, are covered in [Chapter 27 — Customer Care and Support](ch27-customer-care-and-support.md).)

### 26.4 Customer analysis

Customer analysis means using data to understand who your customers are, what they want, and who is about to leave. AI is strong here because it can see patterns across thousands of customers that no person could spot by hand.

**Segment your customers.** AI can group customers by behavior: frequent buyers, big spenders, seasonal buyers, at-risk customers. Each group needs a different message. This is segmentation, and AI does it faster and more accurately than manual rules.

**Spot churn before it happens.** *Churn* means a customer stops buying. AI can look at signals — fewer visits, smaller orders, less engagement — and flag customers who are likely to leave soon. That gives you time to win them back with an offer or a personal call, instead of finding out after they are gone.

**Find the next best offer.** AI can look at what a customer bought and suggest what they are likely to want next. "Bought a phone, likely needs a case and insurance." This is the recommendation engine idea, and it lifts the value of each customer.

**Read what customers say.** AI can read reviews, survey comments, and support chats and pull out the main themes: what people love, what annoys them, what they ask for. Instead of reading a thousand comments one by one, you get a summary of the big themes. This turns raw feedback into something you can act on.

**Do not treat people as data points.** Analysis is a tool to serve customers better, not to manipulate them. Use what you learn to make their experience better, not to exploit their weaknesses. The line between personalization and manipulation is real, and you should stay on the right side of it.

## Ethics and Responsibility

Sales and marketing touch people's attention and trust directly, so the ethical line matters.

**Do not spam.** AI makes it easy to send too much. Sending messages to people who did not ask, or more than they agreed to, is spam. Respect consent and frequency. A short list of people who want your messages beats a huge list you blast.

**Be honest in AI-written copy.** AI can write a claim that sounds true but is not. Check every factual claim — price, features, results — before it ships. Never let AI invent a benefit you cannot deliver.

**Disclose when it is a bot.** In many places, and as a matter of good practice, a customer should know they are talking to a chatbot and not a person. Make the handoff to a human easy and clear.

**Respect privacy.** Customer analysis uses personal data. Follow the rules for handling it — the basics are in [Chapter 10 — Privacy and GDPR](ch10-privacy-and-gdpr.md). Collect only what you need, tell people what you collect, and keep it secure.

**Do not manipulate.** Personalization should help people find what they want, not push them into a purchase they will regret. Avoid dark patterns — tricks that pressure people. Build trust, not a trap.

**Keep a human in the loop.** AI drafts the email, the ad, the reply. A human reviews it before it reaches a customer. This single rule prevents most of the damage.

## Mistakes to Avoid

**Spamming with AI.** Using the tool's power to send more than people want. Send less, make it count.

**Shipping unreviewed AI copy.** A wrong price or a false claim in an AI-written email damages trust. Always review.

**A chatbot that never hands off.** A bot that bluffs instead of passing to a human frustrates customers and loses sales. Design the handoff first.

**Generic, flat copy.** AI text that sounds like everyone else's. Edit for your voice or it will be ignored.

**Over-trusting the lead score.** Treating a score as a verdict instead of a hint. Use it to set priority, not to ignore people.

**Garbage data in, garbage analysis out.** If your CRM data is messy, the segments and churn flags are wrong. Clean your data first.

**Treating customers as data points.** Using analysis to manipulate instead of serve. Stay on the ethical side.

**No disclosure of bots.** Letting a chatbot pretend to be human. Be clear.

**Ignoring privacy rules.** Using personal data without consent or security. Follow GDPR basics.

**Confusing activity with results.** Counting emails sent instead of deals closed. Measure outcomes, not volume.

**Skipping the baseline.** Not measuring conversion before, so you cannot prove the lift. Measure first (see Chapter 22).

**Replacing the human touch entirely.** Customers still want a person for hard problems. Keep humans for the value conversations.

## Practical Exercise

### 26.7 Exercise: plan one AI-assisted campaign

Pick one campaign — an email to past customers, a chatbot on your site, or a lead-scoring pass — and plan it end to end.

**Step 1 — Choose the job.** Pick one: lead scoring, an email campaign, a chatbot, or a customer analysis. Do one, not all.

**Step 2 — Define the goal and the metric.** What should this achieve? Signups, replies, resolved questions, won-back customers? Pick one number to measure.

**Step 3 — Measure the baseline.** What is that number now? Write it down. Without it you cannot prove the lift.

**Step 4 — Gather the data.** For scoring: your past leads and which closed. For email: your consented list. For the chatbot: your real customer questions and answers. For analysis: your customer records. Clean the data first.

**Step 5 — Build the AI part.** Score the leads, draft the email, train the bot, or run the segmentation. Let AI do the heavy lifting.

**Step 6 — Add the human review.** Read every draft. Check every factual claim. Decide the chatbot's handoff rules. Nothing ships without a human read.

**Step 7 — Check consent and privacy.** Confirm you are allowed to message these people and that their data is handled correctly.

**Step 8 — Launch small and measure.** Run it on a small group first. Compare the metric to the baseline. If it works, scale up. If not, learn and adjust.

Do one campaign well. The lessons you learn — about tone, about handoffs, about what your customers respond to — carry into every campaign after.

## Checklist

### 26.8 Sales and marketing checklist

Before launching any AI-assisted sales or marketing activity, check these.

- [ ] **You measured the baseline** for the one metric you care about.
- [ ] **A human reviews every AI-written message** before it reaches a customer.
- [ ] **Every factual claim is checked** — price, features, results.
- [ ] **You have consent** to message the people you are messaging.
- [ ] **You respect frequency** — no spam, no over-sending.
- [ ] **The chatbot has clear handoff rules** to a human.
- [ ] **The chatbot is trained on your real questions**, not generic ones.
- [ ] **You disclose that it is a bot** where required and as good practice.
- [ ] **You clean your data** before scoring, segmenting, or analyzing.
- [ ] **You feed outcomes back** into the lead-scoring model so it learns.
- [ ] **You treat the lead score as a hint**, not a verdict.
- [ ] **You use analysis to serve customers**, not to manipulate them.
- [ ] **You follow privacy rules** (GDPR basics, see Chapter 10).
- [ ] **You keep humans for the hard conversations.**
- [ ] **You measure outcomes** (deals, replies, wins), not just volume sent.
- [ ] **You launch small first** and scale only what proves itself.

If a box is empty, you are risking trust. Fill it before you press send.

## Key Takeaways

- AI helps sales and marketing by personalizing at scale — scoring leads, tailoring messages, answering questions, and spotting at-risk customers.
- The mobilezone case (a Microsoft customer story) built two Copilot Studio agents — Mia for customers, Supporto for internal IT — handling 1,600+ chats a month and cutting IT resolution time by about 50%.
- AI drafts, a human reviews: never ship an AI-written message or let a chatbot bluff instead of handing off to a person.
- Clean data is the foundation — messy records make lead scores, segments, and churn flags wrong.
- Use AI to serve customers better, not to spam or manipulate them; consent and honesty protect the trust you are selling on.

<!-- BEGIN agentbridge-examples -->

## Try it with AgentBridge

Here is how the same job looks with AgentBridge. Each box shows the finished result and the one line you type to get it.

### Turn an idea into a proposal

![A structured project proposal document](../../assets/examples/project-proposal.png)
*A structured project proposal document*

**What you ask:** `Create a project proposal for a small online shop: goals, what we deliver, timeline of 8 weeks, and a price of 9,500 euros.`

The agent builds a proposal with the client's goal, your solution, the deliverables, the timeline and the price — all in a clean layout that looks like it took a whole afternoon. It took a minute.

*Tip: Add your logo and a sentence about past results to make it feel personal.*

---

### Track your sales

![A sales tracker with revenue by channel](../../assets/examples/sales-tracker.png)
*A sales tracker with revenue by channel*

**What you ask:** `Create a sales tracker with month, channel and revenue, and a chart of revenue by channel.`

The agent builds the tracker and the chart. Add rows as you go, or attach your raw sales list and ask it to fill the sheet for you.

*Tip: Attach a messy export from your shop and say 'clean this into a tracker' — it will.*

---

### A pitch deck from one prompt

![A presentation slide built by the agent](../../assets/examples/pitch-deck.png)
*A presentation slide built by the agent*

**What you ask:** `Make a 6-slide pitch deck for my delivery startup: problem, solution, market, model, traction, ask.`

The agent designs the slides with a clean look, one clear idea per slide, and the right order for a pitch. In the browser you press F11 for full screen and present.

*Tip: Need a real .pptx to send? Use /tools office-files and ask for PowerPoint.*

---

### A client sales deck

![A client-facing sales presentation slide](../../assets/examples/sales-presentation.png)
*A client-facing sales presentation slide*

**What you ask:** `Create a sales deck summarising our work with Acme and proposing the next phase.`

The agent builds a focused deck: results so far, what the client gained, and the proposed next step. You tweak the numbers and present with confidence.

*Tip: Attach the project report and the agent pulls the highlights into the slides.*

---

### A polite follow-up

![A friendly follow-up email draft](../../assets/examples/follow-up.png)
*A friendly follow-up email draft*

**What you ask:** `Write a short follow-up to a client who has not replied to our quote from last week.`

The agent writes a light, polite nudge that reminds without pressure. You send it and keep the relationship warm.

*Tip: A scheduled follow-up can send these for you if a reply has not arrived.*

---

### A customer newsletter

![A newsletter draft ready to send](../../assets/examples/newsletter.png)
*A newsletter draft ready to send*

**What you ask:** `Write a monthly newsletter for our customers: new items, a tip, and a small discount code.`

The agent writes the newsletter in your voice with the news, a useful tip and the offer. Send it, or let it prepare one on a schedule.

*Tip: A monthly scheduled task can draft the newsletter for your review each time.*

---

### Turn a topic into a podcast

![A podcast episode ready to play](../../assets/examples/podcast-episode.png)
*A podcast episode ready to play*

**What you ask:** `Create a 5-minute podcast episode about why small shops should go online, in a friendly two-voice style.`

The agent writes the script and produces an audio episode with two voices, ready to publish. Your message, in audio form, with no studio.

*Tip: Give it your key points and it shapes them into a natural conversation.*

<!-- END agentbridge-examples -->
