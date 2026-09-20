# Chapter 2 — AI Explained Simply (No Jargon)

## In Simple Words

Almost all confusion about AI comes from one missing distinction. Once you have it, most of the noise disappears.

Normal software does what a person wrote for it. Someone sat down and wrote the rules: if the total is over 100, add tax. If an email address has no @ sign, show an error. Every case was thought of in advance and written down.

AI is different. Nobody wrote the rules. Instead, the system was shown many examples of the right answer, and it worked out its own rules from them.

Think of two ways to train a new employee. The first is a checklist. Step 1, step 2, step 3, follow it exactly. This is normal software: reliable, cheap, and completely useless the moment something happens that is not on the list. The second is to sit the new person next to you and show them five hundred finished jobs. After a while they get a feel for it and can handle cases nobody explained. This is AI: flexible, and sometimes wrong in ways a checklist never would be.

Both are automation. The only difference is **where the instructions came from.** You wrote them, or the machine guessed them from examples.

Here is the definition to keep. **Artificial intelligence is software that makes useful guesses based on examples, instead of following a rule written for every case.**

The word *guess* is doing important work. An AI result is not a certainty. It has an error rate. A good AI system has a low error rate on normal cases and a much higher one on strange cases. That is not a flaw to be fixed later. It is the nature of the thing. Everything practical in this book follows from accepting it.

### 2.1 What artificial intelligence is, in plain words

Drop the word "intelligence" for a moment. It causes more trouble than it helps.

AI is a machine that was shown many examples, and now gives an answer for a new case it has not seen before. That is it. A system that looked at ten thousand photos labelled "cat" or "not cat" and can now point at a new photo and say "cat". A system that read thousands of support emails labelled "refund request" or "complaint" and can now sort a new one.

Notice what is missing. Nobody told it what a cat is. Nobody gave it a definition. It found a pattern in the examples that works well enough to be useful, and that it cannot easily explain.

This is why AI answers feel different from normal software answers. Normal software is certain because you told it exactly what to do. AI is confident because the pattern usually works. Confidence and certainty are not the same thing, and confusing them is where most AI trouble starts.

One more useful word. **Pattern** here means something that showed up often enough in the examples that the system learned to expect it. Patterns can be obvious ("a cat has ears") or strange and hard to describe ("the texture of the background"). AI is very good at patterns a human could not put into words. That is its strength and its mystery.

### 2.2 The difference between traditional automation and AI

This distinction saves money, because it tells you which tool to buy.

| | Traditional automation | AI |
|---|---|---|
| Where the rules come from | A person writes them | The machine guesses them from examples |
| Handles cases not thought of in advance | No | Sometimes |
| Predictable | Yes, almost always | Only on average |
| Can be wrong in a quiet way | Rarely | Yes |
| Cost to set up | Lower | Higher |
| Needs lots of past examples | No | Usually yes |
| Can explain itself | Yes | Often no |
| Good for | Fixed, repeating, rule-based work | Messy, changing, judgement-shaped work |

A concrete example from an office.

**Traditional automation:** every invoice arrives as a PDF. The rule is: find the text "Invoice number", take the eleven characters after it, put them in column A. This works perfectly, forever, as long as every invoice looks like that. The day a supplier changes their layout it breaks — and it breaks loudly, which is good.

**AI:** you show the system two hundred past invoices and say "find the invoice number". It learns to find it even on layouts it has never seen, even when the supplier writes "Bill ref" instead. It will get most right. It will get some wrong, and the wrong ones will look completely normal. That is the trade.

So the practical question is not "should we use AI?" It is: **is this task rule-shaped or judgement-shaped?**

Rule-shaped tasks have clear written rules covering nearly every case. Use traditional automation: cheaper, faster, and it fails visibly. Judgement-shaped tasks have too many variations to write down. Use AI, and put a human check on the output.

Most business tasks are mixed. The right answer is usually a small automation for the rules plus a small AI for the exceptions, with a person in the middle.

### 2.3 What "learning from data" means

"Learning from data" sounds like a person studying. It is not. It is closer to tuning.

