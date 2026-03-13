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

But the workflow always had friction.

Every conversation existed in isolation.

Each time a problem arose, the process started from scratch: paste the relevant code, explain the architecture again, reconstruct the context. Even when the model was helpful, the interaction never quite integrated with the rest of the work.

The chat window was a separate universe.

That limitation didn't matter much at first. But as AI became more embedded in the workflow, the fragmentation became harder to ignore.

---

## Engineering Work Is Mostly Context

The deeper problem was that engineering rarely happens in small, isolated snippets.

Most real work involves navigating context:

- repositories
- documentation
- infrastructure definitions
- datasets
- metadata schemas
- pipelines and orchestration logic

Understanding a system means understanding how all of those pieces relate to each other.

Chat interfaces flatten that complexity.

You can paste pieces of context into a conversation, but the system itself never lives inside the environment where the work is happening. The model only sees what you choose to show it in that moment.

That's useful for quick questions, but it breaks down when AI becomes part of the thinking process.

Because once you start using AI as a collaborator, the missing context becomes the biggest bottleneck.

> **Note:** This isn't a model problem — it's an interface problem. The models improved dramatically over this period. The workflow stayed the same.
{: .note}

---

## The Moment the Workflow Changes

At some point, the relationship with AI shifts.

Instead of asking:

> "Can this tool answer my question?"

You start asking:

> "Where should AI live in the workflow?"

That's a very different problem.

The first version of AI tools assumed the interface would always be chat. But chat is optimized for conversation, not for reasoning about complex systems with many moving parts.

Engineering work needs something closer to a workspace.

A place where code, documents, architecture diagrams, datasets, and conversations all exist together.

Without that shared context, every interaction starts with reconstruction.

---

## Moving Toward an AI Workspace

More recently, I've been experimenting with a workflow centered around Claude.

The interesting change isn't simply model capability. It's the idea of working with artifacts instead of isolated conversations.

Instead of starting every interaction with a blank chat window, the work begins with the things you're already building: documents, code, datasets, and structured ideas.

The AI then becomes something that can operate within that environment, rather than outside of it.

That small shift has surprising consequences.

You can evolve documents collaboratively instead of rewriting them from scratch. Code and explanations live alongside each other. Context accumulates rather than disappearing with each conversation.

The system starts to feel less like a chatbot and more like a persistent workspace for reasoning.

---

## AI as Engineering Infrastructure

What this points toward is something larger than a single tool or model.

AI is slowly becoming part of the infrastructure of technical work.

Not infrastructure in the sense of servers or pipelines, but in the sense of cognitive infrastructure—the systems that support how engineers think, explore ideas, and communicate complex systems.

We've seen similar shifts before.

Version control changed how teams collaborate on code. Continuous integration changed how software gets validated and shipped. Cloud infrastructure changed how systems get deployed and scaled.

AI may end up changing something more fundamental: how engineers reason through problems in the first place.

Instead of thinking alone and producing solutions, engineers increasingly work in a loop:

**think → test ideas with AI → refine → implement.**

> **Tip:** This loop works best when AI has access to the full context of what you're building — not just the snippet you pasted. The closer the AI lives to your actual work, the tighter the loop.
{: .tip}

The cycle becomes faster, more exploratory, and more conversational.

---

## The Future of AI Workflows

If this trajectory continues, the next generation of AI tools won't feel like chat interfaces at all.

They will look more like integrated environments where codebases, documentation, datasets, architecture discussions, and reasoning processes are all connected.

In that world, AI stops being something you consult occasionally.

It becomes something that exists continuously inside the systems where work happens.

Less like a chatbot.

More like a co-processor for engineering thought.

We're still early in that transition.

But once you start using AI as part of the thinking process rather than just a question-answering tool, it becomes hard to imagine going back to the old workflow.
