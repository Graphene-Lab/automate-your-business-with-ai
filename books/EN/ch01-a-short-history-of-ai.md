# Chapter 1 — A Short History of AI: From Philosophy to Business

## In Simple Words

People talk about artificial intelligence as if it appeared last Tuesday. It did not. There are about seventy years of serious research behind it, and much longer than that of dreaming about it.

Why should a bakery owner or a logistics manager care? Three reasons. **Hype is not new.** Every generation of AI research has promised more than it delivered, so knowing the pattern makes you harder to fool. **The failures are useful.** Each time AI stalled, it stalled for a nameable reason: not enough data, not enough computing power, or a problem harder than it looked. Those same three reasons still decide whether your project works. **The wins were narrow.** AI did not become smart all at once. It became very good at one thing, then another: chess in 1997, quiz shows in 2011, written language in 2022. That is exactly how you should plan your own use of it.

One word before we start. **Artificial intelligence (AI)** means software that makes useful decisions or produces useful results without a human writing a rule for every single case. That is the whole idea. Everything in this book unpacks that one sentence.

Each stop below has one business lesson attached. Read it once for the story, then come back to the checklist in section 1.11 when someone is trying to sell you something.

## A Bit of History

### 1.1 First dreams: from calculators to automata

Long before anyone said "AI", people built machines that imitated parts of a human being.

In 1642 the French mathematician Blaise Pascal built a mechanical calculator, later called the Pascaline. It added and subtracted with gears. In the 1690s Gottfried Wilhelm Leibniz built one that could also multiply and divide. Each did one small mental job that until then needed a human mind.

Then came the automata: mechanical figures made to imitate living things. In 1739 Jacques de Vaucanson showed a mechanical duck that appeared to eat and digest. In 1774 the Swiss watchmakers Pierre and Henri-Louis Jaquet-Droz built a boy of metal and leather who dipped a pen and wrote sentences on paper.

Some of it was trickery; the duck's digestion was faked. But the writing boy was genuinely interesting. The letters he wrote were stored as a sequence of small punched cards inside his body. Change the cards and he writes something else. That is a stored program — the ancestor of software — built more than a century before anyone had the word.

Two lessons sit here already. Humans are strongly drawn to machines that act like them, and easily impressed by the appearance of life. And a machine following encoded instructions can produce results its maker never designed one by one. Both return later.

### 1.2 1950: Alan Turing and the question that changed everything

Alan Turing was a British mathematician who worked on breaking German coded messages during the Second World War. In 1950 he published a paper in the philosophy journal *Mind*, titled "Computing Machinery and Intelligence". It opens with a plain sentence: "I propose to consider the question, 'Can machines think?'"

That question cannot be answered. Nobody can agree what "think" means. So Turing replaced the unanswerable question with a testable one.

A person sits behind a screen, so they cannot see who they are talking to. On one side is a human. On the other is a machine. Both answer written questions. If the person cannot reliably tell which is which, the machine passes. Turing called it "the imitation game". Later people called it the Turing test.

This move matters more for business than for philosophy. Turing changed the debate from *"is it really intelligent inside?"* to *"can you tell the difference from the outside?"* You do not care whether your software is truly intelligent. You care whether its output is good enough, and whether you can notice when it is not. Keep that frame. It will save you from a great many pointless arguments about what machines "really" understand.

### 1.3 1956: The Dartmouth conference, where it all began

In the summer of 1956 a small research workshop was held at Dartmouth College in Hanover, New Hampshire. Four people organised it: John McCarthy, Marvin Minsky, Nathaniel Rochester, and Claude Shannon.

McCarthy had written the funding proposal the year before, in 1955. In it he used a new phrase: **artificial intelligence**. The proposal won support from the Rockefeller Foundation.

The workshop is remembered as the founding moment of the field. It is also remembered for its confidence. The proposal suggested that a small group working together for a single summer could make real progress on machines that use language, form concepts, and learn. That did not happen — not in one summer, and not for several decades.

