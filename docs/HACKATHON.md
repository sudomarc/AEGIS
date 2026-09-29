# ForgeHacks Operating Sheet

## Official dates

- **Start:** October 3, 2026 — 12:00 PM EST
- **Submission lock:** October 10, 2026 — 12:00 PM EST
- **Judging:** October 10–11
- **Winners:** October 12, 2026 — 3:00 PM EST

Official source:
https://forgehacks-2026.devpost.com/rules

## Eligibility and submission

Current rules say:
- Current students worldwide are eligible subject to standard exceptions.
- Teams contain 1–4 participants.
- Public code is required unless organizers require private sharing for judging.
- Open-source libraries, public datasets, and pre-trained models are permitted.
- AI coding tools are permitted.
- The project must be substantially created during the hackathon period.
- Required submission material includes the project description, selected track, 2–4 minute public demo video, GitHub repository, written technical/problem description, and evidence such as screenshots, architecture diagram, or deployment link.

## Prompt gate

The six track prompts are intentionally released at kickoff. Until the official prompt is available, AEGIS must remain prompt-agnostic.

Record the exact prompt in:
`docs/research/OFFICIAL-PROMPT.md`

Do not rely on a paraphrase when making scope decisions.

## Suggested build cadence

### Phase 0 — kickoff
Prompt capture → constraint extraction → problem selection → judge-fit check.

### Phase 1 — architecture
Thin-slice architecture → data/model contracts → test strategy.

### Phase 2 — implementation
End-to-end demo path → AI depth → integrations → evaluation.

### Phase 3 — hardening
Failure handling → security/privacy → performance → responsive/accessibility QA.

### Phase 4 — submission
README → screenshots → architecture diagram → metrics → 2–4 minute video → final verification.

## Pre-kickoff compliance

Allowed:
- governance;
- agent instructions;
- research methodology;
- generic templates;
- empty directories/placeholders;
- environment variable names.

Avoid:
- prompt-specific features;
- a finished product;
- pre-recorded final demo;
- fake evaluation results;
- claiming pre-kickoff work as hackathon-built functionality.
