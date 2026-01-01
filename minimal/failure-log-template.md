# Failure Log

**What this is:** A record of what went wrong, why, and how it was fixed. Not for blame — for learning.

**How to use it:** When something breaks in your collaboration, add an entry. Be specific. Over time, this becomes a map of your system's weak points and how you've addressed them.

**Why this matters:** Failures that aren't logged repeat. Failures that are logged become structural improvements. The goal isn't to avoid all failure — it's to make failure *visible* and *repairable*.

---

## When to Log

Log a failure when:

- The AI produced something wrong that required correction
- A misunderstanding caused wasted work
- Context was lost and had to be re-established
- Numbers drifted or were inconsistent
- Trust or tone broke down
- You had to say "that's not what I meant" more than once

Don't log:

- Minor clarifications that didn't disrupt flow
- Normal iteration and refinement
- Things that felt annoying but didn't actually cause problems

---

## Entry Structure

Each entry should capture:

1. **Date** — when it happened
2. **Category** — what type of failure (see categories below)
3. **What happened** — brief factual description
4. **Why it happened** — root cause, not surface symptom
5. **How it was fixed** — what repair action was taken
6. **What changed** — what's different now to prevent recurrence

---

## Failure Categories

Use these to classify entries (or create your own):

| Category | Description |
|----------|-------------|
| **Context drift** | AI lost or misremembered prior context |
| **Numerical error** | Wrong calculations, mixed units, invented numbers |
| **Version confusion** | Working from outdated or wrong version of a document |
| **Boundary violation** | AI stepped outside its designated role or scope |
| **Tone/trust issue** | Emotional misalignment, defensiveness, false reassurance |
| **Miscommunication** | Instructions were unclear or misinterpreted |
| **Other** | Doesn't fit above categories |

---

## Failure Log Template

| Date | Category | What happened | Why it happened | How it was fixed | What changed |
|------|----------|---------------|-----------------|------------------|--------------|
| | | | | | |

---

## Patterns to Watch

After you have 5–10 entries, look for patterns:

- Are certain categories appearing repeatedly?
- Are failures clustering around specific tasks or contexts?
- Are the same root causes recurring despite fixes?

Patterns indicate structural weaknesses. Address the pattern, not just individual incidents.

---

---

# Worked Example

Below is a filled-in example showing how this template looks in practice. Delete this section when you create your own.

---

## Failure Log

| Date | Category | What happened | Why it happened | How it was fixed | What changed |
|------|----------|---------------|-----------------|------------------|--------------|
| Jan 14 | Context drift | AI drafted blog post using old brand voice — formal tone when we'd shifted to conversational | Brand voice doc wasn't in Running Document references; AI used training defaults | Re-drafted with correct voice; added brand voice doc to references | Running Document now includes brand voice link |
| Jan 16 | Numerical error | Budget calculation showed £600/month available instead of £500 | AI recalculated from conversation history instead of Canonical Numbers | Corrected figure; re-emphasized that Canonical Numbers is the only source | Added explicit instruction to Running Document: "All figures from Canonical Numbers only" |
| Jan 18 | Version confusion | Two versions of "Week 2 post" existed — AI edited the wrong one | No naming convention; files had similar names | Deleted duplicate; established naming convention | All drafts now: [Topic]_v[X]_[Date].md |
| Jan 21 | Miscommunication | Asked for "a few alternatives" — AI produced 12 options | "A few" was ambiguous | Selected 3; clarified preference for 3–5 options | Added to Rules: "When asked for alternatives, provide 3–5 unless specified otherwise" |
| Jan 23 | Tone/trust issue | AI was overly cautious after previous correction — hedging everything, asking excessive clarifying questions | Overcorrection after Jan 21 feedback | Direct conversation: acknowledged the issue, reset expectations | Added to Rules: "One clarifying question max before proceeding; ask forgiveness not permission for small judgment calls" |

---

## Patterns Observed

**After 5 entries:**

1. **Context drift** and **numerical error** both stemmed from the same root: AI not consistently referencing the canonical documents. 
   - *Structural fix:* Opening prompt for each session now explicitly states: "Read the Running Document and Canonical Numbers before responding."

2. **Miscommunication** appeared when instructions used vague quantifiers ("a few," "some," "briefly").
   - *Structural fix:* Rules section now includes default interpretations: "a few = 3–5," "briefly = 2–3 sentences."

3. **Tone/trust issue** emerged as a reaction to correction, not as a primary failure.
   - *Structural fix:* After corrections, explicitly affirm the working relationship: "That fix was right; we're aligned; proceed normally."

---

*This Failure Log was last updated: January 23, 2025*
