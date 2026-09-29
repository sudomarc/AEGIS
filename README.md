# AEGIS

**ForgeHacks Online 2026 — AI for Real World Problems**

AEGIS is the working repository for our ForgeHacks 2026 submission.

> **Status:** PRE-HACKATHON SCAFFOLD — no prompt-specific product implementation yet.

## Competition

ForgeHacks Online 2026 runs **October 3–10, 2026**.

Official rules currently state:
- Kickoff: **October 3, 12:00 PM EST**
- Prompt reveal: at kickoff
- Submission deadline: **October 10, 12:00 PM EST**
- Judging: October 10–11
- Winners: October 12, 3:00 PM EST
- Teams: 1–4 students
- AI coding tools such as ChatGPT, Claude, and Copilot are allowed.
- Projects must be substantially created during the hackathon period.

Source: https://forgehacks-2026.devpost.com/rules

## Before kickoff

We prepare only the engineering operating system:
- agent governance;
- research and decision templates;
- project structure;
- environment configuration names;
- verification conventions;
- demo/submission checklist.

We do **not** pre-build the final solution before the prompt reveal.

## During kickoff

1. Capture the exact official track prompt.
2. Map requirements to a narrow, testable product.
3. Activate at least five independent agent roles.
4. Select the smallest credible architecture.
5. Build an end-to-end thin slice first.
6. Add AI depth and measurable evaluation.
7. Verify, review, polish, document, and record the demo.

## Repository structure

```
AGENTS.md                 # mandatory project governance
docs/
  HACKATHON.md            # event constraints and operating checklist
  DECISIONS.md            # dated technical/product decisions
  handoffs/               # compact agent-to-agent state transfers
  research/               # prompt/evidence research
src/                      # product code during the hackathon
tests/                    # verification and evaluation
```

## Source of truth

The ForgeHacks rules and prompt are the event authority. The Vibe Coding Instructions repository is the engineering-agent governance authority.

External governance:
https://github.com/sudomarc/vibe-coding-instructions
