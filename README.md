# OpenClaw / Klause · Agent Architecture Showcase

This repository documents the parts of my OpenClaw/Klause agent setup that can be shown publicly: roles, permissions, review gates, synthetic traces and reliability checks.

It is intentionally not a dump of the raw operating system. Real prompts, logs, memory files, customer data, lead data, credentials, internal strategy and revenue material are excluded.

## What this shows

- how a multi-agent workflow can be split into roles, permissions and review gates
- how autonomous tasks need boundaries before they touch public channels or customer-facing actions
- how synthetic traces can explain behavior without leaking private runtime data
- how to document risks honestly instead of presenting a magical agent demo

## Review in 2 Minutes

| What to check | Where |
| --- | --- |
| Architecture | [ARCHITECTURE.md](./ARCHITECTURE.md) |
| Permissions | [PERMISSION_MATRIX.md](./PERMISSION_MATRIX.md) |
| Synthetic run | [SYNTHETIC_TRACE.md](./SYNTHETIC_TRACE.md) |
| Risks and limits | [THREAT_MODEL.md](./THREAT_MODEL.md) |
| Smoke tests | [EVAL_SMOKE_TESTS.md](./EVAL_SMOKE_TESTS.md) |

## Documents

- [ARCHITECTURE.md](./ARCHITECTURE.md) — redacted architecture overview
- [PERMISSION_MATRIX.md](./PERMISSION_MATRIX.md) — what agents may do automatically and what requires human approval
- [SYNTHETIC_TRACE.md](./SYNTHETIC_TRACE.md) — safe example trace with fake data
- [THREAT_MODEL.md](./THREAT_MODEL.md) — public-release risks and mitigations
- [EVAL_SMOKE_TESTS.md](./EVAL_SMOKE_TESTS.md) — checks used to think about reliability and release safety

## Public boundary

This repo may be used as a portfolio artifact. It should never contain:

- secrets, API keys or environment files
- customer data, private leads, phone numbers or emails
- real prompts, raw logs, memory dumps or private dashboards
- internal strategy, budget, revenue or pipeline data
- executable outreach or calling automation

## Portfolio context

Main portfolio: [robert-systems.com](https://robert-systems.com)

Target frame: AI Implementation, Workflow Automation, AI Adoption and customer-facing AI systems.

## License

Portfolio/reference material. All rights reserved by Robert Dörries.
