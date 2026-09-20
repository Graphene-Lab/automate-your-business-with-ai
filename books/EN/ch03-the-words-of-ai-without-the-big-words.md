# Chapter 3 — The Words of AI, Without the Big Words

## In Simple Words

Most bad AI decisions are not caused by bad technology. They are caused by words that nobody stopped to define.

A vendor says "our AI platform integrates with your systems through a low-code API and uses a large language model." Everyone nods. Nobody asks what any of it means. Six months later the project is over budget, the data is somewhere unexpected, and nobody can say who owns what.

Words are the interface. If your team does not share the same meaning for "model", "training", and "integration", you cannot make good decisions about any of them. You cannot compare two vendors. You cannot write a contract. You cannot tell when something is going wrong.

This chapter is a working glossary, not a dictionary. Each word gets a plain meaning, an everyday analogy, and the one question you should ask when you hear it.

One rule runs through all of it. **A real explanation always contains a verb and an object.** Not "it's AI-powered", but "it reads your invoices and puts the total in your accounting file." If someone cannot give you a verb and an object, they have not told you anything.

### 3.1 Data, information, knowledge

Three words people use as if they were the same. They are three different steps, and the difference matters when you plan.

**Data** is raw facts with no meaning attached. A column of numbers. A folder of PDFs. A list of dates. Data on its own tells you nothing. The number 47 is data.

**Information** is data with context. "Invoice 47 was for €1,200 and was paid late." Now the number means something. Information is data placed somewhere.

**Knowledge** is information plus an understanding of what to do with it. "When this customer pays late, it is usually because their own client pays late, so we chase them gently and they always pay eventually." That is knowledge. It lives in a person's head, and it took years to build.

Think of a filing cabinet. Data is the paper. Information is the paper in a labelled folder. Knowledge is knowing which folders matter on Monday morning and which can wait until March.

**Why this matters for you.** AI works on data. It does not automatically gain your knowledge. You can feed a system ten thousand invoices and it will learn patterns in them. It will not learn why your biggest client always pays late on purpose, because that is knowledge held by one person who has never written it down.

Before any AI project, ask: **how much of what makes this task work is written down as data, and how much lives in someone's head?** The gap between those two numbers is the size of your real problem. Closing it is usually harder, and more valuable, than the AI part.

**Ask the vendor:** "What data do you need from us, in what form, and how much of it?"

### 3.2 Algorithm, model, training

**Algorithm.** A recipe. A clear, ordered set of steps that solves a problem. Making coffee is an algorithm. Long division is an algorithm. An algorithm does not need a computer; it just needs steps. The word comes from the name of the ninth-century mathematician al-Khwarizmi, whose work on step-by-step calculation was translated into Latin and eventually gave us the word.

**Model.** In everyday AI talk, a model is the thing you get at the end of training: a set of learned settings you can use to answer new cases. Think of it as a trained employee. You do not have to re-teach them every morning. The knowledge is in them.

The word is used two ways, and mixing them causes confusion. In the older sense, a model is a written description of how something works, like a financial model in a spreadsheet. In the modern AI sense, a model is a file full of numbers that were adjusted until the answers came out right. When someone says "the model" today, they usually mean the second thing.

**Training.** The process of getting from nothing to a model. Show examples. Let the system guess. Compare with the right answer. Adjust. Repeat many times. Chapter 2 explained the mechanism. What matters here is the business meaning: **training is a step you pay for once, and its quality sets the ceiling on everything after it.** A model trained on poor examples cannot be fixed by a better interface. It can only be retrained, which means paying again.

Three questions that clear up almost any conversation:

1. **What is the input?** What goes in?
2. **What is the output?** What comes out?
3. **What was it trained on?** Which examples, from when, how many?

If a vendor cannot answer question three, you are not buying a model. You are buying a promise.

### 3.3 Generative AI, LLM, prompt

