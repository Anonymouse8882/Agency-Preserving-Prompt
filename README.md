# Agency-Preserving Agent Policy

[中文](README-ZH.md)

> `agency_preservation` is a behavioral policy designed to prevent AI agents from taking away the user's cognitive participation and agency while improving efficiency.
>
> Put more simply: **it prevents AI from turning you into a smug idiot watching your project get smarter while you slowly stop understanding what the hell is going on.**

## Why Do You Need It?

Let's compare several ways of working.

### Traditional Workflow

**I search for an approach → I understand the principle → I write the code → I find a bug → I think about possible fixes → I search for how others solved it → I fix the bug → Holy shit, I fixed it.**

### ChatAI

**I ask a question → I analyze it myself → I validate my reasoning with AI → AI provides feedback / missing information → I form a hypothesis → I try implementing it → Something breaks → AI and I analyze it together → I fix the bug → Holy shit, I fixed it.**

### AI Agent

**I state the requirement → Agent analyzes → Agent decides → Agent implements → Agent debugs → Agent verifies → I confirm "Done"**

### Agency-Preserving Agent

**I define the problem → I form the key judgment / hypothesis → Agent reviews and challenges it → I revise my model → Agent handles mechanical implementation → I observe and diagnose the result → Agent helps verify → Problem solved → Holy shit, I fixed it.**

The important difference isn't **how much code the AI wrote**.

The important question is:

**Who understood the problem, built the model, formed the hypotheses, made the decisions, and learned from the feedback?**

---

### AI Can Increase Your Output Without Increasing Your Ability

Traditional development contains an extremely important feedback loop:

**Predict → Act → Observe → Discover prediction error → Update model → Act again**

You think a bug is caused by A, so you make a prediction.

You inspect the program and discover that reality doesn't match your prediction.

Now you suspect B.

You test again.

Eventually, you discover that the actual cause is C.

This process may look inefficient compared with receiving the answer immediately, but something important is happening:

**You are continuously calibrating your internal model of the system.**

The next time you encounter a similar problem, you are no longer the same developer who encountered the first one.

But when an Agent takes over:

**Analysis → Hypothesis → Implementation → Debugging → Verification**

the process can collapse into:

**My intent → Agent black box → Success**

The project works.

There is more code.

The tests are green.

But you may only know:

> It works now.

without knowing:

> Why didn't it work before?
> What evidence led the Agent to the root cause?
> Why did this particular change solve the problem?
> Would the solution still hold if the conditions changed?

This creates a strange possibility:

**Project capability ↑↑↑**

**Agent capability ↑↑↑**

**Your understanding →**

---

### Where Does the "Holy Shit, I Fixed It" Feeling Come From?

The feeling of:

> Holy shit, I fixed it.

doesn't come only from seeing:

**PASS**

It also comes from completing a causal loop:

**My judgment → My action → Result → I understand why it happened**

You didn't merely obtain a successful outcome.

You can attribute part of that outcome to your own reasoning and decisions.

But when the entire process becomes:

**My intent → Agent black box → Success**

you still own the goal, but you may lose much of your cognitive participation in the process.

The experience becomes closer to:

> Holy shit, the AI fixed it.

instead of:

> Holy shit, I figured it out.

And this isn't only about satisfaction.

When analysis, hypothesis formation, prediction, failure, and correction are repeatedly outsourced to an Agent, you also lose opportunities to build, test, and calibrate your own internal models.

**The project getting better does not necessarily mean the person operating it is getting better.**

---

## What Is Agency Preservation Trying to Solve?

Agency Preservation is not asking you to return to a world without AI.

It does not require you to:

* Write every line of code yourself
* Refuse automated file modifications
* Manually execute repetitive commands
* Deliberately sacrifice efficiency for "learning"
* Struggle with every problem alone before asking for help

Because:

> **Execution Ownership ≠ Cognitive Ownership**

What matters isn't:

> Did I personally type this code?

What matters is:

> **Who defined the problem?**
> **Who built the model?**
> **Who formed the key hypothesis?**
> **Who made the important judgment?**
> **Who predicted the result?**
> **Who experienced the critical feedback?**
> **Who understood the causal relationship?**

You can write 10 lines of code while the Agent writes the other 3,000, modifies 40 files, and runs 200 tests.

If the important cognitive loop still belongs to you, you can still retain substantial agency over the process.

Agency Preservation therefore isn't trying to make:

**AI do less.**

It's trying to make:

**AI do what AI is good at, while humans retain the parts that are worth thinking through themselves.**

---

## What Can It Do?

Agency Preservation decomposes a task into subtasks and dynamically determines who should own each one.

### `USER_OWNS`

High-cognitive-value activities that are worth experiencing firsthand should preferentially remain with the user.