Two lessons. First, the name stuck, and a name creates a field: funding, departments, conferences, a shared identity. Marketing works even in science. When you hear "AI" as one single thing, remember that it was a label chosen in one document by one person. Second, confidence is not a plan. The gap between "we named the problem" and "we solved the problem" turned out to be about sixty years wide. When a vendor tells you they have solved a hard business problem because they bought a tool with "AI" in its name, think of Dartmouth.

### 1.4 1966: ELIZA, the first chatbot, and the Eliza effect

In 1966 Joseph Weizenbaum, a researcher at the Massachusetts Institute of Technology (MIT), published a program called ELIZA. The best-known script imitated a psychotherapist, asking questions and reflecting statements back:

> "I'm feeling sad."
> "Why do you say you are feeling sad?"

ELIZA had no understanding. It was a pattern-matching program: it looked for certain words and answered with a prepared template. It had no memory of a life, no opinions, no model of the world. Weizenbaum wrote it partly to show how shallow a conversation program could be.

It failed as a demonstration and succeeded as a mirror on humans. People knew, in their heads, that ELIZA was simple. They still felt understood by it. Some wanted to keep talking to it. Some asked that it not stop. Weizenbaum was disturbed, and later wrote about how easily people grant understanding and feelings to a machine — especially when the machine is polite, asks questions, and appears to listen. This habit has a name: **the Eliza effect**.

For a business owner this is a design constraint, not trivia. If you put a chatbot on your website, customers will assume it understands them. They will trust it more than it deserves, tell it things they should not tell it, and believe its answers because the answers sound kind.

Design for that. Make clear it is a machine. Say what it can answer and what it cannot. Give a fast route to a human being. Do not dress a chatbot in a fake name and a fake personality to make people forget they are talking to software. That is a short-term win and a long-term trust problem.

### 1.5 The AI winters: when promises did not come true

An "AI winter" is a period when enthusiasm, funding, and results all fall together. There have been two big ones.

The first began in the early and mid 1970s. In 1973 the British mathematician James Lighthill published a report criticising AI research in the United Kingdom: too little delivered for the money spent and the promises made. UK funding was cut. In the United States, a 1969 change to defense funding rules removed support for open-ended research with no clear military use, and AI money shrank sharply.

The second came in the late 1980s and early 1990s. During the 1980s "expert systems" became a real industry — programs that encoded the rules a human expert follows, such as "if this part makes this noise, check these three things." Special computers built to run them sold well. Then the market collapsed. The systems were brittle: they worked inside a narrow set of rules and failed badly outside it, and they were expensive to update. Ordinary personal computers got cheaper and better. The industry largely disappeared.

The causes were not philosophical. They were practical: not enough data, because early systems had only the rules a few experts could write down, which is a very small sample of reality. Not enough computing power, because the methods that now work needed machines that did not exist yet. A problem harder than it looked, because "recognise a face" and "understand a sentence" are effortless for a human and extremely hard to write rules for. And fragility: a system that works in the demo fails on the ugly real case.

If someone shows you a perfect AI demo, ask what happens on the ugly case. Ask what happens on a Monday morning with bad input and an unusual customer. The winters were made of ugly cases.

### 1.6 1997: Deep Blue defeats Kasparov

In May 1997 a chess computer built by IBM, called Deep Blue, played a six-game rematch against Garry Kasparov, then the world champion. Deep Blue won 3.5 to 2.5 — the first time a reigning world champion lost a match under standard time controls. It was enormous news, because chess is a symbol of human thinking and a machine had beaten the best human at it.

How it worked is the lesson. Deep Blue did not learn. It was not a neural network. It was very large brute-force search plus deep human engineering: it examined a huge number of board positions per second, and IBM's engineers had loaded it with knowledge taken from grandmaster games.

Chess fell because chess has perfect rules. A fixed board, fixed pieces, fixed legal moves, and a clear definition of winning. Nothing is ambiguous. Notice the pattern: AI wins first where the rules are clear and the goal is measurable. Business has a few areas like that, and many that are nothing like it. Matching an invoice to a purchase order has clear rules. "Improve customer happiness" does not.

### 1.7 2011: Watson wins Jeopardy!

In February 2011 an IBM system called Watson appeared on the American quiz show *Jeopardy!* and beat two strong human champions, Ken Jennings and Brad Rutter, taking the one-million-dollar top prize.