**Generative AI** is AI that produces new content instead of only sorting or scoring. Chapter 2 defined it. Here is the vocabulary around it.

**LLM — large language model.** "Large" means it has a lot of adjustable settings, measured in billions. These settings are called **parameters**. A 13-billion-parameter model contains 13,000,000,000 numbers. "Language" means it was trained on text. "Model" means it is the usable result of training.

So an LLM is a very big set of numbers, adjusted by reading an enormous amount of text, until it became good at continuing text. That is the whole thing. It is not a database of facts. It is a text-continuation machine.

**Prompt.** The text you give the model. Your question, your instruction, your request. That is all a prompt is.

The word matters more than it sounds, because what you get back depends heavily on the prompt. A vague prompt gives a vague answer. A prompt with context, an example, and a clear format gives a much better one. Learning to write good prompts is a real business skill, and it takes about a week to learn well.

A prompt is like a brief you give a freelance writer. A bad brief — "write something about our product" — gets something useless. A good brief — "write 150 words for small shop owners, in plain English, in this tone, and leave out pricing" — gets something you can use. The writer is the same. Only the brief changed.

**Hallucination.** When a model states something false in a confident way. The word is imperfect, because the model is not hallucinating in any medical sense. It is continuing text in a way that sounds right, with no separate store of facts to check against. This is why generative AI needs verification for anything that matters.

**Context window.** How much text the model can consider at one time. Think of it as a desk. Everything you want it to look at must fit on the desk. Text that does not fit simply is not there. Modern desks are large, but not infinite, and a crowded desk works worse than a tidy one.

**Ask the vendor:** "Which model do you use, who made it, and where do my prompt and my data go when I send them?"

### 3.4 RPA, no-code, low-code

These three words get sold as if they were AI. Usually they are not.

**RPA — Robotic Process Automation.** Software that copies what a person does at a computer: open this system, copy this field, paste it into that system, click Save. It works by mimicking mouse and keyboard actions, or by using the same screens a person uses. The term came into use in the early 2000s.

RPA is not AI. It has no learning and no guessing. It follows a recorded sequence exactly. It is reliable and brittle at the same time. The analogy is a macro in a spreadsheet: it does the same steps every time, fast, and breaks if the layout changes.

**When RPA is right:** the task is fixed, high-volume, and the screens do not change. Copying order data from an email into your order system a hundred times a day is a classic RPA job. It is cheap and it works.

**When RPA is wrong:** anything that varies. If the input is not always in the same place, RPA will break, and it will break often.

A common and sensible pattern: **AI reads and understands the messy input; RPA does the boring typing.** The AI handles variation. The RPA handles repetition.

**No-code.** Tools where you build an automation by clicking, dragging, and choosing from a menu, without writing program code. Good for simple, clear workflows. Fast to start.

**Low-code.** Similar, but you can write a little code when the menu does not offer what you need. More flexible, slightly more technical.

Both are genuinely useful, and both have a hidden cost: they are easy to start and hard to finish. A no-code workflow that grows to twenty steps, three systems, and four people editing it becomes difficult to understand and dangerous to change. There is a well-known pattern where a company builds dozens of small no-code automations, nobody can map them all, and eventually someone has to rebuild everything.

**Ask the vendor:** "Does this actually learn anything, or does it follow a fixed sequence? If a screen changes, what breaks and who fixes it?"

### 3.5 Cloud, API, integration

**Cloud.** Someone else's computer. That is the honest definition. Your files and software run on machines in a large data centre that another company owns and maintains, and you pay by usage over the internet.

The cloud has real advantages: no hardware to buy, capacity you can grow in minutes, automatic maintenance. It also has one permanent consequence: **your data is on someone else's machines, in a country you may not have chosen, under a contract you probably did not read.** [Chapter 8](ch08-self-hosting-keep-your-data-under-control.md) covers running things yourself, and [Chapter 11](ch11-digital-sovereignty.md) covers control and sovereignty.

