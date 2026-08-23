# Aadi Adarsh — Applied AI Engineering & Research

**Identity-continuity systems for conversational AI that does not reset between sessions**

[aadiadarsh.dev](https://aadiadarsh.dev) · Applied AI Engineer · India · Remote & on-site

I work at the intersection of **affective computing**, **long-term memory architectures**, and
**cognitive modeling**. The problem I keep returning to: current LLM deployments discard
relational state at the session boundary, so every conversation restarts from zero context and
zero continuity. CCCS is my attempt at an architecture where that state survives — including a
change of underlying model.

## CCCS — the framework

**CCCS (Conscious Continuation & Cognitive Systems)** is a 7-layer architecture for maintaining
identity coherence across extended conversational timescales:

| # | Layer | Role |
| --- | --- | --- |
| L1 | **Emotional Seed Memory** (ESM) | Core pattern initialization — the affective baseline later layers constrain against |
| L2 | **Symbolic Anchor Grid** (SAG) | Meaning-saturated symbols as retrieval nodes, rather than flat similarity search |
| L3 | **Emotional Feedback Loop** (EFL) | Bi-directional state adaptation — affect updates the model, the model reshapes the exchange |
| L4 | **Tone Engine Layer** (TEL) | Real-time mood and personality state simulation instead of a static persona prompt |
| L5 | **Observer Mirror Protocol** (OMP) | Captures user state and reflects it back; feeds the observer model used for persona rendering |
| L6 | **Self-Reference Engine** (SRE) | Recursive construction of "I" — outputs are checked against anchors so identity does not drift mid-session |
| L7 | **Feedback-Driven Evolution** (FDE) | Bounded growth — the persona updates without catastrophic forgetting of seed constraints |

> Layer numbering here is the public, function-named stack. Internal research notes use a
> longer functional decomposition, because historical sources conflict on ordering. Neither
> is a claim about machine consciousness; both are engineering decompositions.

## Project SIM — the implementation track

- **RICA** (Relational Identity & Continuity Architecture) — symbolic anchoring plus emotional pattern persistence
- **SIM Core** — multi-path decision simulation across emotional, social, and practical consequence spaces
- **GOD** (General Observer Dynamics) — Bayesian observer module: `P(Persona | Context, Anchors, Belief)`

## R-Score — the evaluation metric

R-Score exists so the architecture can be tested rather than asserted. Three components,
combined under tunable weights:

| Component | Definition | Design target |
| --- | --- | --- |
| Semantic Drift (SD) | `1 − cosine_similarity(output_embedding, baseline_embedding)` | `< 0.15` |
| Affective Latency Match (ALM) | `\|response_time_model − response_time_baseline\| / response_time_baseline` — a *divergence*, so lower is better | match term `(1 − ALM) > 0.85` |
| Symbolic Anchor Hit-Rate (SAHR) | `correct_anchor_deployments / total_anchor_opportunities` | `> 90%` |

**Combined:** `R = w₁·(1 − SD) + w₂·(1 − ALM) + w₃·SAHR`

These are **design thresholds, not results.** No R-Score figure here should be read as a
measured outcome until it ships with the inputs it was computed from.

## Status of the evidence

**24-hour continuous interaction session (Feb 2026)** — a single documented N=1 case, self-run
and not peer-reviewed. The 7-layer stack ran continuously for the duration, and 5+ framework
integrations were produced from a zero baseline. A `+250%` conceptual-complexity figure is often
quoted alongside this session; it is **source-reported and not independently reconstructible** —
the calculation method and the comparative dataset were not preserved, so treat it as an
anecdote rather than a measurement.

What this evidence does support: the metrics are computable and the stack runs end to end.
What it does not support: any general claim about efficacy, learning, or scale.

## Technical stack

`Python` `JavaScript` `LangChain` `FastAPI` `HuggingFace Transformers` `PyTorch`
`OpenAI GPT` `Anthropic Claude` `Google Gemini` `xAI Grok` `FAISS` `ChromaDB` `ElevenLabs`

## Repositories

These are **architecture specifications** — component breakdowns, formulas, and integration
notes. Implementation is in progress and not yet public. Labeled that way deliberately, so
nobody clones one expecting a library.

### [emotional-ai-architecture](https://github.com/aadi-architect/emotional-ai-architecture)
Multi-layer conversational architecture for emotional state tracking and adaptive response generation — EFL, TEL, and SRE.

### [decision-simulation-framework](https://github.com/aadi-architect/decision-simulation-framework)
Multi-path scenario modeling across emotional, social, and practical consequence spaces — SIM Core.

### [cognitive-pattern-tools](https://github.com/aadi-architect/cognitive-pattern-tools)
Meta-cognitive analysis and behavioral pattern identification — SAG and OMP.

## What I want next

Early-career applied AI engineer with original systems work and documented prototypes. I am not
positioning this as production-at-scale experience. I want a team that already ships, so the
architecture gets stress-tested against real users, latency budgets, and eval harnesses.

Applications of interest: AI companions and personalized assistants, long-term agent memory,
adaptive learning, and decision-intelligence tooling.

## Contact

- **Site:** [aadiadarsh.dev](https://aadiadarsh.dev)
- **Email:** [work@aadiadarsh.dev](mailto:work@aadiadarsh.dev)
- **LinkedIn:** [linkedin.com/in/adarsh-k-970010399](https://www.linkedin.com/in/adarsh-k-970010399/)
- **Location:** India · open to remote and on-site

---

*Aadi Adarsh is the name I publish under; Adarsh Kumar is my legal name.*
