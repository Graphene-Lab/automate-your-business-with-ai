# Chapter 7 — Trustless: Trust Without Trusting

## In Simple Words

The word "trustless" is badly chosen. It sounds like a world with no trust, where nobody believes anything. That is not what it means, and the real idea is much more useful.

Trustless means: **you do not have to trust a person or an institution, because you can verify the fact yourself.**

Start with a familiar contrast. You hire a removal company. You hand over a deposit. You now depend on them showing up. You must trust them, or trust their brand, or trust the law to punish them if they do not. Now think of a vending machine. You put in coins, the drink falls out. There is no relationship, no promise, and no need to believe anyone. The machine enforces the deal by how it is built. That is the feeling of trustless: the agreement is enforced by a system instead of by a person's good intentions.

Three tools make this possible.

**Verification instead of promises.** Instead of someone telling you a thing is true, you check it. A digital signature is the common example. It proves that a file came from whoever holds a particular key, and that the file has not changed since it was signed. You do not need to trust the sender. You check the signature.

**Transparency instead of secrecy.** Instead of keeping a record in one private notebook, you keep it somewhere many people can read and nobody can quietly rewrite. If everyone can see the record, one party cannot change history to suit itself.

**Automatic enforcement instead of hope.** Instead of agreeing terms and hoping they are met, you write the terms so a piece of software carries them out. Money is released when the condition is met. Nobody has to chase an invoice.

Now the honest warning, said early: trustless does not mean risk-free. You have moved your trust from people to systems, and systems are built by people. Code has bugs. The feeds that tell a system what happened in the real world can be wrong or lied to. Keys get lost, and a lost key can mean lost money. The goal is not to remove trust. It is to place trust somewhere you can inspect, and to reduce how much of it you need.

Why bother at all? Because trust is expensive. Every intermediary you rely on — a bank, an escrow agent, a broker, a notary, a platform that holds funds until the job is done — takes a cut and takes time. Trustless systems remove some of that, and make what is left cheaper, faster, and visible. This is not only for banks and programmers; it has direct use in any company that buys from suppliers, hires freelancers, and needs records its accountant can trust.

The wider question of who controls your digital tools is in [Chapter 11](ch11-digital-sovereignty.md). Whether it pays back is a [Chapter 16](ch16-goals-costs-and-return-on-investment.md) question. The security side of verification is in [Chapter 6](ch06-cybersecurity-in-the-ai-era.md).

## A Bit of History

**2008.** In October a paper titled "Bitcoin: A Peer-to-Peer Electronic Cash System" was published under the name Satoshi Nakamoto. Its stated aim was electronic payment without trusted third parties. The trick was a shared, ordered record — a blockchain — kept together by many independent computers, so that no single one of them can rewrite it.

**2009.** The Bitcoin network began running in January. For the first time, two strangers could settle value with no bank in the middle, and neither had to trust the other.

**2015.** Ethereum arrived and added the key upgrade: smart contracts. A smart contract is a program stored on the network that runs exactly as written when its conditions are met. Money could now be tied to a rule.

**2016.** A project called The DAO held funds in a smart contract and was drained because of a flaw in that contract. The fallout split the community. The lesson was sharp and still true: automatic enforcement enforces bugs with the same loyalty it enforces features.

**2017 to 2021.** Decentralised finance grew into a real sector: lending, trading, and settlement run by contracts instead of banks, with stablecoins — tokens meant to hold a steady value — as its working money. It also showed the same failures at a larger scale: bad code, wrong price feeds, dishonest operators. In **2019** the W3C, the body that sets web standards, published Verifiable Credentials: a way for an authority to issue a digital claim — a degree, a licence, an age proof — that anyone can check without telephoning the issuer. That is the identity half of the picture.

**2021 to 2023.** A standard called ERC-4337, known as account abstraction, was proposed in 2021 and later finalised. It lets an account be a small program instead of a single private key, so the account can hold its own rules: spending limits, a list of allowed payees, a second signature for large amounts, and recovery if a key is lost.

**May 2025.** An Ethereum upgrade called Pectra went live on the main network. It let an ordinary wallet address point to smart-contract code, bringing transaction batching, sponsored fees, and better recovery to addresses that previously had none. It also raised the maximum stake a single validator can hold.

**August 2025.** A draft standard called ERC-8004 appeared, titled "Trustless Agents." It was written for the problem this chapter is really about: software agents that deal with other people's agents.

