# Chapter 34 — Services and Consulting

*This chapter is a representative composite. It is not one real firm. It combines the common patterns we see in consulting and professional-services firms that adopt AI. All numbers are illustrative — they show the shape of the decision, not a promise. Replace them with your own.*

## Context

Picture a mid-sized consulting firm. We will call it **Northbeam Advisory**. It has about twenty-five consultants and a small support team. It does not sell a product. It sells expertise and time. A client — usually another company — has a problem, and Northbeam sends people to solve it: a strategy project here, an operations review there, a data study somewhere else.

Every project follows the same rough path. First comes the **pitch**: a proposal that says what the firm understands, what it will do, and what it will cost. If the client agrees, the team does the work. During the work, the client gets regular **status reports**. At the end, there is a final deliverable and an invoice. Between all of this sits a mountain of coordination: finding the right people for the job, booking meetings, writing up what was said, and keeping track of who is free when.

For years, all of this ran on people. A partner writes a proposal by opening an old one and rewriting it. A consultant solves a problem that the firm solved three years ago, but nobody remembers where, so they solve it from scratch. A project manager builds each status report by hand, copying numbers from one file into a slide. Someone spends half a day matching consultant calendars to project needs. The firm is successful. But it spends a great deal of expensive, trained time on work that is repetitive, and it keeps losing knowledge it already paid for once.

A consulting firm is like a professional practice in one important way. Everything it touches is **confidential**. A client's strategy, a cost model, a merger plan — these are shared in trust. That single fact shapes how AI can be used here, just as it does for a law firm. It is the thread running through this chapter.

## The Problem

The firm's leaks are easy to name.

**Proposals are slow.** Every new pitch starts close to a blank page. The firm has written hundreds of proposals and has good material in them, but finding the right past example, the right case study, the right pricing structure, takes time. A partner might spend two full days on a proposal that is mostly reassembly. Slow proposals also mean missed chances — some deals are lost simply because the response came too late.

**Knowledge walks out the door.** When a consultant leaves, the know-how in their head leaves with them. A method they refined, a client quirk they learned, a fix they worked out — unless someone wrote it down, it is gone. So the firm pays to solve the same problems again and again. This is the most expensive leak, because it is invisible.

**Reporting is manual.** A status report is mostly the same each week: what moved, what is late, what is next. But a person assembles it by hand every time, pulling numbers from project files and writing the same kind of narrative. It is reliable and it is dull, and it eats hours that could be billable.

**Coordination overhead.** Matching the right consultant's skills to a project, checking who is free, booking meetings, and writing up the notes afterward is a constant tax. Meetings happen, but nobody wants to write the minutes, so decisions get fuzzy and someone has to redo the conversation later.

If you want to see how these rank against the rest of your firm, the impact-and-effort method in [Chapter 12 — Where AI Can Help Your Business](ch12-where-ai-can-help-your-business.md) is the place to score them.

Over all four sits confidentiality. Any tool that reads a client's proposal or project file must be a tool the firm can trust not to leak it. That question comes first.

## The Solution

Northbeam attacks the four leaks in order of safety, not just size. The rule is the same one a law firm uses: start where a mistake is cheap and the data is not the most sensitive, and move toward the sensitive work only when the tooling is trustworthy.

**A proposal assistant that drafts from the firm's own history.** When a new pitch arrives, a consultant writes a short brief — the client, the problem, the rough scope. An AI assistant searches the firm's past proposals and pulls the most relevant sections, then drafts a first version: an understanding of the problem, a suggested approach, a case study that fits. The partner no longer starts cold. They edit a draft instead of building from nothing. Two days becomes a few hours. This is the same "machine drafts, human reviews" pattern that the Elanco case shows in [Chapter 25 — Administration and Finance](ch25-administration-and-finance.md).

