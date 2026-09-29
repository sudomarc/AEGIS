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


## ForgeHacks Judging Rubric — AEGIS acceptance criteria

The project must be designed and verified against these five judging dimensions:

### 1. Real-World Impact & Relevance
- Clearly addresses a genuine problem.
- Has credible potential for actual use or meaningful benefit to users/communities.
- Prefer evidence, concrete users, and a believable usage scenario over broad claims.

### 2. Technical Implementation & AI Use
- AI/ML components must be technically meaningful, correct, and integrated into the product.
- Avoid a thin LLM wrapper.
- Document model choice, data flow, tools, evaluation, failure handling, and relevant limits.

### 3. Innovation & Creativity
- Show an original idea, approach, or combination of technologies.
- Novelty must serve the problem rather than exist as decoration.

### 4. Execution & Completeness
- Working end-to-end demo is mandatory.
- Prioritize a coherent, polished golden path over a large unfinished feature set.
- Verify usability, reliability, and the amount of functionality actually shipped during the hackathon.

### 5. Presentation & Communication
- 2–4 minute video must explain the problem, solution, AI/technical approach, and impact simply.
- README and written submission must tell the same story and provide enough technical evidence to reproduce or evaluate the project.

### Design rule
No feature is accepted merely because it is impressive. Each proposed feature must map to one or more rubric dimensions and have a clear verification method.
