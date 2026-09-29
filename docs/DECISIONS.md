# AEGIS Decisions

Use dated entries. Separate FACT, OBSERVED, VERIFIED, INFERENCE, ASSUMPTION, UNKNOWN, CONFLICT, and UNVERIFIED when they matter.

## 2026-09-29 — Pre-hackathon scope

**Decision:** Keep the repository prompt-agnostic until the official ForgeHacks prompt is revealed.

**Reason:** The official rules state that projects must be substantially created during the hackathon, and the track prompts are released at kickoff.

**Status:** VERIFIED from official Devpost rules.

**Next trigger:** October 3, 2026 kickoff and prompt reveal.



## 2026-09-29 — Candidate product direction

**Decision:** Keep the current AEGIS concept as a prompt-gated hypothesis, not a committed product.

**Candidate:** multimodal AI-assisted cyber-risk analysis (message/URL/screenshot/QR → extraction/signals → AI analysis → explanation/action/evidence).

**Reason:** It maps naturally to the Cybersecurity track and can demonstrate meaningful AI, real-world value, measurable evaluation, and a strong demo. The official prompt may invalidate or reshape it.

**Status:** INFERENCE / UNVERIFIED for ForgeHacks prompt fit until Oct 3.

## 2026-09-29 — Candidate technical stack

**Decision:** Default to Next.js App Router + TypeScript + Tailwind/shadcn + Zod + Vercel AI SDK + Featherless, with Vercel deployment and Vitest/Playwright verification. Database and n8n remain optional.

**Reason:** Full-stack simplicity, fast iteration, provider abstraction, AI integration, and a low-ops deployment path fit a seven-day hackathon.

**Status:** Architecture candidate; prompt-gated.
