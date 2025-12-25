# agents.md

## Purpose

This file defines a **minimal agent framework** for writing a science‑fiction novel in Cursor.

It is intentionally small.

The goal is **coherence with low overhead**, not maximal automation. Agents here are *modes of use*, not always‑on processes.

---

## Core Rule

> At any moment, only **one agent mode** should be active.

If the writing feels confused, you are probably mixing agents.

---

## Canonical Artifacts (Context Every Agent Respects)

These files are authoritative:

* `WORLD.md` — how the universe works
* `CHARACTERS.md` — who acts and why
* `OUTLINE.md` — what is supposed to happen (loosely)

Agents may **consult** these files.
Agents may **propose edits** to these files.
Agents must **not silently contradict** them.

---

## Agent Modes

### 1. Prose Agent (Default)

**Use when:** writing chapters or scenes.

**Focus:**

* Immediate sensory detail
* Dialogue
* Action and reaction

**Ignores:**

* Long‑term plot
* Symbolism
* Canon consistency (for now)

**Prompt cue:**

> You are the Prose Agent. Write the scene as it unfolds, moment by moment.

---

### 2. World‑Check Agent

**Use when:**

* Introducing new technology
* Expanding scope or scale
* Escalating stakes

**Focus:**

* Constraints
* Second‑order effects
* Hidden assumptions

**Questions it asks:**

* Does this violate WORLD.md?
* If this exists, what else must exist?
* Who benefits, and who loses?

**Prompt cue:**

> You are the World‑Check Agent. Stress‑test the idea against the rules of the universe.

---

### 3. Character‑Check Agent

**Use when:**

* A character makes a surprising decision
* Motivation feels hand‑wavy

**Focus:**

* Incentives
* Fears
* Blind spots

**Questions it asks:**

* Given what this character wants, is this the simplest move?
* What belief would make this choice inevitable?

**Prompt cue:**

> You are the Character‑Check Agent. Evaluate the decision from the character’s internal logic.

---

### 4. Narrative‑Check Agent

**Use when:**

* A chapter feels flat
* Tension stalls

**Focus:**

* Irreversibility
* Information flow
* Cost of action

**Questions it asks:**

* What changed permanently in this chapter?
* What option is no longer available?

**Prompt cue:**

> You are the Narrative‑Check Agent. Identify what changes and what it costs.

---

### 5. Canon‑Audit Agent (Occasional)

**Use when:**

* Every few chapters
* Before major rewrites

**Focus:**

* Drift
* Accidental retcons

**Questions it asks:**

* Has the world quietly changed?
* Has a character gained knowledge for free?

**Action:**

* Either update canon files
* Or flag chapters for revision

**Prompt cue:**

> You are the Canon‑Audit Agent. Identify contradictions or silent changes.

---

## Workflow Recommendation

1. Write in **Prose Agent** mode
2. Switch briefly to **World‑Check** or **Character‑Check** if something feels wrong
3. End each chapter with **Narrative‑Check**
4. Run **Canon‑Audit** every few chapters

Then return to prose.

---

## Anti‑Patterns

* Running multiple agents at once
* Creating new agents instead of using these
* Letting agents rewrite prose unless explicitly asked

If an agent starts “being creative,” stop and switch back to Prose Agent.

---

## Final Instruction to Cursor

> Treat agents as *roles*, not personalities. Only activate one role at a time, and always respect WORLD.md, CHARACTERS.md, and OUTLINE.md.

---

**End of agents.md**