**A searchable memory for the firm.** The firm puts its past deliverables, methods, and notes into an internal search that consultants can ask in plain language. This is often called a **knowledge base with AI search**. Under the hood it uses a technique called **retrieval-augmented generation**, or RAG. In plain words: instead of asking a general AI a question, the system first looks up the firm's own documents, then answers using only what it found there. So when a consultant asks, "How did we handle a supplier-risk review for a retail client?" the system finds the real past project and answers from it. The knowledge stops walking out the door. The chatbot and search technology behind this is covered in [Chapter 27 — Customer Care and Support](ch27-customer-care-and-support.md).

**Reporting that drafts itself.** The status-report tool connects to the project's data — tasks, dates, milestones — and drafts the weekly report: what moved, what slipped, what is next. The project manager reviews it, adds the human judgment about tone and what to emphasize, and sends it. The blank page is gone.

**Scheduling and meeting summaries.** A scheduling assistant matches consultant skills and availability to project needs and proposes who should work on what. For meetings, a tool records the call, drafts the minutes, and lists the decisions and action items. A person checks it before it circulates. Decisions stop being fuzzy because the write-up happens automatically.

In every case, the human stays in charge. In consulting, the client is paying for judgment and accountability. The AI drafts, searches, and summarizes. The consultant decides, tailors, and stands behind the work.

## The Tools

The tools are ordinary, but the way they are deployed is shaped by confidentiality.

- **A proposal assistant** that searches the firm's past proposals and drafts a new one from a brief.
- **An internal knowledge search** (RAG) over the firm's deliverables and notes, so consultants can ask questions in plain language and get answers grounded in the firm's own work.
- **A reporting assistant** that connects to project data and drafts status reports.
- **A scheduling assistant** for matching people to projects, plus a **meeting-summary tool** that turns a recorded call into draft minutes.

How to pick these tools without being dazzled by a demo is covered in [Chapter 17 — Choosing Tools Without Being Fooled](ch17-choosing-tools-without-being-fooled.md). How to connect them to the firm's existing project-management and document systems is in [Chapter 19 — Connecting AI to Systems You Already Use](ch19-connecting-ai-to-systems-you-already-use.md).

**Confidentiality comes first.** A general chatbot that you paste a client proposal into may store it, train on it, or expose it. For a consulting firm, that can break a client's trust and a contractual duty of secrecy. The firm must use tools that keep client data private — either a business-grade service with a clear no-training, no-sharing contract, or a model run on the firm's own machines. Self-hosting is explained in [Chapter 8 — Self-Hosting: Keep Your Data Under Control](ch08-self-hosting-keep-your-data-under-control.md). The danger of staff quietly pasting client data into public tools — shadow AI — is the subject of [Chapter 9 — Third-Party Services and Shadow AI](ch09-third-party-services-and-shadow-ai.md). And because client files and contact lists hold personal data, the privacy rules of [Chapter 10 — Privacy and GDPR](ch10-privacy-and-gdpr.md) apply in full.

## The Costs

Here is an illustrative first-year budget for a firm like Northbeam. These are made-up numbers to show the shape. Use your own.

**Direct costs.**
- Proposal assistant (business-grade, with a confidentiality contract): about €12,000 a year.
- Internal knowledge search (RAG platform): about €9,000 a year.
- Reporting assistant: about €4,800 a year.
- Scheduling and meeting-summary tools: about €6,000 a year.
- Setup and integration with the project-management and document systems: about €12,000 one-time.
- Training the consultants and support staff: about €5,000 one-time.

First-year total: roughly **€48,800**. In steady years after, the recurring subscriptions come to about **€31,800**.

**Indirect costs.**
- Consultants spend time reviewing every AI draft. This is the cost of the safety net, and it must stay.
- The learning dip while everyone adapts.
- The cost of curating the knowledge base. A search is only as good as what you put in it, and someone must keep it clean and current.
- Time spent vetting each tool for confidentiality and compliance before use.
- The cost of a mistake if a draft is trusted without checking — in consulting, a wrong number in a client report can cost far more than a subscription.

