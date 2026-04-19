---
layout: post
title: "Why Technical Constraints Are a Gift"
date: 2026-04-19
---

I've only been a people leader for 3-4 years, and when I first stepped into the role, I assumed the job was about unblocking people and setting direction. That's true—but incomplete.

What I didn't expect is how much of it is about shaping constraints. Left unconstrained, good developers will build… anything. And I mean that in the best way.

## Developers Will Always Choose the Interesting Problem

One of the joys of working with strong engineers is their creativity. Give them a problem like "we need to reliably schedule, run, and monitor a growing set of interdependent data pipelines" and you'll get a spectrum of solutions:

- Airflow on Kubernetes—full control, full operational burden
- AWS Step Functions—managed, but tightly coupled to AWS
- Lambda functions chained together with custom retry logic
- A workflow framework like Prefect or Dagster with its own deployment model
- Or—occasionally—a well-placed cron job

The catch is that creativity naturally gravitates toward interesting complexity, which raises the floor of technical knowledge every engineer on the team has to maintain.

As an individual contributor, that instinct is often a strength. As a manager, I'm beginning to ask different questions: Who is going to maintain this in 18 months? How long will onboarding take for a new hire? What happens when the one person who built this leaves?

And then the harder question: what happens when *I* leave?

A manager who champions a technology and then moves on doesn't just leave a gap on the team—they leave a technical inheritance for the rest of the organization. Someone has to understand it, support it, and decide whether to keep investing in it or pay the cost of replacing it. The broader the technology's footprint, the bigger that burden. And unlike an IC's contribution, a manager's technology decisions can quietly shape the org's trajectory for years.

That's where constraints come in.

## Focus Is a Finite Resource

Everyone has a finite amount of cognitive bandwidth. Time spent learning a bespoke internal platform is time not spent on the actual domain problem the team exists to solve.

If you have a team of engineers with a particular area of expertise, you want their skills compounding on those problems—not on debugging infrastructure and/or problems they didn't sign up to own.

Technical constraints are how you protect that focus. A default like "we prefer managed or widely-adopted tools unless there's a clear, long-term reason not to" means new engineers onboard to familiar territory, the team isn't dependent on one person's tribal knowledge, and cognitive load stays where it belongs.

## New Technology Is a Team-Wide Commitment

This is the part that just recently dawned on me.

When someone introduces a new technology—a new framework, a new infrastructure pattern, a new language—it's rarely just a technical decision. It's a commitment the whole team has to honor. Everyone will eventually need to understand it well enough to review code, debug it when something breaks, maintain it when the original author moves on, and onboard new hires into it.

That's a real cost. And it's often invisible to the person proposing the change, because they're excited and have already done the learning.

What makes this especially hard for me personally: I've been that person. I still am. I love exploring new tools and pushing into unfamiliar territory. But in a leadership role, I realized that my enthusiasm for a new technology can inadvertently set a direction the whole team has to follow—whether they're ready for it or not.

As a manager, I've come to learn that my job is to make that cost visible, and to ensure the whole team is aligned before it's incurred. Not "never adopt new things"—but asking: *Are we all in on this together? Does the team understand what we're signing up for?* If the answer is yes, move forward. If it's no, that's the conversation to have first.

## Constraints Don't Kill Creativity—They Redirect It

Up until now in my management journye, I was hesitant to impose constraints. It felt like limiting the team.

I'm starting to see things a little differently. When the scaffolding is decided, engineers can pour their energy into the interesting parts: the domain logic, the edge cases, the optimizations that actually matter. The creativity doesn't go away—it gets applied where it counts.

Without constraints, every project becomes a mini research effort. With them, teams build on a shared foundation instead of reinventing it each time. Decision fatigue drops. Onboarding becomes predictable. The team's knowledge concentrates where it matters.

## But What If the Manager Is the One Pushing Boundaries?

Here's a tension I haven't fully resolved: sometimes I'm the one with the new idea. I see a problem space, I get excited, and I want to explore it.

The role I'm supposed to play in those moments is different than my instincts want. When I was an engineer with a big idea, my job was to build a proof of concept and convince people. When I'm a manager with a big idea, my job is to define the *problem*—and then create space for the team to figure out how they want to solve it.

> **Important:** There's a difference between *"I think we should use X to solve this"* and *"Here's a problem I think we have—I'd love us to research it and align on an approach."* The first shortcuts the team's ownership. The second invites it.
{: .important}

Honestly though? I'm still working on this. I catch myself dictating not just what problem to solve, but the specific approach, the implementation details, the shape of the solution. That's micromanagement, even when it comes from genuine enthusiasm rather than distrust. The instinct to jump to solutions is hard to unlearn when you've spent years as the do-er.

## When Do You Actually Innovate?

This is the question I keep coming back to.

My default as an individual has always been: "do the thing that needs to get done". Work the long hours. Pick whatever technology solves the problem fastest. I'm not apologizing for that drive—it's gotten a lot done.

But the accumulated cost is a tech stack that looks like a museum of every interesting problem I've ever encountered. A different tool for each era. Each one made sense at the time. Together, they're a maintenance burden the whole team now carries.

So when *is* the right time to innovate? I don't think the answer is "never," and I don't think it's "whenever someone is motivated enough to make it work." It's when there's a genuine problem the current tools can't solve well, the team has the bandwidth to own something new, and there's real alignment—not just one person's momentum.

> **Note:** The hard part is that "we could probably make the existing thing work" is almost always true. Innovation requires making a deliberate case that the cost of staying put outweighs the cost of change. And that's a team conversation, not a solo decision made during hundred-hour weeks.
{: .note}

## How AI has Changed Things—But Not How You'd Expect

AI tools are often framed as a solution to complexity. Need to understand a sprawling codebase? Feed it to the model. Need to onboard to five different tools at once? Ask the AI.

And yes—AI can absorb massive amounts of context. But I've started to think that's the wrong frame.

> **Note:** The more constrained your stack, the more effective AI becomes. If an engineer is working within a focused, well-understood set of tools, AI can spend its context on the actual problem—the business logic, the edge case, the data transformation—instead of burning it on "how does our custom orchestration layer work again?"
{: .note}

A sprawling tech stack doesn't disappear when you introduce AI. It just becomes AI's problem too. The cognitive overhead that slows down human engineers shows up in the same way for AI-assisted workflows—more context to load, more ambiguity to resolve, slower iteration on the thing that actually matters.

Constraints make humans faster. They make AI-assisted development faster too. Less noise, more signal, tighter feedback loops on the exact problem that needs to be solved.

## The Shift from Builder to Steward

As an IC, success looks like building something impressive that is intuitive. As a leader, I'm still learning that thsi looks like systems that are easy to maintain, teams that onboard quickly, and decisions that age well.

That shift is uncomfortable. I have to start saying "no" to technically exciting ideas in favor of simpler, more durable ones. But the payoff shows up over time—fewer late-night incidents, less tribal knowledge, more predictable delivery.

Developers will always find the most creative path forward. I recently realized one of my roles as a manager is to make sure that creativity lands where it matters most—on the actual problems that are correlated to the team's expertise.

> **Important:** Technical constraints aren't a cage. They're a way of saying: *we trust you to do great work, and we're going to protect the space for you to do it.*
{: .important}