Read the timeline as one long argument. Each step moved enforcement out of a person's hands and into a checkable system: first money, then agreements, then identity, then permissions, and most recently agents.

## Curiosity

### 7.6 Ethereum is building plumbing for an agent economy

In August 2025 a draft standard called **ERC-8004** was published on Ethereum's official standards site. Its title is "Trustless Agents," and its stated purpose is to let software agents discover, choose, and work with other agents across organisational boundaries without any prior trust.

It defines three registers, all on-chain.

**Identity.** Each agent gets an on-chain identifier, built on the common ERC-721 token standard, that points to a registration file. That file holds the agent's metadata, the addresses you can talk to, and which trust models it supports. In plain terms: an agent can say who it is, who it acts for, and how you can check it, and you can look that up instead of taking its word.

**Reputation.** A standard way to post and read feedback about an agent, so that performance history is not locked inside one platform's private star rating. Anyone can contribute signals, and the aggregation can happen off-chain. The point is portability: an agent's record follows it, instead of being reset every time it changes marketplace.

**Validation.** Hooks for getting independent checking of an agent's work. The standard lists several methods: having another party re-run the job with money at stake, using zero-knowledge machine-learning proofs — a way of proving a computation was done correctly without revealing the data or the model behind it — using trusted hardware enclaves, or using a trusted human judge.

Why should a small business owner care about a draft standard? It shows where the industry thinks the hard problem is: not "can an agent do the task" but "how do I know whether to believe this agent" — a business question, not a technical one. If it succeeds, you will be able to check a public record instead of trusting a sales deck, which changes who holds the power in the conversation. And the same three questions are a useful checklist today, with no blockchain at all: *Who are you, and who do you act for? How have you behaved before? Can your work be checked independently?*

Two other pieces of the same plumbing are already live. Account abstraction, the ERC-4337 standard, means an agent can hold a budget with rules enforced by code: a hard spending cap, a whitelist of allowed payees, a second human signature above a threshold. And since the Pectra upgrade in May 2025, an ordinary address can point to such code. That combination — an agent that can pay, inside a box it cannot leave — is the practical shape of a trustless agent economy.

Treat all of this as direction, not as a product to buy this quarter. ERC-8004 is a draft. The concepts, however, are usable now.

## A Real Business Example

### The mango that took seven days to trace, then two seconds

In 2017 Walmart and IBM ran a pilot in food supply chains, and the numbers they published became famous in the industry. Tracing the origin of a mango sourced in Central or South America used to take about seven days of phone calls, emails, and paper chasing. With the records held on a shared ledger, the same trace took about 2.2 seconds. IBM described it as complete end-to-end traceability. A parallel pilot tracked pork in China.

Two honest notes. The figure came from a controlled pilot, not a full live rollout, and the 2.2 seconds is the time to query the record, not the time to fix a contaminated shipment.

Now look at what changed. Before, each party kept its own notebook: the farm wrote the harvest date, the packer the batch, the shipper the container, the store the delivery. To answer one question you had to ask four companies to search their private notebooks and hope they answered quickly and honestly. After, everyone wrote into the same record as they went. Nobody could quietly rewrite their page, and "where did this come from" became a lookup instead of a negotiation.

That is the trustless value in one sentence: **you replaced a chain of promises with one shared record you can read.**

It also shows the limit, which matters more than the win. A shared record proves what was written down. It does not prove the writing was true. If a supplier enters a false farm or a false date, the ledger preserves the lie perfectly. The weak link is the moment a human or a sensor puts a fact into the system. Any trustless project that ignores that moment is decoration.

## How to Do It

### 7.3 How it works in practice: verifiable identity, reputation, programmable payments

You do not need a cryptocurrency to use trustless thinking. Four building blocks apply to ordinary business.

**Block 1: Verifiable identity.**
The question is: is this really who it claims to be, and can I check without phoning anyone? Digital certificates and digital signatures already answer this for you every day. When a supplier sends a document signed with a recognised digital signature, you can verify both who signed it and that nothing changed afterwards. A verifiable credential goes further: your accountant can prove they hold a current licence, or a staff member can prove they passed a background check, without handing over the whole certificate and without you calling the issuing body.