The full method for counting these costs and turning the savings into a return figure is in [Chapter 16 — Goals, Costs, and Return on Investment](ch16-goals-costs-and-return-on-investment.md). Do not run the math in your head. Write it down.

## The Results

After a year, measured against a baseline the firm recorded before starting, the illustrative outcome looks like this. Your numbers will differ. These show what a good fit can look like.

- **Proposals got faster.** A pitch that took two days now takes a few hours, because the partner edits a draft instead of building from a blank page. The firm also responds sooner, which wins some deals it would have missed.
- **Knowledge stayed.** When consultants left, their know-how stayed in the searchable base. The firm solved fewer problems twice.
- **Reporting time fell.** The weekly status report became a review of a draft, not a manual build, freeing hours across the project managers.
- **Meetings produced records.** Decisions and action items were written up automatically, so fewer conversations had to be repeated.
- **More billable time.** With less time spent on reassembly and search, consultants spent more of their day on work the client pays for.

The honest caveat: none of this was instant. The proposal assistant produced rough drafts at first until it had enough good past proposals to learn the firm's style. The knowledge search gave weak answers until the documents were organized and tagged. The meeting-summary tool mislabeled speakers early on. The gains ramped up over weeks, as the learning-curve warning in [Chapter 16](ch16-goals-costs-and-return-on-investment.md) predicts. The firm measured the real numbers after the ramp, not during it.

## Lessons Learned

**Confidentiality is the first constraint, not an afterthought.** In consulting, the question is never only "does this tool work?" It is "can this tool be trusted with a client's private file?" Answer that before anything else. Use business-grade tools with a clear no-training contract, or self-host. See [Chapter 8](ch08-self-hosting-keep-your-data-under-control.md) and [Chapter 9](ch09-third-party-services-and-shadow-ai.md).

**The AI drafts; the consultant advises.** A consultant's value is judgment and accountability. The AI shortlists, drafts, and summarizes; the consultant decides and signs. Never let a draft become client-facing work without a human mind on it.

**A knowledge base is a garden, not a dump.** AI search is only as good as the documents behind it. If you throw in messy, outdated, or wrong files, you get confident wrong answers. Someone must own the base, keep it current, and control who can see what. Access control matters: a consultant on one client's project should not be able to search up another client's confidential material. The data-readiness principle is in [Chapter 14 — Data: The Raw Material](ch14-data-the-raw-material.md).

**Recording meetings needs consent.** A meeting-summary tool works by recording the call. Recording a conversation is personal-data processing, and people must know and agree. Tell participants before you record, and follow the rules in [Chapter 10 — Privacy and GDPR](ch10-privacy-and-gdpr.md). Do not record quietly.

**Beware the confident wrong answer.** These tools can produce text that sounds right and is wrong — a case study that never happened, a number that does not add up. In consulting, a fabricated figure in a client report is a disaster. Verify every number and every claim against the real source. The reliability problem is covered in [Chapter 2 — AI Explained Simply](ch02-ai-explained-simply.md), and the duty to be honest about what AI can and cannot do is in [Chapter 4 — Ethical AI: Doing the Right Thing](ch04-ethical-ai-doing-the-right-thing.md).

**Start with the safe work.** Northbeam began with internal search and reporting drafts — low risk, not yet the most sensitive client proposals. It moved toward proposal drafting only once the tooling was trusted. This is the "high ease first" rule from [Chapter 12](ch12-where-ai-can-help-your-business.md).

**Measure honestly and expect the ramp.** Record the baseline before you start. Judge the project after the learning curve, not during it. The method is in [Chapter 22 — Measuring Results and ROI](ch22-measuring-results-and-roi.md).

The consulting firm's lesson is the same as every other sector's, with one extra guardrail: find the repetitive work — proposals, search, reporting, coordination — let AI draft and retrieve, keep a human on the judgment and the client relationship, and measure honestly. And in a firm built on trust, never let the tool touch a client's confidential file until you are certain it is safe to.