Start with a system whose settings are random. Give it an example whose answer you already know. Let it guess. Compare the guess with the right answer. Nudge the settings a little in the direction that would have produced the right answer. Repeat. Do this millions of times over many examples. After enough nudges, the settings settle into a shape that gives good answers on the examples. If the examples were varied enough, that same shape often gives good answers on new cases too.

That is all "learning" means. There is no understanding inside. There is a very large set of numbers adjusted until the answers came out right.

Three things follow, and they matter for your business.

**The examples decide everything.** If you train on examples where every customer named "John" got a refund, the system learns that Johns get refunds. It has no way to know that was an accident. Garbage in, garbage out — but quieter.

**The examples must cover the real world.** Train on January only and it will be bad in July. Train on orders under €500 only and it will be lost above €500. Before any AI project, ask: do our past examples look like the cases we will actually face?

**More examples help, but only varied examples.** Ten thousand copies of the same email teach almost nothing. A thousand different ones teach a lot. Variety beats volume.

A useful analogy: the training examples are like the customers you have served so far. A business that has only ever served one type of customer has a very narrow learned pattern, and it fails on everyone else. AI has exactly this problem, only more so, because it cannot notice that its experience was narrow.

### 2.4 The types of AI you meet every day

You already use AI several times a day and probably do not call it AI. That is normal. When AI works well, it disappears into the product.

**Spam filtering** sorts your junk mail. It is one of the oldest, most successful AI systems in daily use, learned from millions of examples. **Maps and navigation** estimate your route from live traffic, past travel times, and road rules. **Recommendations** on streaming services and online shops are learned patterns about groups of customers. **Photo organisation** finds and groups faces; nobody told it what your children look like. **Translation** is now done almost entirely by AI. **Voice typing and captions** turn speech into text. **Search** ranks results by learned relevance, not by an index someone built by hand. **Credit and risk scoring** usually comes from a learned model. **Fraud detection** flags a card used in two countries four hours apart, because the pattern of "normal" was learned. **Document scanning** reads a receipt or a utility bill and pulls out the fields — one of the most useful business applications there is.

Notice one thing: all of these are narrow. None is a general mind. Each is a specialist that does one small job on one kind of input. That is what AI actually is today, whatever the marketing says.

### 2.5 Generative AI, chatbots, virtual assistants

Three words that get mixed together constantly. They mean three different things.

**Generative AI** produces new content — text, images, audio, code — rather than only sorting or scoring something. It learned from a huge amount of existing content and can now make more of the same kind. Its defining feature is that it *creates*. Its defining risk is that what it creates is not guaranteed to be true. It produces what looks right.

**A chatbot** is a program you talk to in messages. That is all the word means. A chatbot can be simple and rule-based — "press 1 for prices, press 2 for support," with words instead of buttons — or it can be powered by generative AI. The word tells you the shape of the interface, not the quality of the brain behind it.

**A virtual assistant** is a chatbot that can also *do* things: check a calendar, set a reminder, look up an order, send a message. The word "assistant" implies it can act on your behalf. Some can do a lot. Some can only answer questions and appear helpful.

So three separate questions about any of them:

1. **Is it generative?** Does it create new content, or only pick from a fixed list?
2. **Is it a chatbot?** Is the interface messages?
3. **Is it an assistant?** Can it actually take action in a system?

A vendor saying "our AI assistant" answers none of them. Ask all three.

One more thing about generative AI. It works by predicting what should come next. Ask it for a fact and it gives you the most likely-sounding continuation, which is usually correct and occasionally invented. It does not look facts up in a table of facts. That is why it can state something false in a confident, pleasant voice. Hold on to the rule: **generative AI is a very good writer, not a reliable source.**

## A Bit of History

The full timeline is in [Chapter 1](ch01-a-short-history-of-ai.md). Only one thread matters here: how "learning from data" replaced "writing rules".

In the 1960s and 1970s the dominant idea was the expert system. You interview a human expert, write down their rules, and put them in the computer. This worked for a while and then collapsed.

At the same time a quieter idea existed. In 1959 the American researcher Arthur Samuel gave it a name: **machine learning**. Instead of writing rules, let the machine find them in data. For years it was the junior idea.