**Block 2: Tamper-evident records.**
The question is: can anyone quietly rewrite history? A shared ledger is one answer. So is a simpler trick called a hash — a short fingerprint computed from a file. If you record the fingerprint of a document at the moment you agree it, and the file is later changed, the fingerprint will not match. You can produce that fingerprint later and prove the state of the document then. This costs almost nothing and needs no special permission.

**Block 3: Programmable payments.**
The question is: can the money move by itself when the condition is met? Escrow is the old version: a third party holds funds and releases them on a trigger. The newer version writes the trigger into code, so no human decision is needed at release time. Milestone payment for a freelancer is the obvious case: payment is released when the deliverable is accepted, and the acceptance rule is written down in advance.

**Block 4: Auditability.**
The question is: after the fact, can we both see the same truth? Every action should leave a timestamped, ordered, non-editable record. When both sides read the same record, arguments get short. Your accountant, your auditor, and your customer can all check the same thing without asking you for a favour.

**How to start small, today:**

1. Pick one process where you currently chase confirmation.
2. Write the release condition as a single testable sentence. If you cannot write it as a testable sentence, the process is not ready.
3. Ask whether a machine can measure the trigger. Delivered means a scanned signed delivery note. Approved means a click on an approval button. Completed means a status change in your own system.
4. Put the money behind a rule that waits for that measurement: an escrow service, a payment schedule in your accounting system, or a workflow that requires the trigger before release.
5. Log every step where both sides can see it.
6. Only then automate.

### 7.4 AI agents interacting with each other: the future of automated business

The interesting version of this is near. Your software agent talks to a supplier's software agent, and they settle a transaction without a human on each step.

For that to work safely, five things must exist.

**Identity and authority.** Not only "this is supplier X's agent," but "this agent is authorised to commit up to 500 units at a price below 4.20 each." Authority must be provable and bounded, not assumed.

**A machine-readable deal.** Both sides need the terms in a structured form — quantity, price, delivery date, penalty — not a friendly email thread. A human can forgive ambiguity. An automated system will either stall on it or exploit it.

**A payment rail that can wait.** The payment must be conditional: held, then released on evidence. An instant, unconditional payment removes all leverage and all reason to perform.

**Evidence.** A delivery confirmation, an acceptance record, a signed receipt, in a form both systems can read and neither can quietly alter.

**A dispute path.** Something must handle the case where the two agents disagree, or where the world did not go as the rule assumed. With no escalation route, a small disagreement becomes a stuck payment and an angry supplier.

What is realistic now: agents can already search, compare, draft quotes, and prepare orders. What is not yet routine is letting them commit money and legal terms on their own. The sensible path is a human approving the final commitment while the agent prepares everything. That keeps the speed and drops the risk.

### 7.5 What it means for your company: smart contracts, automatic payments, auditability

**Smart contracts, in plain words.** A smart contract is a program that holds an agreement and carries it out when the stated condition happens. It is not clever and it is not a contract in the lawyer's sense. It is a very literal vending machine. Write the rule carefully and it is a great servant. Write it loosely and it is a great servant too — to whatever you actually wrote.

**Automatic payments.** The practical form is a payment that waits. It waits for a delivery confirmation, an approval click, a milestone accepted, a date reached. Each one is capped, logged, and visible to both sides before it moves.

**Auditability.** Every step leaves a record. Your accountant closes the month faster because there is nothing to reconstruct. A customer dispute ends in minutes because both sides look at the same line. If a regulator asks, you produce the record instead of a story.

**Where it fits well:** cross-border supplier payments where enforcement is slow; freelancer and contractor milestones; marketplaces where buyer and seller are strangers; data-sharing agreements where you must prove what you released and when; insurance that pays on a measured event, such as a flight delay.

**Where it fits badly:** anything that needs judgement, negotiation, or a relationship. Anything where the trigger cannot be measured honestly. Anything where a wrong automatic payment is hard to recover.

## Ethics and Responsibility

Trustless systems change who is accountable, which is exactly why they need careful thought.

**Code that enforces also enforces mistakes.** If your rule releases payment on a condition that is easy to fake, you have automated a loss. Write the rule for the dishonest case, not only for the efficient one.

**Oracles are people.** A "machine-measurable trigger" often depends on a human entering data somewhere. The weakest link in a trustless chain is the moment a person types the truth into it. Design for that person being rushed, mistaken, or bribed.

**Immutability collides with privacy.** Putting personal data on a permanent, unchangeable record can conflict with data-protection rights, including the right to erasure. Keep personal data off public ledgers; store only references and fingerprints. The legal detail is in [Chapter 10](ch10-privacy-and-gdpr.md).

