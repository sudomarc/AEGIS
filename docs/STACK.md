# AEGIS Candidate Stack

## Status

**Candidate stack — prompt-gated.** The stack is intentionally small and can be changed after the official prompt reveal.

## Default

| Layer | Choice | Reason |
|---|---|---|
| App | Next.js App Router | Full-stack web app in one repository |
| Language | TypeScript | Type safety across UI/API/contracts |
| UI | Tailwind CSS + shadcn/ui | Fast, consistent, accessible component base |
| Validation | Zod | Runtime validation for external/user data |
| AI orchestration | Vercel AI SDK | Provider abstraction, structured generation, tool/agent support |
| Primary AI provider | Featherless AI | Hackathon participant access and open-model breadth |
| Model selection | Prompt-dependent | Choose only after requirements/evaluation are known |
| Database | None initially | Avoid unnecessary state/infrastructure |
| Database if needed | Postgres/Supabase | Add only if persistence is required |
| Workflow automation | n8n Cloud | Add only when external workflows materially improve the solution |
| Deployment | Vercel | Fast preview/production deployment |
| Tests | Vitest + Playwright | Unit/integration + browser verification |

## Architecture principle

Start with:

`Browser → Next.js → server-side AI boundary → Featherless → result`

Add storage, retrieval, workflows, external tools, or agents only when the prompt and evidence justify them.

## AI provider boundary

Keep application code provider-agnostic:

`AI service contract → provider adapter → model`

Do not spread provider-specific SDK calls throughout UI components.

## API guardrails

Application-level guardrails should be explicit. Provider behavior must not be assumed.

Recommended controls:
- request timeout;
- maximum request body/input size;
- maximum output tokens where supported;
- maximum tool-call count per request;
- retry limit;
- rate limit per user/session/IP as appropriate;
- concurrency limit where appropriate;
- total request budget for expensive workflows;
- structured validation of model output;
- fail-safe fallback/error state.

These controls reduce accidental cost, runaway loops, and unreliable behavior. They are engineering controls, not evidence of any hidden provider-side token limiter.

## Security

- all secrets server-side;
- no API keys in client bundles;
- validate every untrusted external input;
- restrict tools to allow-listed capabilities;
- never execute untrusted generated code;
- synthetic fixtures for security demos when possible;
- redact sensitive data from logs.

## Model selection protocol

After the prompt reveal:
1. Define the task type.
2. Define measurable success criteria.
3. Shortlist compatible models.
4. Verify current model availability and context/tool capabilities against provider documentation.
5. Run a small controlled comparison.
6. Select the simplest model that meets the measured requirement.

Do not choose a model solely because it is popular.

## Deployment

Use Vercel previews for rapid verification. Production deployment should happen only after a passing build and a focused browser/runtime check.

## Non-goals

We are not building:
- a microservice platform;
- a general AI assistant;
- a custom model-serving cluster;
- a multi-database architecture;
- infrastructure that does not directly support the hackathon product.



## Hackathon-provided tooling

The candidate stack is deliberately compatible with the participant perks advertised by ForgeHacks. These are accelerators, not mandatory dependencies.

Preferred use during the event:
- **Featherless AI** for model experimentation and production AI calls when its current access fits the task.
- **n8n Cloud Pro** for justified workflow automation or tool orchestration.
- **Momen / Adaption** only when they materially reduce build time or add required functionality.
- **DevSwarm** as an AI coding aid if useful to the team.
- **Tin Computer** is a post-event/after-distribution capability according to the current official site, so do not assume it is available during the build window.

Do not design around a sponsor perk that has not been activated or whose current terms differ from the public page.
