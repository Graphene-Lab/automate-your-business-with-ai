# Appendix M — Resources, Reading, and Recommended Tools

A short, honest list of tools and reading. These are **not** ads. They are real, named projects you can look up yourself. Most are open-source, which means you can see how they work and are not locked to one company.

**A note on skill level:** Some tools here need a technical person (an IT partner, a developer, or a tech-savvy hire). You do not need to run them yourself. Read them to know what is possible and to talk intelligently with whoever sets them up.

**Verified:** Every tool and book below was checked against its own website or code repository in **September 2026**. Tools change fast — re-check before you adopt.

## Run AI locally (on your own machines)

Running models locally means the AI works on your own computer or server. Your data does not leave your machine. This is the most private option.

- **Ollama** — `ollama.com`. A free, open-source tool to run open AI models on your own computer. Local models cost nothing and keep data on your machine. It is the easiest starting point for local AI and is often used as the engine behind other tools.
- **Thunderbolt** — `thunderbolt.io` (code: `github.com/Thunderbird/thunderbolt`). An open-source, self-hostable **AI client** from MZLA Technologies, the Mozilla subsidiary that also makes Thunderbird. Announced April 2026 and licensed under the Mozilla Public License 2.0. Its promise is "AI You Control: choose your models, own your data, eliminate vendor lock-in." It runs on web, Windows, macOS, Linux, iOS, and Android, and works with local, on-premise, or cloud models. For local use it points to Ollama or llama.cpp. **Status:** early-stage and under a security audit — treat it as promising, not finished.
- **llama.cpp** — a well-known open-source engine that runs large models on ordinary computer hardware, including your own laptop. It is the technical engine others build on. Mentioned here because Thunderbolt recommends it for free local inference.

**When to choose local:** you handle sensitive data, want to avoid per-message fees, or need the AI to work without sending data out. The trade-off: you pay for hardware and setup, and local models are usually smaller than the biggest cloud models.

## Build automations (connect AI to your work)

These tools let you wire AI into real tasks — reading documents, answering tickets, moving data between apps.

- **Haystack** — `haystack.deepset.ai` (code: `github.com/deepset-ai/haystack`). An open-source framework from **deepset** (Germany) for building AI applications, especially **RAG** pipelines. RAG ("retrieval-augmented generation") means the AI looks up your own documents before answering, so it answers from your facts, not guesses. Free to install (`pip install haystack-ai`); paid enterprise support is optional. Best for a team with a developer.
- **n8n** — `n8n.io`. A **fair-code** automation platform (source is public on GitHub) that lets you build workflows on a visual canvas and connect to 500+ apps. It also builds AI agents and RAG systems, with human-in-the-loop approvals. You can self-host it or use their cloud. "Fair-code" means the code is open to read and self-host, but not a standard open-source license — check the terms if you plan to resell it.

**When to choose these:** you want AI to act on your data across several apps, not just chat. Haystack is for building custom AI pipelines; n8n is for connecting apps and automating steps with AI inside them.

## Learn more (reading)

- **Headcount Zero: How to Build an AI-Run Company with Paperclip** — by **Anthony David Adams**. An open-source book (on GitHub, license CC BY-NC-SA 4.0) about running a company where AI agents do most of the work and a small number of humans judge the output. It covers the "one-person company" idea, how AI agents work, the economics of few employees, and how to govern AI with kill-switches. Read it for the bold vision — then apply it with the caution this book teaches: keep humans in charge of what matters.
- **This book's own chapters** — the strongest "further reading" is often the chapters you skimmed. Re-read the risk chapter before any launch, and the data chapter before you connect any tool to real customer data.
- **Vendor and project documentation** — for any tool above, read the project's own docs and license before adopting. It tells you what is free, what is paid, and what you are agreeing to.

## How to choose, in three questions

1. **Where must the data stay?** If it must not leave your machines, look at the local tools (Ollama, Thunderbolt, llama.cpp).
2. **Do you have technical help?** If yes, Haystack and n8n open the most doors. If no, start with a simple hosted tool and a small pilot.
3. **Can you leave later?** Prefer tools that let you export your data and switch models. Avoid anything that locks your data in.

## A caution on lists like this

Tools rise and fall. A name here may change, merge, or fade within a year. That is normal in AI. The **principles** in this book — keep data private, keep a human in the loop, measure results, avoid lock-in — outlast any single tool. Use this list as a map, not a promise.