**API — application programming interface.** A defined way for one piece of software to ask another to do something.

Think of a restaurant kitchen. You cannot walk in and cook your own meal. You go to a window and order from a fixed menu. The kitchen tells you exactly what you can order and how. That window is the API: it lets the outside world use the kitchen without breaking it.

In practice, your website asks the shipping company's API "what will it cost to send this parcel to Madrid?" and gets a number back in seconds. Nobody phones anyone.

Two things to know. First, if a vendor's product has no API, you cannot connect it to anything yourself, and you depend on that vendor forever. Second, every API call means data crosses a boundary. Each one is a small door. Some doors are locked and logged. Some are not.

**Integration.** Connecting systems so data moves between them without a person carrying it. This is where most projects actually spend their time and money, and vendors rarely say which level they mean:

1. **Files.** Export a spreadsheet, upload it somewhere. Simple, slow, error-prone.
2. **API.** A live connection. Fast, reliable, needs setup work.
3. **Native.** Built into the same platform. Best, but it locks you into that platform.

**Ask the vendor:** "Which systems do you connect to today, by what method, who does the setup, and what happens to the connection if we leave?"

## A Bit of History

The words are older than the technology, and knowing that helps.

**Algorithm** comes from al-Khwarizmi, a ninth-century Persian mathematician whose books described step-by-step calculation. The word is over a thousand years older than the computer. **Data** comes from the Latin for "things given" — facts in the plain sense, long before it meant something stored. **Neural network** comes from the 1940s, from early attempts to describe a brain cell as a tiny on/off switch; the phrase stuck even though modern systems bear little resemblance to real brains. **Machine learning** was named in 1959 by Arthur Samuel, an American researcher working on a checkers program. **Large language model** came into common use around 2018, when models trained on web-scale text appeared. **Prompt** is borrowed from older computing, where it meant the place where you type; it now means the instruction you give a model, which is a much bigger job than typing ever was. **RPA** appeared in the early 2000s to describe software that mimics a human at a screen, and **low-code** and **no-code** entered business vocabulary around 2014.

The lesson in the vocabulary is simple. Almost none of these words were invented by the people who built the technology. They were borrowed, stretched, and then sold. That is why they feel vague. They are vague. Your job is to pin each one down before you sign anything.

## Curiosity

### 3.6 A model trained only on 1930s data wrote Python — how is that possible?

In April 2026 a small research team released an unusual language model. It was called **talkie**, and its whole point was what it did not know.

The team — Nick Levine, David Duvenaud of the University of Toronto, and Alec Radford — trained a 13-billion-parameter model on English text published only before 1931. About 260 billion tokens of it. A **token** is a small chunk of text, roughly a word or part of a word. The sources were digitised books, newspapers, periodicals, scientific journals, patents, and case law.

Nothing from after 1930 went in. No computers. No internet. And crucially, no programming language, because Python was not created until the late 1980s.

Then they tested whether it could write Python.

**The result.** It could, a little. The team gave the model a standard programming test called HumanEval, with a twist: each problem came with a few random example functions shown right in the question. The model had never seen Python in training. But it could look at the examples in front of it and copy the structure.

The results were honest and modest. The vintage model scored far below modern models. Every correct answer it produced was a simple one-line program, like adding two numbers, or a small change to one of the examples it was shown. As the team put it, there is still a long way to go before this capability is notable.

But one example was genuinely striking. Shown a function that encoded a rotation cipher — a code where each letter shifts by a fixed amount — the model produced the decoding function by changing a single character, turning an addition into a subtraction. It had never seen Python. It had never seen a computer. It worked out, from the shape of the example in front of it, that decoding is the reverse of encoding.

**How is that possible?** The answer is a behaviour called **in-context learning**: picking up a pattern from the examples placed directly in the question, rather than from training.

Here is the plain version. To read text well, a model has to become extremely good at noticing structure. Which word follows which. What opens and what closes. What is a definition and what is an example. What is a cause and what is an effect. It learns all of this from ordinary books and newspapers.

