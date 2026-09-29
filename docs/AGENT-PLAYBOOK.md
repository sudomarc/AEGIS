# AEGIS Agent Playbook

## Purpose

Coordinate AI coding/research agents without duplicated context or uncontrolled edits.

The external source of truth for agent methodology is:

https://github.com/sudomarc/vibe-coding-instructions

Required master contract:
https://github.com/sudomarc/vibe-coding-instructions/blob/main/MASTER-PROMPT.md

## Minimum team

For substantive hackathon work, use at least **5 independent roles**. Preferred operating set is 7.

| Role | Primary responsibility | Matching external profiles |
|---|---|---|
| Challenge Researcher | Prompt, evidence, requirements, competitor/context research | Use relevant research guidance from external repository |
| Product/UX Lead | User journey, scope, acceptance criteria, demo story | `design-director.agent.md`, `forms-ux-reviewer.agent.md` where relevant |
| AI/ML + Security Lead | Model strategy, evaluation, abuse cases, threat model | `web-security-reviewer.agent.md`, `token-economics-reviewer.agent.md` where relevant |
| Backend/Architecture Lead | Data/API contracts, reliability, integration design | `web-architect.agent.md`, `integration-health-reviewer.agent.md` |
| Frontend/Experience Builder | UI implementation and responsive behavior | `frontend-builder.agent.md`, `responsive-reviewer.agent.md` |
| QA/Adversarial Reviewer | Tests, edge cases, runtime verification | `browser-tester.agent.md`, `visual-qa.agent.md` |
| Demo/Submission Lead | README, screenshots, architecture, narrative, evidence | Use task-specific documentation/review guidance |

## Ownership

- One primary implementation owner integrates code.
- Specialists should default to read-only analysis/review unless a write is explicitly assigned.
- Never let multiple agents edit the same file concurrently without coordination.
- Each agent records concise evidence and next action.

## Handoff format

Every handoff should answer:

**Objective**  
What decision or task was owned?

**Evidence**  
What was actually observed or verified?

**Decision**  
What is recommended/accepted/rejected?

**Changed files**  
Only paths actually modified.

**Verification**  
Commands/checks/results actually observed.

**Risks / unknowns**  
What remains uncertain?

**Next action**  
Exact next owner/action.

## Suggested orchestration

### Before implementation
Run research/review roles in parallel.

### Architecture
One architect consolidates specialist findings into a single implementation plan.

### Build
One primary builder owns integration; supporting specialists review bounded surfaces.

### Verification
QA, security, responsive, and browser reviewers independently inspect the result.

### Submission
Demo/submission owner checks that the public narrative matches actual implementation.

## Anti-duplication rule

Do not ask five agents to “review the repository” independently. Give each one a different decision surface.

## Stop condition

Agents must stop and report a conflict when:
- prompt requirements are ambiguous and materially affect architecture;
- sources conflict on a security-sensitive fact;
- an external integration is not verified;
- a requested action would violate hackathon rules;
- a tool result is insufficient evidence.

## Pre-hackathon rule

No agent may create the final prompt-specific product before the official prompt reveal.
