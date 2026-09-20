# Chapter 35 — Healthcare, Education, and Public Bodies

*This chapter is a representative composite. It is not one real organization. It combines the common patterns we see in small clinics, schools, and public offices that adopt AI for administration. All numbers are illustrative — they show the shape of the decision, not a promise. Replace them with your own. The rules for regulated data are set out in [Chapter 10 — Privacy and GDPR](ch10-privacy-and-gdpr.md) and [Chapter 5 — Rules and Legal Responsibility](ch05-rules-and-legal-responsibility.md); this chapter shows how those rules play out in practice.*

## Context

Picture a small community medical clinic. We will call it **Riverside Family Clinic**. It has four general practitioners, two nurses, and a front desk with three administrative staff. It serves a few thousand patients in a town.

The clinic's day is run at the front desk. The phone rings constantly. People call to book an appointment, to move one, to ask what to bring, to ask about a referral, to ask when a result is ready. The three admin staff spend most of their day on the phone and on paper. Referral letters arrive by post and must be read, filed, and routed to the right doctor. Forms must be checked before a patient is seen. Meanwhile, the doctors finish each visit and then spend time writing up the notes — a task that piles up until some of it is done late at night.

Now picture two more places with the same shape. A **primary school** where the office answers the same questions from parents every day, handles admissions paperwork, and juggles timetables. A **local council office** where staff process citizen applications — a permit, a benefit claim, a registration — each one a stack of forms and documents that must be read, checked, and moved along.

Three different places. The same pattern: a small team buried under scheduling, documents, and repeated questions, while the trained people — doctors, teachers, caseworkers — spend time on paperwork instead of the work they were trained for.

What makes these three special is the data. A clinic holds **health data**. A school holds data about children. A public office holds data about citizens and their entitlements. These are not ordinary records. They are among the most protected kinds of personal data. That single fact sets a higher bar for everything in this chapter.

## The Problem

The leaks are the familiar ones, but the cost of getting it wrong is higher.

**Front-desk overload.** The phone queue is the clinic's bottleneck. Staff spend hours on repeated questions — opening hours, what to bring, how to reschedule — while real urgent calls wait. Long waits frustrate patients and burn out the staff.

**No-shows.** When patients forget an appointment, the slot is wasted and someone else could have had it. In a busy clinic, a high no-show rate means real patients wait longer for care.

**Documentation burden.** After each visit, the doctor writes notes. This is necessary and it is heavy. Clinicians everywhere report spending a large share of their day on records rather than patients. It is a known driver of stress and burnout. The work is careful but repetitive.

**Document handling.** Referral letters, forms, and results arrive in many formats. Someone must read each one, pull out the key facts, file it, and route it to the right person. Miss a document and a patient waits.

**Repetitive questions for citizens and parents.** In the school and the council office, the same questions come in over and over, in many languages, and the answer is always the same. Answering them is simple but it consumes the office.

Over all of this sits the rule that this data is **special category** data. Under the GDPR, health data and data about children get extra protection. The EU AI Act adds more: systems used in medical devices or in ways that affect people's rights are treated as higher risk and carry heavier duties. The details live in [Chapter 10](ch10-privacy-and-gdpr.md) and [Chapter 5](ch05-rules-and-legal-responsibility.md). The point here is simple: in these settings, privacy and compliance are not a box to tick at the end. They shape every choice from the start.

## The Solution

Riverside attacks the admin load in order of safety. The rule is the same as in a law firm: start where a mistake is cheap and the data is least sensitive, and move toward the sensitive work only when the tooling is trustworthy. And in a clinic, the most sensitive work — clinical judgment — is never automated at all.

**AI scheduling and reminders.** A chatbot on the website and a phone system handle routine bookings: book, move, cancel. They answer the repeated questions instantly. Automated reminders go out before each appointment, which cuts no-shows. The front-desk staff are freed for the calls that need a human — a worried patient, a complex case. The chatbot technology is the same as in [Chapter 27 — Customer Care and Support](ch27-customer-care-and-support.md).

