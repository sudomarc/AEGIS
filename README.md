# AEGIS

**ForgeHacks Online 2026 — AI for Real World Problems**

AEGIS is the working repository for our ForgeHacks 2026 submission.

> **Status:** PRE-HACKATHON / PROMPT-GATED. The repository contains governance and planning only; the final product is not built yet.

## Competition window

- **Kickoff / prompt reveal:** October 3, 2026 — 12:00 PM EST
- **Hacking ends / submissions lock:** October 10, 2026 — 12:00 PM EST
- **Judging:** October 10–11
- **Winners:** October 12, 2026 — 3:00 PM EST
- **Team size:** 1–4 students
- **Format:** Fully online, worldwide subject to the published eligibility exceptions

Official rules: https://forgehacks-2026.devpost.com/rules
Official site: https://www.forgehacks.dev/

## Design target

AEGIS is optimized against the official judging rubric:

1. **Real-World Impact & Relevance** — genuine problem, specific users, credible benefit.
2. **Technical Implementation & AI Use** — meaningful AI/ML integration, technical depth, correctness; not a thin wrapper.
3. **Innovation & Creativity** — useful originality or novel combination of technologies.
4. **Execution & Completeness** — working demo, polish, usability, and substantial hackathon-shipped functionality.
5. **Presentation & Communication** — clear 2–4 minute video, README, written explanation, and technical evidence.

See docs/SCORECARD.md for acceptance gates.

## Candidate product

A prior brainstorm produced a **candidate**, not a commitment: a multimodal AI-assisted cyber-risk analyzer that could analyze a message, URL, screenshot, or QR code, combine deterministic signals with ML/LLM reasoning, explain the evidence, and recommend safe action.

This concept is intentionally **prompt-gated** and must be adapted or discarded after the official track prompt is revealed.

## Candidate stack

**Next.js App Router + TypeScript + Tailwind/shadcn + Zod + Vercel AI SDK + Featherless**, deployed on Vercel, with **Vitest/Playwright** verification. Postgres/Supabase and n8n are optional additions only when justified by the final prompt.

See docs/STACK.md.

## Operating model

### Pre-hackathon
Prepare the engineering operating system only:
- repository governance;
- external Vibe Coding Instructions;
- multi-agent role contracts and handoffs;
- research methodology;
- candidate architecture/stack;
- evaluation and submission templates;
- deployment pathway;
- environment variable names.

Do **not** implement final prompt-specific product functionality before kickoff.

### During hackathon
1. Capture the exact prompt.
2. Validate the problem and target user.
3. Run at least five independent agent roles.
4. Choose a narrow golden path.
5. Build the thin slice end-to-end.
6. Add meaningful AI depth and evaluation.
7. Harden security/reliability/UX.
8. Prepare the 2–4 minute demo and submission.
9. Verify the final repository and submit once.

## Repository map

- AGENTS.md — mandatory governance and external Vibe Coding Instructions policy.
- docs/HACKATHON.md — official dates, eligibility, rules, judging rubric, compliance gates, participant tooling.
- docs/ROADMAP.md — day-by-day build strategy.
- docs/STACK.md — candidate technical stack and API guardrails.
- docs/SCORECARD.md — product acceptance gates mapped to judging criteria.
- docs/AGENT-PLAYBOOK.md — seven-role orchestration model and handoff contract.
- docs/SUBMISSION.md — final Devpost/GitHub/demo checklist.
- docs/PARTICIPANT-PERKS.md — verified build-time sponsor benefits and activation guidance.
- docs/research/RESEARCH-PLAN.md — prompt/problem/competitive/technical research process.
- docs/research/OFFICIAL-PROMPT.md — exact prompt capture location for kickoff.
- docs/architecture/CANDIDATE.md — prompt-gated architecture hypothesis.
- docs/DECISIONS.md — dated decisions and uncertainty.
- docs/handoffs/ — compact cross-agent state snapshots.
- src/ — product implementation during the hackathon.
- tests/ — verification/evaluation during the hackathon.

## Governance source of truth

The external engineering-agent governance source is:
https://github.com/sudomarc/vibe-coding-instructions

Do not replace it with locally invented agent/skill instructions.
