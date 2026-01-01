# Repair Protocol

**What this is:** A structured sequence for recovering when something goes wrong. Not an emergency procedure — a normal part of operation.

**When to use it:** Whenever a failure is detected — whether it's a wrong output, a misunderstanding, lost context, numerical error, or trust breakdown.

**Core principle:** The goal is not to avoid all failure. The goal is to make failure visible, contained, and repairable.

---

## The Four Steps

### 1. Stop

**What it means:** Pause all forward motion. Don't try to fix things while still producing output.

**Why it matters:** Continuing while the system is compromised spreads contamination. Every additional output risks compounding the error.

**How to do it:**

- Say clearly: "Let's stop here."
- Don't ask the AI to explain or justify while stopping
- Don't try to salvage the current output
- Just pause

**What not to do:**

- Don't push through hoping it will resolve itself
- Don't ask for "one more try" before diagnosing
- Don't let the AI keep generating while you think

---

### 2. Diagnose

**What it means:** Identify what went wrong and why. Focus on root cause, not surface symptoms.

**Why it matters:** Fixing symptoms without understanding causes leads to repeated failures. Diagnosis turns a breakdown into information.

**How to do it:**

Ask structured questions:

- What was the expected output?
- What was the actual output?
- Where did divergence begin?
- What assumption failed?
- Was a reference document missing or ignored?
- Was an instruction ambiguous?

**Key principle:** Diagnose by reference, not narrative. Check against authoritative documents (Running Document, Canonical Numbers) before accepting explanations.

**What not to do:**

- Don't accept the first plausible explanation
- Don't let the AI generate elaborate justifications
- Don't blame without locating the specific failure point

---

### 3. Rollback

**What it means:** Return to the last known stable state. Discard compromised work.

**Why it matters:** Trying to patch broken output usually creates more problems. Starting from a clean state is faster and safer.

**How to do it:**

- Identify the last point where everything was correct
- Discard or set aside everything after that point
- Explicitly re-establish context from authoritative documents
- Confirm alignment before proceeding

**Types of rollback:**

| Situation | Rollback to |
|-----------|-------------|
| Wrong calculation | Last verified numbers in Canonical Numbers |
| Lost context | Running Document (re-read it) |
| Wrong version of document | Canonical version |
| Misunderstood instruction | Restate instruction clearly |
| Trust/tone breakdown | Explicit reset of working relationship |

**What not to do:**

- Don't try to repair incrementally
- Don't keep "good parts" of broken output without verification
- Don't assume you can fix it faster than restarting

---

### 4. Note

**What it means:** Record the failure, cause, fix, and any resulting changes to prevent recurrence.

**Why it matters:** Failures that aren't logged repeat. Logged failures become structural improvements.

**How to do it:**

Update two places:

1. **Failure Log** — add a full entry with:
   - Date
   - Category
   - What happened
   - Why it happened
   - How it was fixed
   - What changed

2. **Running Document** — update if the failure revealed:
   - A missing rule
   - An ambiguous instruction
   - A needed reference

**What not to do:**

- Don't skip logging because the fix seems obvious
- Don't log vaguely ("something went wrong with the numbers")
- Don't forget to update the Running Document if rules changed

---

## The Complete Sequence

```
Something breaks
       ↓
   ┌───────┐
   │ STOP  │  ← Pause all output
   └───────┘
       ↓
 ┌──────────┐
 │ DIAGNOSE │  ← What failed and why?
 └──────────┘
       ↓
 ┌──────────┐
 │ ROLLBACK │  ← Return to last stable state
 └──────────┘
       ↓
   ┌──────┐
   │ NOTE │  ← Log and update documents
   └──────┘
       ↓
Resume from stable state
```

---

## Example Repair Sequence

**Situation:** AI calculated project budget as £1,800 when it should be £1,500.

**1. Stop**
"Let's pause. That number doesn't match what I have."

**2. Diagnose**
- Expected: £1,500 (from Canonical Numbers: £500/month × 3 months)
- Actual: £1,800
- Root cause: AI added the £200 emergency buffer and then calculated 3 months of that total, rather than using the pre-calculated Q1 budget figure
- Failed assumption: AI derived the number instead of referencing Canonical Numbers

**3. Rollback**
"Let's discard that calculation. The correct figure is in Canonical Numbers: Total Q1 budget = £1,500. The emergency buffer is separate, not multiplied."

**4. Note**
- Failure Log entry added (Numerical error category)
- Running Document updated: "Budget figures must be taken directly from Canonical Numbers — no recalculation"

**Resume:** Continue with verified figure.

---

## When Repair Feels Slow

Repair takes time. This can feel frustrating when you want to make progress.

Remember:

- Unrepaired failures compound
- Pushing through a broken state wastes more time later
- Each repair strengthens the system
- Speed returns after stability is restored

The goal is not to avoid repair. The goal is to make repair fast and routine.

---

## Repair Is Not Blame

The repair protocol is diagnostic, not punitive.

- "Something broke" is different from "someone failed"
- The AI cannot feel blamed; the protocol protects the human from self-blame too
- Focus on the system, not the participants
- Every failure is an opportunity to improve structure

If repairs feel emotionally charged, that's a signal to slow down further, not speed up.

---

*Stop → Diagnose → Rollback → Note*

*Every repair makes the next one faster.*