**Do not remove the human from a human problem.** Unhappy customers do not want a perfectly enforced rule; they want someone to listen. Trustless is for the boring middle of a transaction, not for the moment someone is upset.

**Be transparent, and keep a named owner.** Tell the people whose work is now measured by the system, and explain how a decision can be overturned; a rule no one may question will eventually be wrong with nobody able to fix it. Automatic enforcement does not remove responsibility — someone in your company must still own the outcome, as [Chapter 4](ch04-ethical-ai-doing-the-right-thing.md) sets out.

## Mistakes to Avoid

### 7.7 Not everything needs to be trustless

1. **Using a blockchain where a spreadsheet would do.** If the parties trust each other, the record is small, and a normal contract works, a distributed ledger adds cost and complexity for nothing.
2. **Confusing trustless with risk-free.** Code has bugs, feeds can be wrong, keys can be lost, and there is often no support number to call.
3. **Automating a bad process.** A trustless system will enforce your bad process faster and more consistently than a person ever did.
4. **Putting personal data on a public chain.** It cannot be deleted later.
5. **No kill switch.** Any automated payment system needs a way to stop it in one click.
6. **No spending cap.** An agent with an open wallet is an open chequebook.
7. **Trusting the trigger too much.** Ask how the trigger could be faked, then decide whether that matters.
8. **Chasing a pitch.** "Trustless" is a useful design idea, not a reason to buy a token. If a proposal cannot explain the trigger, the record, and the dispute path, it is marketing.
9. **Cutting out every intermediary.** Some intermediaries earn their fee. A notary, a customs agent, or an insurer may be doing real work that code cannot do.
10. **Forgetting who is accountable.** Even with automatic enforcement, a named human must own the result.

## Practical Exercise

### 7.8 Think of a business process that could benefit from trustless automation

Pick one process where you currently spend time checking, chasing, or arguing. Work through these nine questions in writing.

1. **Who are the parties?** Name them. Note whether they already trust each other.
2. **What must be true before money moves?** One sentence.
3. **Who verifies that today?** A person? How long does it take? How often is it wrong?
4. **What does that verification cost?** Time, fees, delays. Rough numbers are fine; mark them as rough.
5. **Can a machine measure the trigger?** If yes, what is the signal? If no, can the process be redesigned so it can?
6. **What is the evidence trail?** What record exists, where, and can either side change it?
7. **What happens in a dispute?** Who decides, and how fast?
8. **What is the worst way this could be abused?** Write the dishonest scenario before the efficient one.
9. **What is the cap?** The maximum loss if the rule is wrong.

Now score it. If the verification cost is a large share of the transaction value, the trigger is machine-measurable, and you can set a low maximum loss, the process is a strong candidate. If the trigger cannot be measured by a machine, or the maximum loss is high, keep a human in it.

Write one page. Bring one candidate to your next meeting.

## Checklist

### 7.9 When to consider a trustless approach

- [ ] **You pay an intermediary mainly to hold or check something**, and that check could be written as a rule.
- [ ] **The parties do not already trust each other**, and building trust would be slow or impossible.
- [ ] **The release condition can be stated as one testable sentence** that a machine can measure.
- [ ] **The transaction happens often**, so the setup cost is spread across many uses.
- [ ] **It is cross-border or cross-company**, where local enforcement is slow or unclear.
- [ ] **You need a shared, non-editable record** that both sides and your auditor can read.
- [ ] **You can set a hard spending cap** and a one-click stop before automating.
- [ ] **No personal data needs to sit on the permanent record.**
- [ ] **A dispute path exists** and names a human who can override the rule.
- [ ] **You have compared it honestly** with a normal contract and a normal process, and trustless still wins on cost, speed, or risk.

## Key Takeaways

- Trustless does not mean no trust; it means you verify a fact instead of trusting a person to tell it.
- The three working parts are verifiable identity, tamper-evident records, and automatic enforcement of a written condition.
- Ethereum's draft ERC-8004 and the account-abstraction standards show where agent-to-agent business is heading: identity, reputation, and independent validation, with budgets bounded by code.
- The weakest link is the trigger — the moment a human or a sensor tells the system what really happened.
- Do not use trustless where a normal contract works; use it where verification is expensive, the trigger is measurable, and the maximum loss is capped.