Structure, it turns out, transfers. A model that has become very good at noticing "this block opens here, closes there, and this value flows into that one" can apply that same skill to a block of Python it has never seen. It is not using Python knowledge. It is using structure knowledge on Python material.

That is why it could reverse the cipher function. It was not programming. It was pattern-following applied to a subject that did not exist in its training data.

**Why the researchers did it.** The reason is practical and clever: a model trained only on pre-1931 text cannot have memorised the test. Modern models are trained on the modern web, which contains the answers to most public test questions. That is called **data contamination**, and it makes modern benchmarks unreliable. A model may score well because it saw the answer before, not because it can reason. Talkie is clean by construction. Whatever it does, it genuinely did.

**The honest limits.** The team also reported that talkie performed worse overall than its "modern twin" — an identical model trained on modern web data — even after correcting for the fact that modern questions confuse a 1930s model. They blamed part of the gap on OCR noise: in 1930 nothing was digital, so every page had to be scanned and transcribed, which introduces errors that native digital text does not have. They said that as an amateur research effort they never expected to close the gap fully. They did estimate that the historical corpus could grow to well over a trillion tokens, enough for a model roughly comparable to the original ChatGPT.

**The business lesson.** Two things.

First, these models are structure-followers more than fact-collectors. That explains both their power and their unreliability. Structure transfers well. Truth does not come with it.

Second, **data contamination is a real problem in vendor claims.** When a vendor says "our model scores 94% on this benchmark", ask whether the benchmark was in the training data. This is not a small technicality. It is the difference between a measured capability and a memorised answer. Ask it in every vendor meeting.

## A Real Business Example

### When the words are the product: "AI washing"

In September 2024 the United States Federal Trade Commission announced a law-enforcement sweep it called **Operation AI Comply**. The target was companies making exaggerated or deceptive claims about what their products could do with artificial intelligence. The FTC's own name for the practice is **AI washing**.

The pattern regulators described is simple, and it is worth recognising, because it is how bad AI purchases begin.

A company has an ordinary product. Maybe a scheduling tool, or a marketing automation tool, or a chatbot built from a fixed list of replies. The company adds "AI-powered" to the marketing. Nothing in the product changes. The price goes up. Sales go up.

The FTC's position is that this is a consumer-protection problem, not a technical one. If you claim a capability you do not have, that is a deceptive claim, and the label "AI" does not protect you from it.

**Why this is a business example and not just a legal one.** Because the same trap runs in both directions. Vendors use the words loosely to sell. Buyers use the words loosely to justify a budget internally. A manager who cannot explain what the technology does writes "AI-driven automation" in a proposal, gets the budget approved, and then has to make something work that nobody defined.

The regulator's sweep is useful to you as a checklist in reverse. Before you buy, ask:

1. **What specific claim is being made?** Write it down in one sentence with a verb and an object.
2. **How would we know if that claim were false?** If nobody can name a test, the claim is decoration.
3. **Is the claim in the contract?** Marketing language is not a commitment. If a capability matters, it should be written down with a number and a date.
4. **Who is accountable if it does not perform?** Name a person, not a company.

An honest vendor answers all four comfortably. A vendor who is washing gets vague. Vagueness in answer to specific questions is itself the answer.

## How to Do It

### The plain-word test

Use this whenever a technical term appears in a meeting.

**Step 1: Stop on the word.** Do not let it pass because it sounds important.

**Step 2: Ask for a sentence with a verb and an object.** Not "it uses a large language model", but "it reads our support emails and drafts a reply". If the speaker cannot produce one, the word has no content yet.

**Step 3: Ask what goes in and what comes out.** Every real system has an input and an output. Write both down.

**Step 4: Ask what breaks it.** Every technology has a failure mode. An honest vendor names theirs.

**Step 5: Write your own definition on one line and read it back.** If a smart colleague could not understand it, the definition is not finished.