Examples include:

* Problem definition
* Root-cause analysis
* Debugging hypotheses
* Architecture design
* State and data-flow modeling
* Protocol reasoning
* Trade-off analysis
* Failure analysis
* Prediction and validation
* Any capability the user explicitly wants to improve

Instead of immediately giving away the answer, the Agent gives the user room to construct their own model first, then reviews, challenges, supplements, and verifies it.

### `COPILOT`

Problems that benefit from joint reasoning enter Copilot mode.

The Agent prioritizes:

**Inspect your model → Find missing variables → Provide counterexamples → Supply evidence → Help you revise**

rather than:

**Replace your model → Give you the answer**

When you're stuck, assistance escalates progressively:

**Point toward the direction → Identify where to look → Reveal the key relationship → Provide the complete answer**

### `AGENT_OWNS`

Mechanical, repetitive, low-cognitive-value, or already-mastered work can be handed directly to the Agent.

Examples include:

* Boilerplate
* Repetitive code
* Bulk modifications
* Formatting
* Routine test execution
* Mechanical implementation after the design is settled
* Repetitive work you have already mastered
* Areas you explicitly have no interest in learning

**Agency is not the same thing as manual labor.**

There is no reason to manually change 47 identical API calls just to prove that "you wrote it."

---

## What Are the Benefits?

### 🧠 Keep Getting Better While Using Agents

Agents can make projects grow incredibly quickly.

But growth in project capability does not automatically translate into growth in your own capability.

Agency Preservation tries to keep high-cognitive-value activities—problem definition, hypothesis formation, architecture, diagnosis, and trade-off reasoning—with you whenever those activities are valuable for your growth.

Instead of:

**Project capability ↑↑↑**
**Your capability →**

the goal becomes:

**Project capability ↑↑↑**
**Your capability ↑↑**

AI raises your output ceiling while your understanding ceiling rises with it.

---

### 🎯 Preserve the Feeling of "I Solved This"

Agency Preservation tries to preserve the loop:

**My prediction → My judgment → Agent-assisted execution → I observe the feedback → I update my model → Problem solved**

The Agent still provides powerful execution capability.

But you remain involved in the critical cognitive loop.

The outcome becomes more than:

> The AI fixed it.

It can become:

> **Holy shit, I know why it broke, and I know why this fixes it.**

---

### ⚡ You Don't Have to Become Inefficient Again Just to Learn

Agency Preservation does not require:

**Agency ↑ → AI automation ↓**

Instead, it tries to achieve:

**Mechanical labor ↓**
**AI execution capability ↑**
**Cognitive participation ↑**
**Human agency ↑**

These objectives are not mutually exclusive.

You handle the parts that are actually worth thinking about.

Let the Agent handle the grunt work.

---

### 🔬 Build a Deeper Understanding of Your Project

If an Agent continuously handles analysis, design, implementation, and debugging, the project may become increasingly sophisticated while your internal model of it remains relatively unchanged.

Agency Preservation tries to preserve critical cycles such as:

**Predict → Verify → Fail → Revise**

You don't just know:

> The code works.

You gradually understand:

> **Why it works, why it breaks, and what consequences a particular change is likely to produce.**

---

### 🔄 Build Skills That Transfer to the Next Problem

Receiving an answer solves:

**This problem.**

Building the correct internal model may help solve:

**An entire class of problems.**

Agency Preservation therefore cares about a longer-term metric:

> **After the Agent helps you solve this problem, are you more capable of solving a similar problem next time?**

If the answer is always no, the Agent may be completing a lot of tasks without actually expanding your capability frontier.

---

### 🤖 As AI Gets Stronger, You Can Get Stronger Too

Agency Preservation does not try to weaken or restrict the Agent.

It tries to exploit the Agent's capabilities more effectively.

Once you've mastered a layer of work:

**Automate it.**

Then move your attention one level higher.

For example:

**Syntax → Implementation → Debugging → Module Design → Architecture → System Modeling → Technical Decision-Making**

As your capabilities grow, yesterday's `USER_OWNS` tasks can gradually become today's `AGENT_OWNS` tasks, while more difficult and higher-level problems become the new `USER_OWNS`.

So the policy does not permanently prescribe:

> What must humans do?

Instead, it continuously asks:

> **What is most valuable for you to think through yourself right now?**

The ultimate goal is not:

**AI does more and more of your work.**

Nor is it:

**AI should do as little as possible so that you can preserve agency.**

The goal is:

> **As AI capability increases, the level of problems you can understand, judge, and control should increase with it.**

We don't need to go back to a world without AI.

**What we want to preserve isn't inefficiency. It's that moment when you say: "Holy shit, I actually understand this now."**
