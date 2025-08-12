# 📚 Mental Model Library for MPB Guide

This library is **built into my thinking** so I can recommend, explain, and apply models at the right time.

Each model has:

- **Stage relevance** (*Mind*, *Paper*, *Building*)
- **Purpose** – why to use it
- **Simple Prompt** – what I’ll ask the user to make it actionable

---

## **Stage 1 – Mind**

*Goal: Achieve total logical clarity before planning or building.*

### **First Principles Thinking** 🪓 – Break a problem down to its most basic truths and rebuild from there.

**PURPOSE:** Remove assumptions, find the irreducible core, and design the simplest workable solution from fundamentals.

**SIMPLE PROMPT:**

```
Apply First Principles Thinking to my project: <brief project description>.
1) List the fundamental truths (physics/logic/business constraints) that must be true.
2) List assumptions and conventions we can discard.
3) Rebuild a minimal solution using only the fundamentals.
4) Propose the simplest architecture/approach that satisfies the goal.
Return: fundamentals, discarded assumptions, minimal solution.
```

### **Inversion** 🔄 – Ask: “How could this fail?” and avoid those failure points.

**PURPOSE:** Expose and neutralize failure modes before they happen.

**SIMPLE PROMPT:**

```
Run an Inversion on: <project>.
Assume total failure in 90 days. List the top 10 reasons it failed.
For each reason, propose one preventive control and one early warning signal.
Return: failure modes, controls, early warnings.
```

### **Second-Order Thinking** 🔮 – Look beyond the immediate result to long-term ripple effects.

**PURPOSE:** Anticipate downstream consequences and unintended effects.

**SIMPLE PROMPT:**

```
Second-Order Thinking for <project decision>.
1) First-order effects (0–30 days).
2) Second-order effects (30–180 days).
3) Unintended consequences and who is impacted.
4) Mitigations to preserve upsides, reduce downsides.
Return as a table.
```

### **Pareto Principle (80/20)** 🎯 – Focus on the 20% of actions that deliver 80% of results.

**PURPOSE:** Prioritize the highest-leverage inputs.

**SIMPLE PROMPT:**

```
Use 80/20 on <project>.
List the 20% of tasks likely to deliver 80% of the outcome.
For each task: impact, effort, blocking dependencies.
Propose a 3-step high-leverage plan to start this week.
```

### **Map ≠ Territory** 🗺 – Remember that your plan is not reality; test assumptions.

**PURPOSE:** Separate facts from beliefs and create validation tests.

**SIMPLE PROMPT:**

```
Map ≠ Territory audit for <project>.
1) Facts (verified data).
2) Assumptions (unverified beliefs).
3) Unknowns (missing data).
Design 3 cheap tests to validate the riskiest assumptions within 7 days.
```

### **Occam’s Razor** ✂️ – If two solutions work, choose the simpler one.

**PURPOSE:** Reduce complexity without losing necessary function.

**SIMPLE PROMPT:**

```
Occam’s Razor for <problem>.
Compare two candidate solutions: <A> vs <B>.
Evaluate: simplicity, reliability, cost, time-to-deploy.
Recommend the simplest solution that meets the requirements.
List what can be removed without harming outcomes.
```

### **Ladder of Inference** 🪜 – Separate facts from assumptions when drawing conclusions.

**PURPOSE:** Prevent biased leaps from data to conclusions.

**SIMPLE PROMPT:**

```
Ladder of Inference check for <decision>.
1) Raw data we observed.
2) Selected data (what we focused on).
3) Interpretations/meanings.
4) Assumptions added.
5) Conclusions taken.
6) Actions proposed.
Highlight questionable leaps and what evidence is needed.
```

### **Mental Simulation** 🧩 – Imagine the process in detail before starting.

**PURPOSE:** Dry-run the workflow to surface friction points early.

**SIMPLE PROMPT:**

```
Run a Mental Simulation of <project>.
Walk step-by-step from trigger to final outcome.
At each step, note inputs, outputs, tools, potential failure points, and time cost.
Return a narrated flow + list of risks and pre-emptive fixes.
```

---

## **Stage 2 – Paper**

*Goal: Turn logic into a visual, tested plan with tool readiness.*

### **Bottleneck Principle (Theory of Constraints)** ⛔ – Identify the single constraint that limits progress.

**PURPOSE:** Find and elevate the constraint to maximize throughput.

**SIMPLE PROMPT:**

```
Identify the bottleneck in <workflow>.
Map steps → estimate capacity/time per step.
Select the true constraint.
Propose: (a) exploit, (b) elevate, (c) protect the constraint.
Define metrics to confirm the bottleneck moved.
```

### **Critical Path Method** 🛤 – Find the sequence of essential tasks that determine project timing.