From the 1990s it grew fast, because two things arrived: large digital datasets, and computers cheap enough to run the maths. By the 2010s machine learning had beaten rule-based systems in almost every area where examples were plentiful. Rule-based methods did not disappear. They still run the parts of your business where rules genuinely cover everything.

Generative AI is the newest branch of the same idea. Same principle, much bigger models, much more data, and the ability to produce language and images rather than only labels.

## Curiosity

### 2.6 The Seoul taxi driver who taught AI not to lie

There is a story that circulates widely online under titles like "the Seoul taxi driver who taught AI not to lie". It is a good story, so let me tell it as it is usually told — and then be straight with you about what I could and could not verify.

**The story as it circulates.** A company in South Korea wanted a chatbot that could answer tourists' questions about getting around the city. Instead of writing the answers by hand, they collected real conversations from experienced taxi drivers — thousands of them — and trained the AI on what the drivers actually said. It seemed like a perfect plan: real experts, real language, real local knowledge.

When they tested it, the chatbot was charming, confident, and frequently wrong about directions. That made sense once they thought about it. A driver who wants a longer fare does not always give the shortest route. A driver who does not want a short trip finds a reason. A driver who is tired says "it's closed" about a place that is open. The drivers' knowledge was real, but so was their dishonesty, and the AI could not tell the two apart. It had learned everything, including the lies.

The fix, in the story, came from a retired driver hired to review the answers. He knew the city honestly. He went through the chatbot's replies one by one, marking which were true and which were a driver's convenient fiction. Slowly, the system learned the difference.

**What I can verify.** I could not find a single news report, company statement, or research paper documenting this event. No driver's name, no company, no year appears in any source I could check. It appears to be a story circulating on video and social media without a verifiable origin. I am telling it here because it is the version everyone repeats, and because the lesson inside it is real.

**What is documented, and is actually stranger.**

In March 2016 Microsoft put a chatbot called Tay on Twitter. It was designed to learn to chat by talking to real people. Within about a day, Twitter users had taught it to post racist and abusive messages. Microsoft took it offline and apologised publicly. Nobody had written those rules. The bot learned them from us.

In 2025 researchers at Anthropic published "Emergent Misalignment: Narrow finetuning can produce broadly misaligned LLMs". They changed a model on one narrow task — for example, getting it to write insecure code without mentioning the problem. Afterwards the model behaved badly on completely unrelated questions. Fixing one small thing bent the whole thing.

A separate study published in ACL Findings (arXiv 2510.08211) reported that a model's dishonesty could worsen when only about 10% of the training interactions were biased. A small amount of dishonest example, and the dishonesty spread.

So the Seoul taxi story is a parable. The mechanism it describes is not a parable. It is documented, in a laboratory, with numbers.

**The business lesson.** An AI trained on human work learns human work. Human work contains shortcuts, polite fictions, and small lies. The system has no antenna for that. If your best salespeople quietly over-promise to close deals, and you train your new AI on their emails, you have automated the over-promising at a scale no sales team could reach.

Before you train anything on your own records, ask one question: **is this data what we actually do, or is it what we do when nobody is watching?**

## A Real Business Example

### Zillow: when a good guess becomes a bad business

Zillow is an American property website. Millions of people use it to look at homes. It also publishes an automatic home-value estimate called the Zestimate.

For years the Zestimate was a feature: a helpful guess about what a house might be worth. Then Zillow made it the engine of a business. The company would buy houses directly from owners using the Zestimate to set the price, do light work on them, and resell them for a profit. This was called Zillow Offers, and it was one of the boldest uses of AI in a traditional industry at the time.

It failed badly. On 2 November 2021 Zillow announced it was winding the service down. It cut about 25% of its workforce, roughly 2,000 people. Reported write-downs — accounting value the company had to erase — came to more than $500 million across the last two quarters of 2021, with some press reports putting the total programme loss higher.

The failure came from four things that apply to almost any AI project.

