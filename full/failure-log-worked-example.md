# Failure Log — Worked Example

This is a filled-in example showing how a Failure Log looks in practice, including pattern analysis. Use it as a reference when creating your own.

---

## Failure Log

| Date | Category | What happened | Why it happened | How it was fixed | What changed |
|------|----------|---------------|-----------------|------------------|--------------|
| Jan 14 | Context drift | AI drafted blog post using old brand voice — formal tone when we'd shifted to conversational | Brand voice doc wasn't in Running Document references; AI used training defaults | Re-drafted with correct voice; added brand voice doc to references | Running Document now includes brand voice link |
| Jan 16 | Numerical error | Budget calculation showed £600/month available instead of £500 | AI recalculated from conversation history instead of Canonical Numbers | Corrected figure; re-emphasized that Canonical Numbers is the only source | Added explicit instruction to Running Document: "All figures from Canonical Numbers only" |
| Jan 18 | Version confusion | Two versions of "Week 2 post" existed — AI edited the wrong one | No naming convention; files had similar names | Deleted duplicate; established naming convention | All drafts now: [Topic]_v[X]_[Date].md |
| Jan 21 | Miscommunication | Asked for "a few alternatives" — AI produced 12 options | "A few" was ambiguous | Selected 3; clarified preference for 3–5 options | Added to Rules: "When asked for alternatives, provide 3–5 unless specified otherwise" |
| Jan 23 | Tone/trust issue | AI was overly cautious after previous correction — hedging everything, asking excessive clarifying questions | Overcorrection after Jan 21 feedback | Direct conversation: acknowledged the issue, reset expectations | Added to Rules: "One clarifying question max before proceeding; ask forgiveness not permission for small judgment calls" |
| Jan 26 | Context drift | AI forgot that we'd decided to delay video content to Q2; suggested video ideas for February | Decision was made before Running Document was established; never captured | Added decision to Running Document Decisions Log | Committed to logging all significant decisions immediately |
| Jan 28 | Numerical error | AI calculated cost of 4 freelance articles as £280 instead of £300 | Used old rate (£70) instead of updated rate (£75) from Canonical Numbers | Recalculated correctly | Confirmed AI re-reads Canonical Numbers at start of each session |
| Jan 30 | Boundary violation | During content planning session, AI started offering detailed SEO technical recommendations | Scope creep; no clear boundary on what domains AI should cover | Redirected to content focus; noted that SEO is out of scope for this collaboration | Added to Rules: "Stay within content strategy; flag but don't elaborate on SEO, technical, or design issues" |
| Feb 2 | Cross-domain interference | AI applied risk-averse tone from finance project to content brainstorming | Had been working on finance earlier; context bled over | Reset context; re-read content project Running Document | Added practice: clear "context switch" statement when changing projects |

---

## Patterns Observed

**Pattern 1: Reference failures (Jan 14, Jan 16, Jan 26, Jan 28)**

Four of nine failures involved the AI not properly referencing authoritative documents — either forgetting they exist or using outdated information.

*Structural fixes applied:*
- Running Document now explicitly lists all reference documents
- Opening instruction for each session: "Read the Running Document and Canonical Numbers before responding"
- All significant decisions logged immediately to prevent orphaned context

*Status:* After fixes, reference failures dropped significantly. Last occurrence: Jan 28.

---

**Pattern 2: Ambiguous instructions (Jan 21, Jan 30)**

Two failures resulted from instructions that seemed clear to human but were interpreted differently by AI.

*Structural fixes applied:*
- Rules section now includes default interpretations for common ambiguous terms
- Scope boundaries made explicit in Rules section

*Status:* Resolved. No recurrence after rules clarified.

---

**Pattern 3: Overcorrection after feedback (Jan 23)**

AI became overly cautious after receiving correction, degrading usefulness in the opposite direction.

*Structural fix applied:*
- After corrections, explicitly affirm the working relationship
- Added rule about "ask forgiveness not permission for small judgment calls"

*Status:* Single occurrence. Watching for recurrence.

---

**Pattern 4: Context bleed between projects (Feb 2)**

Working on multiple projects in same day caused tone/approach from one to leak into another.

*Structural fix applied:*
- Clear "context switch" protocol when changing projects
- Re-read relevant Running Document before continuing

*Status:* New pattern. Fix just implemented.

---

## Summary Statistics

| Category | Count | % of Total |
|----------|-------|------------|
| Context drift | 2 | 22% |
| Numerical error | 2 | 22% |
| Version confusion | 1 | 11% |
| Boundary violation | 1 | 11% |
| Tone/trust issue | 1 | 11% |
| Miscommunication | 1 | 11% |
| Cross-domain interference | 1 | 11% |
| **Total** | **9** | **100%** |

---

*Last updated: February 2, 2025*