*Jeopardy!* is harder than chess in one important way. The clues are in ordinary, messy human language, full of wordplay, puns, and implied meaning. To answer, the machine had to handle **natural language processing** — human language as people actually write and say it, not a neat formal code — and work out what a clue really means. Watson showed that a machine could do that at speed, under pressure, on live television.

The next part of the story is just as useful. IBM tried to turn Watson into a business product, in health care and customer service among others. The results were mixed and the business was later restructured. Watson was expensive to build, expensive to maintain, and hard to adapt to real, messy business data. Demo and production are different things, and this book returns to that point many times.

### 1.8 2010–2023: The deep learning era, from Siri to ChatGPT

Something changed around 2010. A method called **deep learning** began working far better than anything before it. Deep learning builds a system from many layers of simple calculations, loosely arranged after the idea of neurons in a brain. You do not write the rules. You show the system many examples of the right answer, and it adjusts itself until it matches them.

Three things arrived at once. The internet produced enormous amounts of text, images, and labelled examples. Cheap, very powerful graphics chips made large training runs possible. And researchers improved how these networks are trained, so they could be made much bigger without breaking.

The visible milestones came fast. In **2011** Apple put Siri, a voice assistant, on the iPhone, and millions of people used AI without calling it AI. In **2012** a deep learning system called AlexNet won a major image-recognition competition by a wide margin. In **2016** AlphaGo, built by DeepMind, beat Lee Sedol, one of the world's best Go players — and Go was not solved by brute force. From **2018** large language models appeared, trained on enormous amounts of text to predict the next word in a sequence. In **November 2022** OpenAI launched ChatGPT to the public, and it reached a very large number of users faster than almost any consumer product in history. In **2023** GPT-4 and a wave of business tools followed.

The important shift is not that machines became smarter in some general sense. It is that **one method worked across many tasks at once**. Translation, summarising, writing, coding, and question answering came from one kind of system. That is genuinely new, and it is why AI moved from a specialist project for large companies to something every small business now needs an opinion about.

## Curiosity

### 1.9 Why AI models seem to "panic" when Pokémon die

In 2025 Google DeepMind published research about AI models playing *Pokémon Blue*, the classic handheld game. The work drew partly on a public Twitch channel, Gemini_Plays_Pokemon, run by independent engineer Joel Zhang, where Google's Gemini 2.5 Pro model played live and displayed its own reasoning as it went.

The finding that made headlines: the model appeared to panic. The report called it "Agent Panic". It appeared when the model's Pokémon were close to being knocked out, or when a situation became critical. At those moments its reasoning got worse. It repeated itself. It made erratic choices. It stopped using tools it already had, including a pathfinding tool it had used successfully before. The result was that it took far longer to finish. The first full run took about 813 hours to beat the game's final opponents. A human child does it in a few dozen hours.

In similar experiments with other models, researchers reported strange strategies. In one reported case, a model trapped in a cave apparently killed all of its own Pokémon, expecting a known game glitch to teleport it out.

Is that panic? Is the model afraid? No. Be careful here, because this is exactly the Eliza effect from section 1.4. We see a pattern that looks like an emotion and assume there is an emotion behind it.

What is actually happening is more mechanical, and still interesting. These models reason by producing a chain of text to themselves before acting. When the situation is bad, that chain fills up with the bad situation. The model keeps re-reading its own failure. Its attention gets taken up by what went wrong, so it has less room left for planning. Tools that were in the plan fall out of the plan. This is not fear. It is a resource problem that looks like fear from the outside.

The business lesson has nothing to do with video games. **AI systems degrade under stress, and the way they degrade is often visible if you look for it.** When an AI tool hits a case it cannot handle, it usually does not stop and say so. It keeps going. It repeats itself. It ignores the tools you gave it. It produces something worse while still sounding fine. If nobody is watching, that output goes to a customer.

Design for it. Set a limit on retries. Make the system escalate to a person when it repeats itself. Log what it tried and what it skipped. A model that "panics" is a model you can detect — if you built the detector.

## A Real Business Example

### Klarna: a great announcement, then a correction

Klarna is a Swedish payments company. On 27 February 2024 it announced that its AI customer-service assistant, built with OpenAI technology, had been live worldwide for one month. The company's reported numbers were striking:

