# AI Project Drift Control

## *Preface*

This is not a manual for AI.
It’s a description of how I have success with it.

I don’t treat AI as an oracle, a shortcut, or a replacement for thinking.
I arrived at that position by finding out for myself what happens when it’s used that way — and what breaks.

What works better for me is treating AI as a system I interact with:
one that responds well to clear questions, constraints, and feedback, and poorly to vague intent.

Everything in this guide reflects a pattern that’s worked for me across real projects, including building an Android app that decodes live weather radar data on-device and renders it with OpenGL. More importantly, it reflects a process I’ve been able to repeat.

That process is simple:

- I ask for recommendations

- I ask why those recommendations make sense

- I ask what assumptions, tradeoffs, and limitations exist

- I check alignment with scope, constraints, and sources of truth

Only then do I act

This isn’t about knowing the “right” answer up front.
It’s about setting up a process where bad answers surface early, good answers are explainable, and progress compounds instead of drifting.

You don’t need to copy my workflow exactly.
You don’t need to use the same tools.
And you definitely don’t need to agree with every choice I make.

If you get anything out of this, I hope it’s not specific prompts or tactics, but a clearer sense of how I approach working with AI:

- slowing down just enough to avoid mistakes

- asking better questions

- using AI to explore decisions instead of guessing them

- and keeping long projects from slowly going off the rails

That’s it.
-- Slasaa

## 1. Context Control

### *How I Think About This*

I treat chats as temporary working memory.

### *What I Do*

Keep one clear purpose per chat

Delete chats that drift or hallucinate

Archive good chats at natural milestones

### *Example Prompts I Use*

```
"This chat has one purpose: designing the database schema."

"If we drift, stop and remind me."

"We’ve finished initial planning. Summarize the validated decisions so I can archive this chat."
```

### *Why This Works for Me*

I preserve signal and eliminate noise.

---

## 2. Setting the Rules

### *How I Think About This*

I ask AI to help evaluate constraints before locking them.

### *Example Prompts I Use*

```
Give me 3 viable constraint options.

For each, explain:

- why someone would choose it
- what it limits later
- when it would fail

Which option best fits these goals, and why?
```

### *Why This Works for Me*

I understand decisions before committing.

---

## 3. Drift Detection

### *How I Think About This*

Drift starts when exploration stops too early.

### *Example Prompts I Use*

```
"Pause. List any assumptions you’re making right now."

"Are we still operating within the original constraints?"
```

### *Why This Works for Me*

I catch issues early.

---

## 4. Drift Correction

### *How I Think About This*

I correct reasoning, not just answers.

### *Example Prompts I Use*

```
"Stop. Back up and restate the problem using only validated information."

"Re-explore alternatives instead of continuing this path."
```

### *Why This Works for Me*

Fixing reasoning fixes output.

---

## 5. Structured Prompting

### *How I Think About This*

I structure prompts to explore decisions step by step.

### *Example Prompts I Use*

```
"Don’t solve yet. First give me an outline of options only."

Expand option 2 and explain tradeoffs.
```

### *Why This Works for Me*

Understanding beats guessing.

---

## 6. Verification & Testing

### *How I Think About This*

Verification applies to decisions as much as outputs.

### *Example Prompts I Use*

```
"List every assumption this decision relies on."

"Under what conditions would this approach break?"
```

### *Why This Works for Me*

Verified decisions age better.

---

## 7. Role-Based Chats

### *How I Think About This*

Some chats explore decisions. Others execute them.

### *Example Prompts I Use*

```
"Your role in this chat is decision exploration only."

"Do not write code."

"Your role is implementation only. Follow locked decisions exactly."
```

### *Why This Works for Me*

Clear roles produce clear outcomes.

---

## 8. Reset & Recovery

### *How I Think About This*

Archive good state. Delete bad state.

### *Example Prompts I Use*

```
"Summarize the clean, validated state so I can archive this chat."

"Start fresh with only this information as context"
```

### *Why This Works for Me*

State discipline prevents mistakes.

---

## 9. Precision Control

### *How I Think About This*

Different decision stages require different zoom levels.

### *Example Prompts I Use*

```
"High-level overview only. No details yet."

"Now zoom in and give exact steps."
```

### *Why This Works for Me*

Correct zoom prevents confusion.

---

## 10. Noise Reduction

### *How I Think About This*

Noise hides tradeoffs.

### *Example Prompts I Use*

```
"Ignore everything except the following snippet:"

"Do not include background explanation. Focus only on the decision."
```

### *Why This Works for Me*

Less noise reveals better options.

---

## 11. Thinking in Structures

### *How I Think About This*

