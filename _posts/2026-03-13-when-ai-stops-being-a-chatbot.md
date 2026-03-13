---
layout: post
title: "When AI Stops Being a Chatbot"
date: 2026-03-13
---

At some point over the last few years, AI quietly became part of my engineering workflow.

Not in the way people usually describe it—generating code snippets or answering simple questions. Instead, it started showing up in the places where engineering work is actually difficult: reasoning through system design, debugging infrastructure problems, and trying to articulate how complicated data systems fit together.

Early on, that workspace was ChatGPT.

Whenever I was stuck on something—a pipeline architecture, a dependency issue, a strange CI failure—I would open a conversation and start working through the problem. Sometimes it produced useful code. More often it acted like a second set of eyes, helping me interrogate assumptions and explore how a system might behave.

It was less like asking a tool for answers and more like thinking out loud with a collaborator that never got tired.

Over time, this became a pattern. Difficult problems would send me to a chat window before they sent me to documentation.

But the more I relied on it, the more one limitation became obvious.

> **Important:** Chat is a terrible interface for thinking about systems. Every conversation resets. Every session starts from scratch. The tool is helpful, but the workflow fights you.
{: .important}

---

![Chat interface vs AI workspace — the shift in how AI fits into engineering work](/assets/images/ai-workflow-shift.svg)

## The Early AI Workflow

The first phase of working with AI looked something like this:

1. Open a chat.
2. Paste code.
3. Describe the problem.
4. Iterate on ideas.

For many engineering tasks, that was surprisingly effective.

It worked well for:

- debugging dependency issues
- troubleshooting infrastructure configurations
- reasoning about data pipeline steps
- drafting documentation for developer tools
- testing architectural ideas

In many ways, AI functioned like a junior collaborator with infinite patience. It would happily walk through problems step by step, propose alternate approaches, and point out things that were easy to miss when you'd been staring at the same code for too long. 

Inititally this workflow had friction, as every conversation existing in isolation. That changed when ChatGPT introduced persistent memory — the ability to carry context across sessions. Suddenly the model could remember my projects, my preferences, my way of working. I didn't have to re-explain everything from scratch. That was a genuine shift, and it made the workflow meaningfully better.

> **Note:** ChatGPT's memory feature moved AI from a stateless tool to something that could actually learn your context over time — closer to a collaborator than a search engine.
{: .note}

But even with memory, a core limitation remained. The model knew what I had told it before — but it had no access to the actual systems. Codebases evolve. Infrastructure changes. Pipelines get restructured. ChatGPT's memory was a record of past conversations, not a live view of the work itself. Every time something changed, the gap between what the model knew and what was actually true quietly widened.

The chat window was a separate universe. That limitation didn't matter much at first, but as AI became more embedded in the workflow, the fragmentation became harder to ignore.

---

## Engineering Work Involves Context

Engineering rarely happens in small, isolated snippets. Real work means navigating a web of related pieces:

- repositories and their history
- documentation and architecture decisions
- infrastructure definitions
- data schemas, pipelines, and orchestration logic

Understanding a system means understanding how all of those relate to each other — and how they're changing. You can paste pieces of that context into a chat window, but the system itself never lives there. The model only sees what you choose to show it, at that moment, frozen in time.

Once you start using AI as a collaborator rather than a search engine, this gap becomes the main constraint.

---

## The Moment the Workflow Changes

At some point the question shifts. Instead of:

> "Can this tool answer my question?"

It becomes:

> "Where should AI live in the workflow?"

That's a fundamentally different problem — and it exposes the core limitation of chat. Chat is optimized for conversation. Engineering work needs something closer to a workspace: a place where code, documents, datasets, and decisions all exist together, and where AI can operate on the current state of things rather than a description of them.

> **Note:** This isn't a model problem — it's an interface problem. Models improved dramatically over this period. The workflow stayed the same.
{: .note}

---

## Moving Toward an AI Workspace

More recently, I've been experimenting with a workflow centered around Claude.

The shift isn't model capability — it's working with artifacts instead of isolated conversations. Instead of starting every session from a blank window, the work begins with the things you're already building: documents, code, datasets, structured ideas. Documents evolve collaboratively rather than being rewritten from scratch. Code and explanations live alongside each other. Context accumulates rather than resetting.

The next layer is live connections. MCP (Model Context Protocol) lets you connect the model directly to your actual systems rather than describing them. In my current workflow that means GitHub, Jira, Slack, and [Synapse](https://claude.com/resources/tutorials/using-the-synapse-org-connector-in-claude) — the biomedical research platform where much of the scientific data we work with lives. The agent can query open tickets, check repository state, look up dataset metadata, and pull project context from Slack threads — all in a single session, without manual copy-pasting.

On top of that sits [Agent Skills](https://agentskills.io) — an open standard for giving agents discoverable capabilities. A skill is a folder of instructions, scripts, and context that an agent finds and uses autonomously. Instead of you providing context at the start of each session, the agent discovers what it needs as the work unfolds. As the systems change, the agent's understanding of them changes too.

The result is that the gap between "what the model knows" and "what is actually true right now" collapses.

> **Tip:** Agent Skills is adopted across 30+ tools — Claude Code, GitHub Copilot, Cursor, Databricks, and others. Skills you define once travel with you across your entire toolchain.
{: .tip}

---

## AI as Engineering Infrastructure

> **Important:** What this points toward is larger than any single tool.
{: .important}

We've seen this pattern before. Version control changed how teams collaborate on code. Continuous integration changed how software gets validated. Cloud infrastructure changed how systems get deployed. Each shift didn't just add a new tool — it changed the underlying conditions of how engineering work happens.

AI is doing something similar, but at the level of reasoning itself. Not infrastructure in the sense of servers or pipelines, but cognitive infrastructure — the systems that shape how engineers think through problems, explore ideas, and communicate complex systems to each other.

Instead of thinking alone and producing solutions, engineers increasingly work in a loop: **think → test ideas with AI → refine → implement.** The unit of work gets smaller and more exploratory.

We're still early in that transition. But once you start using AI as part of the thinking process rather than a question-answering tool, it becomes hard to imagine going back.

Less like a chatbot. More like a co-processor for engineering thought.