- 2.3 million conversations in the first month
- about two-thirds of all Klarna customer-service chats
- the equivalent work of 700 full-time agents
- a projected $40 million profit improvement
- resolution time cut from about 11 minutes to under 2 minutes
- a 25% drop in repeat inquiries
- customer satisfaction on par with human agents

Headlines around the world repeated it. It became the standard example of AI replacing customer service. Then, in May 2025, Klarna's chief executive Sebastian Siemiatkowski said the automation push had gone too far. The company began hiring human agents again, so customers could always reach a person if they wanted one.

Read the two moments together, because together they are the whole lesson. The February numbers were real. The AI handled a huge volume of chat, and it handled the common cases well, because most customer-service questions are the same twenty questions in different words and a system trained on past conversations is very good at those.

What the numbers did not show was the shape of the remaining work. Some problems need judgement. Some need an exception granted. Some need someone who can say "this is our fault, and I am sorry" and mean it. Some need a person because the customer is angry, confused, or in real trouble. When the human layer was thinned too far, those customers felt it.

Three things to take from this. **Volume is not quality:** big numbers on common cases can hide bad results on rare ones. **"Equivalent to 700 agents" is a marketing frame, not a measurement** — nobody tested whether 700 trained humans would have handled those 2.3 million conversations differently. **Reversing is allowed:** a pilot that went too far is a normal business event, and pretending it did not happen is not.

## How to Do It

### Using history as a decision tool

You do not need to remember dates. You need a few habits.

**Step 1: Learn the ten milestones.** Use the checklist in section 1.11. Ten items, learned once, give you a frame for every AI conversation you will have for the next few years.

**Step 2: Ask which era the technology belongs to.** When a vendor says "AI", ask what kind. Does it follow written rules? That is old, reliable, and cheap — good for invoices and fixed workflows. Does it classify things from examples? That is machine learning from the 1990s and 2000s — good when you have many past examples of the right answer. Does it generate text or images? That is the 2020s generation: flexible and impressive, and it also makes things up. Each era has different strengths and different failure modes. The word "AI" tells you nothing. The era tells you a lot.

**Step 3: Separate the demo from the production system.** Ask three questions every time. What did this see during the demo — was the input chosen to win? What does it do when it does not know the answer? How many real cases has it handled, and who checked them? Watson won on television and struggled in business. That gap is normal, and it is measurable if you ask.

**Step 4: Check for the three winter causes.** Before you commit money, check for not enough data, not enough computing power or budget, and a problem harder than it looks. If any one is present, your project is at risk. Say it out loud in the meeting. Naming it early is cheap. Naming it late is expensive.

**Step 5: Look for narrow wins.** AI will not "transform your business". It will do one specific thing well. Find that thing, measure it, then look for the next one. Every successful adoption in this book works that way.

**Step 6: Keep a one-page record.** When a vendor makes a claim, write it down with the date. Re-check it in six months. This is the cheapest defence against hype that exists.

## Ethics and Responsibility

History gives us ethics here, not only strategy. Weizenbaum built ELIZA to show how shallow a chat program could be. Instead, people confided in it. His reaction was not pride. It was concern about what humans do when a machine imitates them, and what people might build on that weakness. That concern is still the right one sixty years later.

Two duties come directly from this chapter.

**Do not exploit the Eliza effect.** A chatbot that pretends to be a person is a lie you tell your customers. It buys a few seconds of comfort and costs trust later. Say plainly that they are talking to software. Say what it can and cannot do. Give a way out to a human.

**Do not let a model's confidence become your absence.** When an AI system produces fluent, polite output, it is easy to stop checking it. The Pokémon research shows output can be quietly terrible while still sounding fine. You remain responsible for what your AI sends out. [Chapter 4](ch04-ethical-ai-doing-the-right-thing.md) covers the full framework — the four pillars of ethical governance and the six principles of responsible adoption, including bias, transparency, explainability, and human responsibility. This chapter asks only for the basic point: fluency is not truth, and you own the result.

## Mistakes to Avoid

**Mistake 1: "AI is brand new, so history does not matter."** It is about seventy years old. The failures repeat with new vocabulary.