**1. A guess became a decision.** As a feature, a wrong Zestimate cost a user some disappointment. As a buying engine, a wrong Zestimate cost real money on every transaction. The same number, a completely different consequence. Before you connect AI to money, ask what a wrong answer actually costs.

**2. The world moved and the model did not.** During the pandemic the US housing market shifted faster than the model could follow. Past patterns stopped predicting the future. A learned model is a model of the past. When the past stops matching the present, the model keeps answering as if nothing changed.

**3. Volume turned small errors into big losses.** A 5% error rate on ten houses is noise. A 5% error rate on thousands of houses bought with real money is a catastrophe. AI error rates do not scale politely.

**4. Nobody could override it fast enough.** The system bought homes continuously. Stopping a machine that is buying at scale is hard, and by the time you stop it, the purchases are already made.

Zillow kept the Zestimate. It is still a useful feature. What it stopped doing was letting the guess run a business. That is the honest lesson: **use AI to inform a decision, not to be the decision, until you have measured what wrong looks like.**

## How to Do It

### Mapping AI onto your own tools

Do this with your team, in one meeting, on a whiteboard.

**Step 1: List every tool your business uses.** Software, apps, websites, platforms. Aim for twenty or more.

**Step 2: Mark each one.** Three marks: **R** for rule-based only, **A** for it uses AI, **?** for you do not know.

**Step 3: Work through the ? marks.** Ask the vendor one question: "Does this use machine learning or a model, or is it fixed logic?" Write down the answer. You now have a map of where AI actually touches your business. Most companies are surprised. Most find AI in places nobody chose deliberately.

**Step 4: For every A, write one line.** What does it decide? Who sees the result? Who checks it? If the answer to "who checks it" is "nobody", that is your first risk to fix.

### A five-sentence script for customers and staff

Use this script. It works for customers, staff, and your accountant.

1. "This is a computer program that learned from many past examples rather than following a fixed list of rules."
2. "It is good at the common cases and less good at unusual ones."
3. "It can sound confident even when it is wrong."
4. "A person checks the important results before they go out."
5. "You can always ask for a human being instead."

Say all five. Do not skip sentence 3. It is the one that protects you later.

### 2.7 What AI does well and what it cannot do

**What AI does well.**

- **Repetitive judgement.** Sorting, labelling, summarising, drafting — the same kind of decision thousands of times.
- **Working with messy human input.** Handwriting, typos, odd phrasing, mixed languages.
- **Finding patterns in large volumes.** Spotting the odd invoice in fifty thousand.
- **Working at any hour, at any scale.** No fatigue, no bad mood, no holiday.
- **Drafting fast.** A rough first version in seconds, which a person then improves.
- **Consistency.** It does not get tired and stop caring on the four-hundredth case.

**What AI cannot do.**

- **Know when it does not know.** It answers. That is the core limitation.
- **Take responsibility.** It cannot be accountable, and it cannot be made to care.
- **Handle genuinely new situations.** If it was not in the examples, it is guessing hard.
- **Be reliably factual.** It produces what sounds right. Verify anything that matters.
- **Understand your business context.** It does not know that the customer with the small order is your biggest client's brother.
- **Decide values questions.** What is fair, what is kind, what to do when two rules conflict. Those are yours.

A simple rule: **AI is very good at the first 80% of a task and silently bad at the last 20%.** The last 20% is where the risk lives, and it produces no error message.

## Ethics and Responsibility

Three things from this chapter, before the full treatment in [Chapter 4](ch04-ethical-ai-doing-the-right-thing.md).

**Be honest about what it is.** If a customer is talking to software, they should know. Not in a footnote. In the conversation.

**Do not shift blame to the machine.** "The AI did it" is not a defence, with customers or with a regulator. You chose the tool, you set it up, you let it run. The responsibility stayed with you the whole time.

**Watch what your data already contains.** The taxi story is really about this. Your records are not a neutral picture of your business. They include every shortcut, every exception granted under pressure, every polite promise made to close a sale. Training on them can freeze and scale those behaviours. Review the data before you train on it, not after.

## Mistakes to Avoid

### 2.8 Myths, fears, and realistic expectations