**Ambient documentation that drafts, the doctor signs.** For a visit, a tool listens to the conversation (with the patient's clear consent) and drafts the clinical note afterward. The doctor reviews it, corrects anything wrong, and signs it. The doctor is fully responsible for the note; the tool only removes the typing. This is the same "machine drafts, human reviews" pattern that the Elanco case shows in [Chapter 25 — Administration and Finance](ch25-administration-and-finance.md). The tool does not diagnose. It writes down what was said so the doctor can check it.

**Document routing.** A tool reads incoming referral letters and forms, extracts the key facts — the patient, the request, the urgency — and files and routes them. A person still checks the pile, but the sorting is done, so nothing sits unread.

**A questions assistant for citizens and parents.** In the school and the council office, a chatbot answers the repeated questions in plain language and in several languages, at any hour. A parent asking "what documents do I need for admissions?" or a citizen asking "how do I apply for this permit?" gets an instant answer. The office staff handle only the questions the bot cannot.

Notice the line that never moves. The AI books, reminds, drafts, extracts, and answers. A doctor signs the clinical note. A caseworker decides on an application. A teacher makes the educational call. In these settings, the AI touches the admin around the decision, never the decision itself.

## The Tools

The tools are ordinary, but they are deployed under a much stricter set of rules.

- **A scheduling and reminder system** with a chatbot and phone handling for routine bookings.
- **An ambient documentation tool** that drafts visit notes from a recorded conversation, for the clinician to review and sign.
- **A document-extraction tool** that reads letters and forms and routes them.
- **A questions chatbot** for parents and citizens, working in multiple languages.

How to pick these tools without being dazzled by a demo is covered in [Chapter 17 — Choosing Tools Without Being Fooled](ch17-choosing-tools-without-being-fooled.md). How to connect them to the clinic's patient system or the office's case system is in [Chapter 19 — Connecting AI to Systems You Already Use](ch19-connecting-ai-to-systems-you-already-use.md).

**The compliance bar is the whole story here.** Health data and children's data cannot be pasted into a public chatbot. These organizations must use tools that keep the data protected: a business-grade service with a clear no-training, no-sharing contract and a data-processing agreement, or a model run on their own machines or in a controlled, in-region cloud. Self-hosting is explained in [Chapter 8 — Self-Hosting: Keep Your Data Under Control](ch08-self-hosting-keep-your-data-under-control.md). The danger of staff quietly pasting sensitive data into public tools — shadow AI — is the subject of [Chapter 9 — Third-Party Services and Shadow AI](ch09-third-party-services-and-shadow-ai.md). Keeping the data within the country or region, rather than abroad, is the sovereignty question in [Chapter 11 — Digital Sovereignty](ch11-digital-sovereignty.md). And the legal duties for this category of data are set out in [Chapter 10](ch10-privacy-and-gdpr.md) and [Chapter 5](ch05-rules-and-legal-responsibility.md).

Two practical rules follow. First, **data minimization**: collect and process only what is needed. A scheduling bot does not need a patient's full medical history. Second, **audit trail**: every action the AI takes and every human review must be logged, so the organization can show later who did what.

## The Costs

Here is an illustrative first-year budget for a clinic like Riverside. These are made-up numbers to show the shape. Use your own. The compliance work makes these settings more expensive to set up than a shop.

**Direct costs.**
- Scheduling and reminder system: about €6,000 a year.
- Ambient documentation tool (compliant, with a data-processing agreement): about €14,400 a year.
- Document-extraction and routing: about €7,200 a year.
- Questions chatbot for patients: about €3,600 a year.
- Setup, integration, and the compliance work (data-protection impact assessment, vendor vetting, security review): about €18,000 one-time.
- Training the staff: about €5,000 one-time.

First-year total: roughly **€54,200**. In steady years after, the recurring subscriptions come to about **€31,200**.

**Indirect costs.**
- Clinicians spend time reviewing every drafted note. This is the safety net and it must stay.
- The compliance overhead: a data-protection impact assessment is not free, and it must be done before going live, not after.
- The learning dip while staff and even patients adapt.
- The cost of a mistake if a draft is trusted without checking — in a clinic, this can harm a patient, which is far worse than a lost sale.
- Ongoing monitoring so the tools stay compliant as rules change.

The full method for counting these costs and turning the savings into a return figure is in [Chapter 16 — Goals, Costs, and Return on Investment](ch16-goals-costs-and-return-on-investment.md). In a regulated setting, add the cost of compliance to the ledger before you count any saving.

## The Results

After a year, measured against a baseline the clinic recorded before starting, the illustrative outcome looks like this. Your numbers will differ. These show what a good fit can look like.

- **No-shows fell.** Automated reminders brought more patients to their appointments, so fewer slots went wasted and more people got seen.
- **The phone queue shortened.** The chatbot and self-booking handled the routine calls, so the front desk could focus on patients who needed a person.
- **Documentation time dropped.** Doctors spent less time typing notes and more time with patients, because they started from a draft to check instead of a blank page.
- **Documents moved faster.** Referrals and forms were sorted and routed automatically, so fewer sat unread and fewer patients were left waiting.
- **Access improved.** The multilingual questions assistant helped parents and citizens who do not speak the local language get answers without waiting for an interpreter.

The honest caveat: none of this was instant. The documentation tool drafted imperfect notes at first and needed each doctor to correct its style. The scheduling bot misunderstood some requests early on. The gains ramped up over weeks, as the learning-curve warning in [Chapter 16](ch16-goals-costs-and-return-on-investment.md) predicts. The clinic measured the real numbers after the ramp, not during it.

## Lessons Learned

**Regulated data means a higher bar, from the first step.** Health data and children's data are special category. You cannot treat them like a product description. Use compliant tools, sign a data-processing agreement, keep the data in-region, and do a data-protection impact assessment before going live. The rules are in [Chapter 10](ch10-privacy-and-gdpr.md) and [Chapter 5](ch05-rules-and-legal-responsibility.md).

**Never automate the decision.** A tool may draft a clinical note, but a doctor signs it and owns it. A tool may sort an application, but a caseworker decides it. In these settings the AI works on the admin around the decision and never makes the decision. This is both a safety rule and, for higher-risk uses, a legal one under the EU AI Act.

**Consent for recording is not optional.** Ambient documentation records a conversation. The patient must know and agree, clearly and beforehand. Do not record quietly. This is personal-data processing under [Chapter 10](ch10-privacy-and-gdpr.md).

**Data minimization protects you.** Give each tool only the data it needs. The scheduling bot does not need the full medical record. The less sensitive data a tool touches, the smaller the damage if it goes wrong.

**Keep an audit trail.** Log what the AI did and what the human reviewed. In a regulated setting, being able to show the record later is as important as the result itself.

**Beware the confident wrong answer.** A drafted note that misstates what was said, or a chatbot that gives a wrong instruction, can cause real harm here. A human must check. The reliability problem is in [Chapter 2 — AI Explained Simply](ch02-ai-explained-simply.md), and the honesty duty is in [Chapter 4 — Ethical AI: Doing the Right Thing](ch04-ethical-ai-doing-the-right-thing.md).

**AI can widen access, not just cut cost.** The multilingual assistant and the always-open chatbot helped people who otherwise struggle to reach the office. In public services, that fairness is a result worth as much as the money saved.

**Measure honestly and expect the ramp.** Record the baseline before you start. Judge the project after the learning curve, not during it. The method is in [Chapter 22 — Measuring Results and ROI](ch22-measuring-results-and-roi.md).

The lesson for clinics, schools, and public offices is the same as every sector's, with the strictest guardrail of all: find the admin load — scheduling, documents, repeated questions — let AI draft, sort, and answer, keep a trained human on every decision, protect the sensitive data as the law requires, and measure honestly. The prize is not just a cheaper office. It is more time with patients, students, and citizens — which is the whole point of the work.