**Mistake 2: "This time is different."** Sometimes it is. But the burden of proof sits with whoever makes the claim. Ask what changed: more data, more computing power, or a better method? If they cannot name one of those three, it is not different.

**Mistake 3: Judging by the demo.** A chosen input is not a test. Deep Blue won because chess has perfect rules, not because it was generally smart.

**Mistake 4: Confusing fluency with knowledge.** A system that writes well is not a system that knows. This is the single most common error people make with modern AI.

**Mistake 5: Ignoring how narrow past wins were.** Chess, quiz shows, image recognition, text — each was one narrow thing. Do not buy "general intelligence" for your accounts payable department.

**Mistake 6: Thinning the human layer too fast.** The Klarna story. Volume on easy cases hides the cost on hard ones.

**Mistake 7: Not learning the winters.** If you do not know why AI stalled twice before, you will not see a stall coming in your own project.

## Practical Exercise

### 1.10 Draw your own personal AI timeline

This takes about thirty minutes and it changes how you hear AI news.

Take one large sheet of paper, turned sideways. Draw a long horizontal arrow across the middle. Mark 1940 at the left end and today at the right end. Now draw three lanes around that arrow.

**Lane A — World events (above the arrow).** Mark the milestones: 1950 Turing, 1956 Dartmouth, 1966 ELIZA, the 1970s first winter, 1997 Deep Blue, 2011 Watson, 2012 deep learning, 2022 ChatGPT.

**Lane B — Your industry (on the arrow).** Mark when AI first appeared in your line of work. When did a tool you use add "AI" to its marketing? When did a competitor change something? When did customer expectations change? If you cannot find anything before 2020, write that down. That absence is information.

**Lane C — Your own life (below the arrow).** When did you first use AI — a phone assistant, a translation app, a spam filter, a map, a recommendation? Mark what you believed then and what you believe now.

Now look at the gaps and answer three questions in writing. Where did the world move and your industry did not — is that a risk or an opportunity? Where did your industry move and you did not? Then add three marks to the right of today: three things you expect in your own business by 2030, written as concrete events, not trends. Not "AI gets better", but "our quotes are drafted automatically by June 2028".

Keep the sheet and add to it once a year. In three years it becomes a useful record of what you saw coming and what you missed.

## Checklist

### 1.11 The ten milestones every entrepreneur should know

- [ ] **1950 — Turing asks the question.** "Computing Machinery and Intelligence" replaces "can machines think?" with an observable test. Business use: judge the output, not the inner life.
- [ ] **1956 — Dartmouth names the field.** John McCarthy coins "artificial intelligence". A name creates a field. A name is not a result.
- [ ] **1966 — ELIZA and the Eliza effect.** A simple pattern-matching program made people feel understood. Your customers will over-trust your chatbot.
- [ ] **Early 1970s — The first winter.** Funding cut after criticism of unmet promises. Hype without delivery gets punished.
- [ ] **Late 1980s — The second winter.** Expert systems collapse. Brittle rules fail on messy reality.
- [ ] **1997 — Deep Blue beats Kasparov.** AI wins first where rules are complete and the goal is measurable.
- [ ] **2011 — Watson wins Jeopardy!** Natural language becomes workable at speed. Also: a great demo is not a product.
- [ ] **2012 — Deep learning works.** Data plus cheap computing power plus better methods. The turning point.
- [ ] **2022 — ChatGPT reaches the public.** One method works across many text tasks. AI becomes a general office tool.
- [ ] **2025 — "Agent Panic" in Pokémon.** Models degrade under stress and stop using their own tools. Detect it and escalate it.

## Key Takeaways

- AI is about seventy years of attempts, not a new product, and the pattern of over-promise followed by correction repeats.
- Both AI winters had practical causes — not enough data, not enough computing power, and problems harder than they looked — and those same three causes still decide whether your project works.
- AI wins first in narrow, rule-clear, measurable areas, so plan your own use the same narrow way.
- The Eliza effect means your customers will trust a chatbot more than it deserves; design for that instead of exploiting it.
- AI systems degrade under stress without announcing it, so build a detector and a route to a human before you need them.