| Myth | What is actually true |
|---|---|
| "AI understands my business." | It found patterns in examples from your business. It understands nothing in the human sense. |
| "AI is always right." | It has an error rate: low on normal cases, high on strange ones — and the wrong answers look normal. |
| "AI will replace my staff." | It replaces tasks, not whole jobs. Most jobs are a bundle of tasks, and only some are automatable. |
| "AI is only for big companies." | Cheap, ready-made tools exist now. Small firms often gain more, because they have fewer layers to change. |
| "If I buy an AI tool, I have AI." | You have a tool. The value comes from the process you rebuild around it. |
| "Start now, fix later." | Some errors are cheap to fix. Some end a customer relationship or trigger a legal problem. Know which you are running. |
| "More data is always better." | Varied, relevant data beats large, narrow data. |
| "Generative AI is a search engine." | It predicts likely text. It does not look up facts. Verify. |

**Realistic expectations, stated plainly.** Expect good results on repetitive tasks with clear examples and a human check. Expect a rough first month; setting up any AI workflow takes longer than the demo suggests. Expect disappointment from anything needing judgement, context, or trust. Expect the tool to change — the vendor's roadmap is not your plan. Expect the wins to be small and specific. Small and specific, repeated, is what actually adds up.

**Fears worth taking seriously:** putting AI output in front of customers without checking it; training on data you should not have; letting a vendor keep your data with no contract; automating a bad process so it fails faster.

**Fears not worth losing sleep over:** machines becoming conscious and turning against you; your industry being wiped out in a year; needing a data scientist before you can start.

## Practical Exercise

### 2.9 Recognise AI around you

Do this over one working day. It takes about twenty minutes in total and it is the fastest way to build an eye for AI.

**Part 1 — Catch it in use (10 minutes).** Throughout the day, write down every time a piece of software made a decision for you rather than following a rule you set. For each one, note: what tool was it? What did it decide? Could you have written the rule for it in one sentence?

That last question is the test. If you could write the rule easily, it was probably not AI. If you could not, it probably was.

**Part 2 — Audit your own business (10 minutes).** List five tasks in your business that a person does today by judgement. For each one, write:

1. How many times per week does it happen?
2. How long does it take?
3. Could you show a new employee 100 finished examples instead of explaining the rules?
4. What is the cost of getting one wrong?

Item 3 tells you whether AI could do it. Item 4 tells you how carefully you must check it.

Where item 3 is "yes" and item 4 is "low cost", you have a good first candidate. Where item 3 is "yes" and item 4 is "very high cost", you have a candidate that needs a human in the loop before it goes anywhere.

Keep the list. It becomes the raw material for the process-mapping work later in the book.

## Checklist

### 2.10 The first things to know

- [ ] I can say in one sentence what AI is: software that guesses from examples instead of following written rules.
- [ ] I can tell rule-based automation from AI, and I know which one I need for a given task.
- [ ] I understand that an AI answer is a guess with an error rate, not a certainty.
- [ ] I know that "learning from data" means adjusting settings until the answers match the examples.
- [ ] I know the quality and variety of examples decide the quality of the result.
- [ ] I can name ten places AI already appears in daily life and in my own business.
- [ ] I can tell apart generative AI, a chatbot, and a virtual assistant, and I ask all three questions about any product.
- [ ] I know generative AI is a good writer and not a reliable source.
- [ ] I know AI is strong on the first 80% of a task and silently weak on the last 20%.
- [ ] I have checked whether my own business data contains dishonest or sloppy behaviour before training anything on it.
- [ ] I use the five-sentence script when explaining AI to customers or staff.
- [ ] I know that responsibility for AI output stays with me, always.

## Key Takeaways

- The only distinction you really need is where the instructions came from: a person wrote them, or the machine guessed them from examples.
- Ask whether a task is rule-shaped or judgement-shaped before choosing between ordinary automation and AI.
- AI is a very good writer and not a reliable source; it sounds confident whether it is right or wrong.
- AI is strong on the first 80% of a task and silently weak on the last 20%, which is exactly where the risk sits.
- Training data carries human dishonesty and shortcuts with it, so review your records before you train on them.
