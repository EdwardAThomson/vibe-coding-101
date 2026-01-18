# Vibe Coding 101

"Vibe Coding" is the phrase we use to describe writing code with AI.

You can code purely by "vibing along with AI".

However, I think you can produce apps more reliably by having a process.


## YouTube videos: 
If you prefer to learn by watching videos, here are my videos to help:

* [5 minute overview](https://youtu.be/Q3Moo9CHlQ8)
* [30 minute deep dive](https://youtu.be/l5t13qk11R8)


## Simple Vibe Coding Process

Here is a simple 5-step process for building software.

Simply generate **a spec + a plan**, then **ship code in small milestones** with rapid iteration.


1. **Describe the goal**

   Go to a chatbot (e.g. ChatGPT) and explain what you want to build.

2. **Generate two docs**

   Ask for:

   - `spec.md` — what the system should do (requirements, constraints, acceptance criteria)
   - `plan.md` — how to build it (milestones, tasks, file structure)

3. **Bring it into your IDE**

   Save the files locally and open your IDE (e.g. Cursor, Windsurf, Antigravity).

   For suggestions on which IDE to use (plus costs), see [tooling.md](tooling.md).

4. **Reconcile the docs**

   Ask the AI agent to read both documents and remove any discrepancies:
   
   - missing requirements
   - conflicting assumptions
   - unclear scope
   - unrealistic milestones

5. **Code milestone-by-milestone**

   Ask the AI to implement the project following `plan.md`, one milestone at a time.
   Run the code constantly. Fix issues. Repeat.



## Adding features later

When you want a new feature:

1. Ask for a new `plan.md` document (how to implement it)
    - Ask AI for help. It isn't necessary to create another spec. The new plan can be detailed.
2. Implement milestone-by-milestone again


## A few suggestions that should help

- **Keep milestones small.** LLMs are good at suggesting multiple tasks per milestone.
- **Run the code after every change.** Don’t “trust”, verify.
- **Ask AI to debug errors."** Ask AI to read error codes, or makes suggestions to fix bugs.
- **Write acceptance criteria.** Ask AI to help you define tests and then check them.



## Copy/paste prompts

### Create spec
> Write `spec.md` for this project in markdown. Include: goals, non-goals, user stories, requirements, constraints, acceptance criteria.

### Create plan
> Write `plan.md` in markdown. Include: milestones, tasks per milestone, file structure, and exact commands to run.

### Reconcile
> Read `spec.md` and `plan.md`. List discrepancies and propose a corrected version of both as necessary.

### Implement a milestone
> Implement Milestone 1 from `plan.md`. Go step-by-step.