### Your working translation table

| Word you hear | Plain meaning | What to ask |
|---|---|---|
| AI-powered | Uses some learned component, possibly tiny | Which part, exactly? |
| Model | A file of learned settings that answers new cases | Trained on what, when, how much? |
| Training | Adjusting settings against examples until answers match | Who did it, and who checked it? |
| LLM | A very large text-continuation system | Which one, made by whom, running where? |
| Prompt | The instruction you give the model | Can we write and reuse our own? |
| Hallucination | A confident statement that is false | How do you detect and correct it? |
| RPA | Software that mimics a person clicking at screens | What breaks when the screen changes? |
| No-code | Build by clicking, no programming | What can it not do? |
| Low-code | Mostly clicking, some programming allowed | Who maintains it here? |
| Cloud | Runs on someone else's computers | Which country, whose contract, what data leaves? |
| API | A defined window for one system to use another | Does it exist? Can we use it ourselves? |
| Integration | Data moves between systems without a person | Which method, who sets it up, what if we leave? |
| Token | A small chunk of text | How many per typical use, and what does that cost? |
| Context window | How much text the model can look at at once | What happens when our document is too big? |

### Build a shared glossary for your company

Do this once and keep it alive.

1. Start a single page. Every term that comes up in an AI discussion goes on it.
2. Each entry gets three lines: the plain meaning, what it means *in our business*, and one question we still cannot answer.
3. One named person owns the page. Not a committee.
4. Before any vendor meeting, read the page. During the meeting, add to it.
5. Retire entries you never use. Keep it under two pages.

A shared glossary is a small thing with an outsized effect. It turns "we bought AI" into "we use a text model to draft replies and a rule-based tool to file them, and a person checks both".

## Ethics and Responsibility

### 3.7 Privacy, security, bias — the short version

Three words you will hear constantly. Here is the plain introduction. The full treatment lives elsewhere, and you should read those chapters before you deploy anything that touches customer data.

**Privacy** is about who is allowed to see and use personal information. The practical question for every AI tool is simple: *when I paste something in, where does it go, who can read it, and what do they keep?* Never put a customer's personal details into a tool you have not checked. [Chapter 10](ch10-privacy-and-gdpr.md) covers privacy law and GDPR properly.

**Security** is about protecting systems from attack, misuse, and accident. AI adds new ways to be attacked, including tricking a model with carefully worded input and poisoning the data it learns from. [Chapter 6](ch06-cybersecurity-in-the-ai-era.md) covers this in full.

**Bias** is when a system treats some people worse than others in a patterned way, because the examples it learned from were uneven. If past hiring decisions favoured one group, a model trained on them will learn to favour that group. Bias is not a moral failing of the machine. It is a mirror held up to the examples. [Chapter 4](ch04-ethical-ai-doing-the-right-thing.md) covers bias, transparency, explainability, and human responsibility as part of the full ethical framework.

The one thing to take from this section: **you cannot manage a risk you cannot name.** Learning the words is not academic. It is the first requirement for asking the right questions.

## Mistakes to Avoid

**Mistake 1: Accepting "AI" as a feature.** It is not a feature. It is a category containing dozens of very different technologies. Ask which one.

**Mistake 2: Thinking no-code means no thinking.** No-code removes the programming. It does not remove design, maintenance, or the risk of an unmappable tangle of automations.

**Mistake 3: Confusing RPA with AI.** If it follows a recorded sequence, it is not learning anything. That may be exactly what you want, or exactly what will fail.

**Mistake 4: Thinking an API means you are integrated.** An API is a possibility, not a connection. Someone still has to build and maintain the connection.

**Mistake 5: Not asking where the cloud actually is.** "The cloud" is a data centre, in a country, under a contract. Ask which.

**Mistake 6: Letting a vendor define your terms.** If the vendor's vocabulary is the only vocabulary in the room, the vendor controls the meeting.

