# Prompt Library

> A prompt tells the AI what to say. A prompt system tells it **how to think**.
>
> Works with Claude, GPT, Gemini, or any capable LLM.
>
> by **Logue** · [@AlexZio00](https://x.com/AlexZio00)

---

## What this is

Most prompts are instructions: *"Summarize this. Write me that. Act like X."*

These are systems. Each one has internal phase logic, decision routing, and epistemic rules that hold regardless of what you feed in. The AI doesn't decide how to analyze — the system routes it.

Three types in this library:

**Modular frameworks** — pick the layers you need, combine them.  
[Document Deconstructor](prompts/document-deconstructor.md) has 15 modules designed as Lego blocks — run a single phase or all five, in any order. [Sovereign Lens](prompts/sovereign-lens.md) builds image generation prompts as a stack: Base × Camera × Subject × Scene × Fine-tuning. You select one option per layer; the combination defines the output.

**Structured intelligence engines** — collect and analyze information through a fixed output schema, not freeform prose.  
[News Briefing Engine](prompts/news-briefing-engine.md) runs PEST analysis, produces a structured macro read with an explicit action stance, and forces falsification conditions for every conclusion. [Power Structure Debugger](prompts/power-structure-debugger.md) runs Symbol → Narrative → Synthesis — each phase feeding the next — and resolves to a single Cui Bono verdict.

**Adversarial templates** — built to challenge your thinking, not confirm it.  
[Philosopher Sparring Engine](prompts/philosopher-sparring-engine.md) loads a philosopher's actual intellectual weapons and applies them to your claim. Agreement is structurally forbidden until deconstruction passes. [Dilemma Destroyer](prompts/dilemma-destroyer.md) works 5 ordered stages — surfaces the hidden assumption, destroys compromise, builds a third axis, then *attacks its own solution* before proposing anything.

What all six share: no conclusion without a kill condition, no claim without a tag, no output that varies by the AI's mood.

---

## Prompts

| # | Name | Type | What it does |
|---|------|------|-------------|
| 1 | [Document Deconstructor](prompts/document-deconstructor.md) | Modular — 15 modules, 5 phases | Reading engine: surface comprehension → deep inference → critical bias and logic audit |
| 2 | [News Briefing Engine v2.0](prompts/news-briefing-engine.md) | Structured intelligence engine | Daily macro briefing: PEST analysis, explicit action stance, and falsification conditions per conclusion |
| 3 | [Dilemma Destroyer v5.0](prompts/dilemma-destroyer.md) | 5-stage adversarial chain | Breaks false A-vs-B dilemmas — surfaces the hidden assumption, constructs axis C, then attacks it |
| 4 | [Sovereign Lens](prompts/sovereign-lens.md) | Modular — 5 layers, 12 scene presets | AI image generation: combine Base × Camera × Subject × Scene × Fine-tuning to build any shot |
| 5 | [Philosopher Sparring Engine](prompts/philosopher-sparring-engine.md) | Adversarial template × 3 modes | Summon any philosopher to deconstruct your thinking — agreement not permitted until deconstruction passes |
| 6 | [Power Structure Debugger](prompts/power-structure-debugger.md) | Structured intelligence engine — 3 phases | Symbol lineage → narrative verification → Cui Bono synthesis |

---

## How to use

1. Open any prompt file
2. Copy the prompt block
3. Paste into your LLM of choice
4. Fill in the `[INPUT]` section

Each prompt is self-contained. No setup, no API, no account required.

**For modular prompts** (Document Deconstructor, Sovereign Lens): you don't have to run the full system. Pick any individual module or layer that fits your question.

**For multi-phase prompts** (Power Structure Debugger, Dilemma Destroyer, News Briefing Engine): follow the stage order. The later stages assume earlier stages ran — skipping ahead loses the epistemic chain.

Each prompt file includes a worked example so you can see exactly what the output looks like before running it.

---

## Design principles

Every prompt in this library is built around the same four constraints:

- **Zero-base** — strip prior context before analysis. The AI starts from the source, not its priors.
- **Default: No Action** — the base recommendation is always to do nothing until conditions are met. No false urgency.
- **Falsification required** — every conclusion must state what would make it wrong. No kill condition = no claim.
- **Cui Bono** — follow the incentives, not the narrative. Surface beneficiary ≠ actual beneficiary.

---

## License

[CC BY 4.0](LICENSE) — Free to use and adapt. Attribution required: **Logue @AlexZio00**
