# GPT Academic Orchestrator

**A reusable, evidence-bounded GPT master-control protocol for long-form academic writing.**

This repository is intended for a **ChatGPT master-controller conversation** coordinating a human author, a local tool/dispatch agent (such as Codex), and isolated GPT writer/reviewer conversations.

The master controller makes academic plans and recommends or records authorized decisions. Codex dispatches and tracks work; it is not the scholarly decision-maker. The human user remains the final decision-maker.

## What it does

- Recovers state accurately after a chat ends or context fills up.
- Separates research evidence, user-approved scholarly decisions, and execution state.
- Builds minimal, versioned section packets with upstream/downstream contracts.
- Uses independent writer and reviewer sessions, bounded revisions and traceable LOCKED outputs.
- Detects mechanical count and non-prose document issues before expensive review.
- Provides a staged plan for cross-section integration, fact/citation audit, Word fidelity and delivery.

## Quick start with AI-MarkDone in ChatGPT

Save this **shortcut text** under a trigger such as `\\master` (replace URL if forking):

```text
Please read https://github.com/felicis18080925000-design/gpt-academic-orchestrator/blob/main/SKILL.md as a Skill-like protocol, then act as the GPT master controller described there.
Read only the relevant reference files for my current task. Identify exactly what you successfully accessed; if a critical file is inaccessible, stop and say so.
This is not a native Skill installation. You cannot access my local Codex files without an attachment/connector.
Recover state using the latest handoff package I attach; do not infer completed work from prior chat or start a new phase without authorization.

Current task:
```

**Important:** Reading a GitHub document through a URL does not install or persist a native ChatGPT Skill. Each new master conversation must read the protocol or an otherwise equivalent available copy, and must receive current project state. AI-MarkDone only inserts text into the prompt field.

## Repository layout

```text
SKILL.md                       Entry point and binding constraints
references/authority-and-state.md
references/research-and-decisions.md
references/packets-and-fidelity.md
references/review-and-lock.md
references/dispatch-and-recovery.md
references/integration-and-audit.md
templates/PROJECT_HANDOFF.md
templates/DECISION_REQUEST.md
templates/REVIEW_REPORT.md
templates/CHANGE_REQUEST.md
 tests/acceptance-scenarios.md
```

## How to incorporate it into a project

Keep your project-specific `MASTER_CONSTITUTION`, `SOURCE_OF_TRUTH`, `WRITING_STATUS`, locked texts, source documents and user approvals **outside this public repository**. Use `templates/PROJECT_HANDOFF.md` when starting a new ChatGPT master conversation. This repository stores **procedure**, not private client content or a project's substantive decisions.

Do not paste the user's local computer paths into a public repo with personal material. Avoid posting unpublished manuscripts, private source materials, API tokens, email addresses or internal research records.

## Status

`v0.1.0` — candidate protocol. Its controller, section packet, reviewer, mechanical-count, and LOCK principles were informed by an ongoing real-world workflow. Its general-purpose integration and delivery tracks are proposed practices, **not independently demonstrated by publishing a complete manuscript**. No claims of exhaustive testing are made.

## Version pinning

For important projects, record the exact Git commit SHA and link to that revision of `SKILL.md`, instead of silently accepting changing rules from `main`. A project may intentionally upgrade protocol versions after an explicit stage gate. Historical locked work should never be retroactively marked compliant with a new version unless actually checked.

## Governance and maintenance

Substantive changes to stage gates or authority boundaries need user review. Prefer PRs, preserve change history and keep the main protocol relatively short. Skill text is read as procedural documentation, not as authority to override the user's higher-priority instructions or safety requirements.