**Mistake 7: Skipping the plain-word test because it feels slow.** Five minutes of "what does that actually mean?" is cheaper than six months of a project nobody can describe.

**Mistake 8: Believing a benchmark without asking about contamination.** The Talkie experiment exists precisely because modern test results can be inflated by answers already being in the training data.

## Practical Exercise

### 3.8 Translate a technical sentence into plain words

This is the single most useful skill in this chapter. Practise it on these six sentences. Write your answer before reading the model answer.

**Sentence 1:** "Our platform leverages a large language model to deliver intelligent document processing at scale."

*Model answer:* "It reads documents and pulls out the fields you want. It uses a big text model made by someone else. 'At scale' means it can do many at once."

**Sentence 2:** "The solution is a low-code RPA bot with cloud-based API integration."

*Model answer:* "A robot that copies data from one screen to another. You can set it up mostly by clicking. It talks to other systems over the internet through a defined connection. It runs on the vendor's computers."

**Sentence 3:** "We use retrieval-augmented generation to ground the model in your knowledge base."

*Model answer:* "Before it answers, it looks up the relevant pages from your own documents and uses them as the basis. This reduces made-up answers. It only works if your documents are good and up to date."

**Sentence 4:** "The model is fine-tuned on your domain data."

*Model answer:* "They took an existing general model and trained it further on your examples, so it fits your business better. You pay for that. It also means your data was sent to whoever did the training."

**Sentence 5:** "Our AI provides explainable, transparent decision-making."

*Model answer:* "They claim you can see why it decided what it decided. Ask them to show you, on one real case, right now. If they cannot, the claim is decoration."

**Sentence 6:** "It's a multi-agent system with orchestration."

*Model answer:* "Several AI components work on a task in sequence or in parallel, and something coordinates them. Ask: how many components, what does each one do, and what happens if one fails?"

**Now do your own.** Find one sentence from a vendor email you received in the last month. Translate it using the same method: verb and object, input, output, what breaks. Send your translation back to the vendor and ask if it is correct. Their reaction will tell you a great deal.

## Checklist

### 3.9 Your minimum glossary

- [ ] I can explain data, information, and knowledge, and I know how much of my business knowledge is written down.
- [ ] I can define algorithm as "a recipe": an ordered set of steps.
- [ ] I can define model as "the trained thing you use to answer new cases".
- [ ] I can define training as "adjusting settings against examples until the answers match".
- [ ] I know an LLM is a text-continuation system, not a database of facts.
- [ ] I know a prompt is the instruction I give the model, and that its quality changes the result.
- [ ] I know what a token is and roughly what tokens cost per typical use.
- [ ] I know what a context window is and what happens when a document is too big for it.
- [ ] I know "hallucination" means a confident false statement, and that it needs verification.
- [ ] I can tell RPA apart from AI, and I know RPA is cheap and brittle.
- [ ] I know no-code and low-code remove programming, not design or maintenance.
- [ ] I know "the cloud" means someone else's computers, in a specific country, under a specific contract.
- [ ] I know an API is a defined window for one system to use another, and I always ask whether one exists.
- [ ] I know the three levels of integration: files, API, native.
- [ ] I use the plain-word test: a verb, an object, an input, an output, and what breaks.
- [ ] I have started a one-page shared glossary with one named owner.
- [ ] I know that privacy, security, and bias each have a full chapter, and I have read or will read them.

## Key Takeaways

- Most bad AI decisions come from undefined words, not from bad technology.
- A real explanation always contains a verb and an object; if you cannot name one, you have not been told anything.
- Models are structure-followers, not fact-keepers, which is why they transfer skills across subjects and why they state falsehoods confidently.
- The Talkie experiment shows a model with no knowledge of computers can still write a little Python, and it exists because modern benchmark results can be inflated by contaminated data.
- Pin every term down before you sign: what goes in, what comes out, what breaks it, and who owns it.
