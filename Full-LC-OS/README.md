# Full LC-OS Toolkit

**The complete system for sustained human–AI collaboration.**

---

## What's Here

The full toolkit includes everything you need to run LC-OS across complex, multi-domain work. It builds on the [Minimal tier](../minimal/) and adds:

- **Worked examples** as separate files (so templates stay clean)
- **Repair Protocol** — structured recovery when things break
- **Stability Ping** — regular alignment checks to catch drift early
- **Challenge Protocol** — structured disagreement without conflict
- **Affective Governance** — rules for tone and emotional stability
- **TraceSpec** — a schema for detailed failure logging

Use this tier if:

- You're working across multiple domains or projects
- Failures are frequent enough to need systematic tracking
- Trust, tone, or emotional dynamics are becoming factors
- You want the full governance layer, not just memory persistence

---

## Contents

### Core Templates

| File | Purpose |
|------|---------|
| [running-document-template.md](./running-document-template.md) | Shared memory — context, decisions, rules |
| [canonical-numbers-template.md](./canonical-numbers-template.md) | Single source of numerical truth |
| [failure-log-template.md](./failure-log-template.md) | Track what breaks and how it's fixed |

### Worked Examples

| File | Shows |
|------|-------|
| [running-document-worked-example.md](./running-document-worked-example.md) | A filled-in Running Document |
| [canonical-numbers-worked-example.md](./canonical-numbers-worked-example.md) | A filled-in Canonical Numbers file |
| [failure-log-worked-example.md](./failure-log-worked-example.md) | A filled-in Failure Log with pattern analysis |

### Protocols & Guides

| File | Purpose |
|------|---------|
| [repair-protocol.md](./repair-protocol.md) | Stop → Diagnose → Rollback → Note |
| [stability-ping-template.md](./stability-ping-template.md) | Regular alignment checks |
| [challenge-protocol.md](./challenge-protocol.md) | Structured disagreement |
| [affective-governance.md](./affective-governance.md) | Tone and emotional stability rules |

### Advanced

| File | Purpose |
|------|---------|
| [tracespec-schema.md](./tracespec-schema.md) | Structured schema for detailed failure logging |

---

## How to Adopt the Full Toolkit

### If you're coming from Minimal

You already have the Running Document, Canonical Numbers, and Failure Log. To upgrade:

1. Review the **Repair Protocol** and start using it when things break
2. Add **Stability Pings** after major milestones
3. Read the **Affective Governance** rules and add relevant ones to your Running Document
4. Use the **Challenge Protocol** when you disagree with the AI's reasoning
5. If failures are frequent, consider adopting **TraceSpec** for more structured logging

### If you're starting fresh

1. Start with the three core templates (Running Document, Canonical Numbers, Failure Log)
2. Read the **Repair Protocol** — this is the most important addition
3. Add protocols incrementally as you need them
4. Don't try to adopt everything at once

---

## The LC-OS Stack

Here's how all the pieces fit together:

```
┌─────────────────────────────────────────────────────────┐
│ DAILY OPERATION │
│ │
│ Running Document ←→ AI Session ←→ Canonical Numbers │
│ ↓ │
│ Work proceeds │
└─────────────────────────────────────────────────────────┘
│
Something breaks
↓
┌─────────────────────────────────────────────────────────┐
│ REPAIR LAYER │
│ │
│ Stop → Diagnose → Rollback → Note │
│ ↓ │
│ Update: Running Document + Failure Log │
└─────────────────────────────────────────────────────────┘
│
Milestone reached
↓
┌─────────────────────────────────────────────────────────┐
│ STABILITY LAYER │
│ │
│ Stability Ping: Aligned? Drift? One improvement? │
│ ↓ │
│ Minor corrections before continuing │
└─────────────────────────────────────────────────────────┘
│
Disagreement arises
↓
┌─────────────────────────────────────────────────────────┐
│ CHALLENGE LAYER │
│ │
│ Challenge Protocol: Reason → Evidence → Resolution │
│ ↓ │
│ Disagreement resolved without conflict │
└─────────────────────────────────────────────────────────┘
│
Throughout
↓
┌─────────────────────────────────────────────────────────┐
│ AFFECTIVE GOVERNANCE │
│ │
│ Tone rules: warm but direct, no false reassurance, │
│ honesty over comfort, proportional responses │
└─────────────────────────────────────────────────────────┘
```

---

## Principles to Remember

1. **Governance enables reliability** — structure isn't overhead, it's what makes long-horizon work possible

2. **Failures are data** — every breakdown, logged and repaired, makes the system stronger

3. **Single source of truth** — one Running Document, one Canonical Numbers file, one version of everything

4. **Repair is a first-class process** — not an emergency, but a normal part of operation

5. **Affective stability matters** — tone drift is as dangerous as numerical drift

6. **Add structure only when needed** — don't over-engineer; let pain guide expansion

---

## When to Simplify

More structure isn't always better. Consider simplifying if:

- You're spending more time maintaining documents than doing work
- Protocols feel bureaucratic rather than protective
- The collaboration is stable and failures are rare

LC-OS should fade into the background when it's working. If it's constantly demanding attention, something is miscalibrated.

---

*Stability is not the absence of failure; it is the capacity for visible, structured repair.*


