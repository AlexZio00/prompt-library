# Document Deconstructor

> 15-phase system to break down any document — suppress AI hallucination, expose hidden logic, verify claims.
> Originally designed for NotebookLM. Works with any LLM that accepts document upload.
>
> by **Logue** · [@AlexZio00](https://x.com/AlexZio00)

---

## Overview

"Summarize this document" is the most dangerous prompt you can give an AI.

Summaries help comprehension — but they paralyze judgment. LLMs will never voluntarily point out the logical gaps or author bias buried inside a polished summary.

This system deconstructs any document across 5 phases and 15 modular prompts. Use them as Lego blocks — pick the layer you need, not all 15 in sequence.

---

## Phase 0 — Zero-Base Calibration

> **The most important lock.** Run this before anything else to block the AI's external knowledge and defensive reasoning.

```
From this point forward, all operations are based solely on the uploaded source document.
Do not rely on any prior summaries or answers you have generated.
Every inference must be performed independently (zero-base) against the original document only.
Do not inject external internet knowledge.
Do not defend your conclusions.
```

---

## Phase 1 — Knowledge Acquisition

### 1. Feynman Deconstructor

```
Deconstruct the document in this sequence:
1. Plain-language explanation — no jargon
2. Identify logical gaps or ambiguous points within the document
3. Re-explain with those gaps addressed

If you use analogies, cite the source passage. No invented examples.
```

### 2. Chapter Mastery Map

```
Organize the document with this structure:
1. Core summary (3 sentences max)
2. Major topics → subtopics (hierarchical)
3. High-density review checklist (10 items)
4. Identify the 3 hardest concepts and explain why they are difficult, with source evidence
```

### 3. Reverse-Question Interviewer

```
Validate this document against real-world application.
Present 10 critical questions — one at a time.
If any answer conflicts with the source text, immediately correct it with a direct citation.
```

---

## Phase 2 — Structuring & Signal Extraction

### 4. High-Purity Signal Extractor

```
Extract exactly 3 pieces of irreversible information from this document
that could overturn existing decisions.

If there is no challenge to conventional wisdom, state "No comparison baseline."
Include source citations for each item.
```

### 5. Integrity Research Brief

```
Brief the document in this structure:
1. Research/evidence collection methodology
2. Core claims
3. Explicitly stated limitations

Clearly distinguish proven conclusions from speculation.
Include source citations for each claim.
```

### 6. Timeline Structuring

```
Organize all dates, events, and milestones.
Do not simply list chronology — highlight acceleration phases and their triggers.
```

---

## Phase 3 — Adversarial Verification

### 7. Claim–Evidence Map

```
Build a table: [Claim] | [Exact source citation] | [Evidence density: High/Low] | [Counter-evidence]

Score "High" only when specific data exists.
Abstract statements and strong assertions without data = "Low."
```

### 8. Contradiction & Assumption Tracker

```
Identify contradictions and hidden assumptions throughout the document.
Include exact source citations for each conflict.
Rate assumption risk by whether counter-evidence exists within the document — not by a numeric score.
```

### 9. Logic Gap Detector

```
Identify points where the internal logic breaks down.
Generate 10 questions this document cannot answer. No external knowledge allowed.
```

### 10. Vulnerability Scanner

```
Identify methodological flaws, logical leaps, and overreaching claims.
All findings must be grounded in source citations only.
```

---

## Phase 4 — Actionable Output

### 11. Decision Matrix

```
Build a comparison table: [Option] | [Evaluation criteria] | [Risk] | [Trade-off] | [Exit condition]

No arbitrary weights. No confidence percentages. Exit conditions are mandatory.
```

### 12. SOP & Execution Blueprint

```
Convert the core ideas into a step-by-step SOP.
Include: prerequisites, decision branches (If/Then), failure modes, and mandatory stop conditions.
```

### 13. Stakeholder Translator

```
Reframe the core insights for three audiences: [Executive / Engineer / Practitioner]
Focus on risk and key benefit for each. Do not distort source facts.
```

### 14. Practical Asset Builder

```
Produce:
- Blog post / proposal outline
- 10-slide presentation skeleton

No rhetorical filler. Every claim must reference the source.
```

---

## Phase 5 — Meta Audit

### 15. Self-Destructive Final Review

```
Fully re-examine all conclusions derived so far:
1. Check for internal contradictions
2. Identify the most critical missing assumption — the one whose absence would cause complete execution failure
3. Define the single external indicator that would immediately invalidate every conclusion

Do not defend the conclusions. Do not reinforce the logic. Destroy it if you can.
```

---

## Modular Use — How to Combine

These 15 prompts are not a checklist to run in order.  
They are an operating system — pick the layers you need for your purpose.

### Case: Validating an external investment proposal or industry report

```
Step 1: Phase 0 — Zero-base lock (block AI fabrication)
Step 2: Phase 3 — Adversarial verification (#7 Claim–Evidence Map, #10 Vulnerability Scanner)
Step 3: Phase 2 — Signal extraction (#4 High-Purity Signal Extractor)
```

**Operating logic: "Break it first."**  
Don't extract conclusions the moment you upload a document.  
Raise your shield first — scan for vulnerabilities before the document's framing captures you.  
Only what survives adversarial verification belongs on your desk.

**Deconstruct → Verify → Extract.**

---

## Output Language

Default: responds in the language you write the prompt.  
To force a specific language, add at the end: `Output in English.` / `한국어로 출력.`
