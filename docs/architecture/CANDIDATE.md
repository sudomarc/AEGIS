# Candidate Architecture — Prompt-Gated

## Candidate concept

**AEGIS:** a multimodal AI-assisted cyber-risk analyzer for real-world users.

Potential flow:

`Message / URL / screenshot / QR`
→ `pre-processing`
→ `deterministic signals / extraction`
→ `ML or classification`
→ `LLM reasoning`
→ `risk + explanation`
→ `recommended action`
→ `evidence/report`

## Why this is only a candidate

ForgeHacks publishes the track prompt at kickoff. No prompt-specific implementation is permitted before the event.

Therefore this document is a hypothesis used to think about architecture trade-offs only.

## Differentiation hypotheses

Potential differentiators, subject to prompt fit:
- multimodal input;
- evidence-backed explanation;
- action-oriented response rather than classification only;
- measurable evaluation;
- localized/context-aware threat patterns.

## Architecture guardrails

- keep provider access behind a server-side boundary;
- validate model output;
- separate deterministic checks from generative reasoning;
- avoid unsafe autonomous actions;
- make high-impact actions explicit/user-confirmed;
- implement timeouts, rate limits, tool-call limits, and output caps;
- log only non-sensitive diagnostic metadata.
