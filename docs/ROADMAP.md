# AEGIS Hackathon Roadmap

## North star

Deliver one narrow, polished, evidence-backed AI product that directly satisfies the official ForgeHacks prompt and demonstrates a credible real-world use case.

**Optimization order:**

Real problem → Working MVP → Meaningful AI → Differentiation → Polish → Evidence → Presentation

Do not optimize for feature count.

## Phase 0 — Pre-hackathon (Sep 29 → Oct 2)

**Goal:** prepare the engineering operating system without building the final product.

### Prepare
- repository governance;
- external Vibe Coding Instructions workflow;
- agent role contracts and handoffs;
- candidate stack;
- generic UI/app scaffolding only if it is demonstrably prompt-agnostic;
- test/evaluation harness templates;
- README/submission templates;
- research source map;
- environment variable names;
- deployment pathway.

### Do not build
- final prompt-specific features;
- final product workflow;
- prompt-specific datasets or model tuning;
- final demo;
- fake metrics or benchmark claims.

## Phase 1 — Kickoff and prompt lock (Oct 3)

**T+0: Prompt release**

1. Capture the exact official prompt in `docs/research/OFFICIAL-PROMPT.md`.
2. Extract explicit requirements, constraints, users, outputs, and judging implications.
3. Run the Challenge Researcher.
4. Independently review problem, novelty, technical feasibility, and implementation risk.
5. Decide the smallest credible product.
6. Record the decision in `docs/DECISIONS.md`.

**Gate:** no implementation until the team has a written problem statement, target user, golden path, success criteria, and architecture decision.

## Phase 2 — Thin slice

**Target:** end-to-end demo path as early as possible.

Build:

`input → core AI/system behavior → useful result → user action`

Verify the golden path before adding secondary features.

## Phase 3 — AI depth

Add only AI/ML capabilities that are necessary for the prompt, such as:
- classification;
- extraction;
- structured generation;
- retrieval;
- multimodal reasoning;
- tool calling;
- recommendation;
- workflow automation;
- model evaluation.

Document why AI is necessary and how it is evaluated.

## Phase 4 — Real-world proof

Collect:
- target-user evidence;
- realistic synthetic fixtures where sensitive real data would be inappropriate;
- baseline/comparison where meaningful;
- measured precision/recall/F1/latency/etc. only when actually tested;
- known failure cases;
- safety/privacy constraints.

## Phase 5 — Product hardening

Run:
- functional tests;
- adversarial/security review;
- API and rate-limit review;
- error/fallback testing;
- responsive/browser verification;
- accessibility review;
- performance review.

## Phase 6 — Demo and submission

Freeze the story around one compelling scenario.

### Demo sequence
1. Problem
2. User
3. Input
4. AI/system behavior
5. Result
6. Action/impact
7. Technical proof
8. What was built during ForgeHacks

### Submission package
- project title;
- track;
- problem/target users;
- solution;
- technical approach;
- AI/ML explanation;
- real-world impact;
- GitHub;
- 2–4 minute public demo;
- screenshots;
- architecture diagram;
- deployment/testing link where available.

## Phase 7 — Final freeze

Before the deadline:
- verify submission completeness;
- verify all team members are listed;
- verify repository access;
- verify secrets are absent;
- verify licenses;
- verify the final build;
- inspect final diff/status;
- submit once.

## Internal deadline

Treat the published submission lock as the absolute technical deadline, but aim to have the product and recording ready before that point so the final period is for verification and submission recovery, not feature development.