I structure decisions the same way I structure systems.

### *Example Prompts I Use*

```
"Compare options in a table with pros, cons, and implications."

"List constraints as bullet points."
```

### *Why This Works for Me*

Structure makes reasoning visible.

---

## 12. Phase-Based Workflows

### *How I Think About This*

Early phases are for deciding. Later phases are for building.

### *Example Prompts I Use*

```
"We are in planning phase only. No code."

"Decisions are locked. Proceed to implementation."
```

### *Why This Works for Me*

Clear decisions turn execution into follow-through instead of problem-solving.

---

## From Operator Habits to Project Workflow

*Up to this point, everything has been about how I work with AI at the session level.*

Part I focuses on habits:

- how I ask questions

- how I detect drift

- how I control scope

- how I decide when to reset, archive, or stop

- how I ask how to keep AI useful instead of noisy

Those behaviors apply everywhere — regardless of project size, language, or tool.


### *What Changes in Part II*

*Part II zooms out.*

Instead of looking at individual interactions, this section looks at projects that last:

- projects with multiple phases

- projects with changing context

- projects where mistakes compound if they aren’t captured

- projects where AI is used repeatedly over time

The question shifts from:

*“How do I ask how to keep this conversation productive?”*

to:

*“How do I ask how to keep this project coherent across weeks, resets, tools, and agents?”*


### *The Key Shift*

In Part I, control comes from how I interact.

In Part II, control comes from what I externalize:

- sources of truth

- documentation

- decisions

- environments

- plans

- versioned states

This is where AI stops being just a conversational partner and becomes part of a system.


### *What This Section Is (and Isn’t)*

Part II is not:

- a rigid process

- a project management framework

- a claim about the “right” way to build things

It is:

- how I’ve learned to keep long-running work from drifting

- how I make progress survive context resets

- how I decide what gets locked, documented, versioned, or paused

- how I use AI across planning, execution, and iteration without losing control

Everything here still follows the same pattern:
**ask → explain → decide → act**

The difference is that the decisions now outlive a single chat.


Each section stands on its own, but together they describe a workflow where:

- planning is explicit

- execution is controlled

- reality is observable

- decisions are durable

- and stopping points are intentional

### *Part I helps keep a session on the rails,*
### *Part II is about keeping an entire project there.*

---

## 13. Project Setup & Early Planning

This is where I spend time before building anything.
I’ve found that the quality of this phase has a direct impact on how stable everything feels later.

I don’t start by asking AI to build.
I start by making sure we agree on what is real.

## 13.1 Establishing the Source of Truth

*This is the most important step in my workflow.*

- Before I design, plan, or write code, I establish the source of truth that the project must follow.
- When this is clear, everything else becomes easier to reason about.

### *How I Think About This*

AI is very good at reasoning.
AI is not responsible for deciding what reality should be.

If the project isn’t explicitly anchored to external truth, the model will naturally:

- blend similar standards together

- rely on older versions

- fill gaps with reasonable assumptions

- sound confident while missing details

Because of that, I don’t leave this open-ended.
I deliberately anchor the project to authoritative sources up front.

Before building anything, I ask questions like:

```
"What official specifications or standards apply here?"

"Are there ICDs, RFCs, or formal docs?"

"Which sources are authoritative vs informal?"

"What version is current?"

"What has changed recently?"

"What are common edge cases or constraints?"
```

If the project is technical, this usually means:

- official documentation

- published specs

- standards bodies

- vendor docs

- source repositories

If the project is less formal, I still anchor to:

- best practices

- widely accepted conventions

- clearly stated assumptions

Sometimes I run one or two deep research passes before doing any design work.
That upfront clarity consistently pays off later.

### *Example Prompts I Use*

```
"List the official or authoritative sources relevant to this project."

"Separate formal specs from informal guidance."

"Which of these sources should be treated as the source of truth, and why?"

"What version is current, and what has changed recently that people often miss?"

"Based on these sources, list the non-negotiable constraints I should not violate."
```

### *What I Avoid*

- Letting AI invent APIs, fields, or rules

- Treating informal posts as authoritative

- Mixing multiple specs without acknowledging conflicts

- Assuming defaults are always correct

### *Why This Works for Me*

Once the source of truth is established:

- reasoning stays grounded

- drift is easier to notice

- decisions are easier to explain

- verification has a clear reference point

- long-term changes are easier to manage

This step gives everything else a stable footing.

---

## License

This work is licensed under the  
**Creative Commons Attribution–NonCommercial 4.0 International (CC BY-NC 4.0)** license.

You’re free to share and adapt it for non-commercial use with attribution.