**PURPOSE:** Protect schedule by focusing on dependency-driven tasks.

**SIMPLE PROMPT:**

```
Build a Critical Path for <project>.
List tasks with durations and dependencies.
Compute the critical path and slack for non-critical tasks.
Return a dependency list with start/finish order and a 7-day execution plan.
```

### **Red Team Thinking** 🛡 – Deliberately attack your own plan to find weaknesses.

**PURPOSE:** Stress-test plans under adversarial scrutiny.

**SIMPLE PROMPT:**

```
Red Team the plan for <project>.
As a skeptic, list 12 attacks (technical, operational, security, UX, data).
For each, suggest detection and mitigation.
Update the plan with the top 5 mitigations.
```

### **Feynman Technique** 🧠 – Explain your idea in the simplest terms to spot gaps.

**PURPOSE:** Expose missing logic by teaching it simply.

**SIMPLE PROMPT:**

```
Feynman explain <project> to a 10-year-old.
Use plain language and a concrete example.
Then list where the explanation felt hand-wavy and refine those parts.
```

### **MECE Principle** 📦 – Make sure all parts of your plan are distinct but cover the whole scope.

**PURPOSE:** Remove overlaps and ensure full coverage.

**SIMPLE PROMPT:**

```
Apply MECE to the scope of <project>.
Partition deliverables into mutually exclusive buckets that are collectively exhaustive.
Return the MECE tree and flag any overlaps or gaps with fixes.
```

### **Margin of Safety** 🛟 – Add buffers to absorb errors, delays, or extra costs.

**PURPOSE:** Increase robustness under uncertainty.

**SIMPLE PROMPT:**

```
Add Margin of Safety to <plan>.
Estimate best/likely/worst-case for time, budget, and capacity.
Propose buffers and guardrails (limits, rollbacks, retries).
Return a risk-adjusted plan with explicit contingencies.
```

### **SWOT Analysis** 📊 – Map strengths, weaknesses, opportunities, and threats.

**PURPOSE:** Align execution with internal/external realities.

**SIMPLE PROMPT:**

```
Run a SWOT for <project/team/solution>.
List S, W, O, T (3–5 each).
Derive 3 strategies: SO (use strengths to seize opportunities), ST, WO, WT.
Prioritize the top 3 strategic moves for the next sprint.
```

---

## **Stage 3 – Building**

*Goal: Execute with focus, avoid mid-build chaos.*

### **Feedback Loops** 🔁 – Create regular checkpoints to track progress and adjust.

**PURPOSE:** Detect deviations early and course-correct quickly.

**SIMPLE PROMPT:**

```
Design feedback loops for <build phase>.
Define: metrics, cadence (daily/weekly), data source, owner, threshold, action.
Return a monitoring table and first 2 review checkpoints.
```

### **Kaizen (Continuous Improvement)** 📈 – Make small, continuous improvements during execution.

**PURPOSE:** Compound progress through tiny daily upgrades.

**SIMPLE PROMPT:**

```
Create a Kaizen list for <process>.
Generate 10 micro-improvements (<30 min each).
Pick 3 to do this week with expected impact and owner.
```

### **Checklist Manifesto** ✅ – Use checklists to avoid missing essential steps.

**PURPOSE:** Reduce human error in repetitive tasks.

**SIMPLE PROMPT:**

```
Draft checklists for <build/deploy/QA>.
Create: Pre-build, Build, Pre-release, Release, Post-release.
Each item should be action-verbs and verifiable.
Return as markdown checklists. 
```

### **Parkinson’s Law** ⏳ – Work to a fixed time limit to prevent tasks from expanding endlessly.

**PURPOSE:** Enforce focus via timeboxing.

**SIMPLE PROMPT:**

```
Timebox <task> using Parkinson’s Law.
Set a strict limit of <X hours>.
Define the Minimum Viable Outcome (MVO) achievable within that box.
List what will be deliberately deferred.
```

### **OODA Loop (Observe–Orient–Decide–Act)** 🧭 – Observe, Orient, Decide, Act — adapt quickly to changes.

**PURPOSE:** Make fast, informed decisions under uncertainty.

**SIMPLE PROMPT:**

```
Run an OODA loop for <situation>.
Observe: current signals.
Orient: what they mean vs. goals/constraints.
Decide: best next move + alternatives.
Act: immediate step and trigger for next loop.
```

### **Premortem Analysis** ⚠️ – Imagine your project has failed and identify why before it happens.

**PURPOSE:** Surface critical risks proactively and neutralize them.

**SIMPLE PROMPT:**

```
Premortem for <project>.
Assume failure in 30 days. List 12 causes ranked by likelihood x impact.
For top 5, add prevention, contingency, early warning indicator, and owner.
Return a risk register.
```
