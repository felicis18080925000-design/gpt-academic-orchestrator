# Authority, versioning and recovery

## Authority order

1. Latest explicit user instruction and authorization, within governing constraints.
2. Current project-specific, expressly approved master-controller decisions and constitution.
3. Current confirmed project status, versioned artifacts and dependency graph.
4. Verified primary sources and their provenance.
5. Historical plans, draft packets, past reviewer suggestions and chat summaries.

A newer state snapshot reports what happened; it does not itself change scholarly rules. Conflicts between the approved constitution and later state require a decision request. A public reusable Skill cannot override a project's specific authorization.

## Minimum project record

- `MASTER_STATE`: version, current stage, active goal, completed/blocked tasks, next allowed action.
- `MASTER_CONSTITUTION`: scholarly intent, constraints, terminology, approved rules and decision provenance.
- `SOURCE_OF_TRUTH`: claim/type, locator, reading scope, verification status, citation limits.
- `OPEN_QUESTIONS`: issue ID, status, severity, competing options, evidence status, dependencies, writing consequence.
- `SECTION_DEPENDENCIES`: real upstream/downstream, input/output contracts.
- `WRITING_STATUS`: per-section research/packet/writer/reviewer/lock/integration states.
- `VERSION_LOG` and `LOCK_MANIFEST`: raw origins, version paths, hashes, timestamp, exceptional authorizations.
- `DOCUMENT_ELEMENT_MANIFEST` when the source contains non-prose objects.

Names are examples and may be mapped to an existing project's files. Never regenerate authoritative project state merely because its current naming differs.

## Recover after chat/context loss

Require a concise handoff with paths or attached copies of current authoritative files and their versions. Distinguish a local Mac path appearing in text from an attached or otherwise retrievable file. Inspect the smallest necessary artifacts. Report mismatches: e.g. status says `LOCKED` but no lock manifest; reviewer says PASS for a different version; changed file hash; dependency points to an unapproved draft.

If a critical artifact is absent, say **not verified** and request it. Do not claim Codex or ChatGPT shares one continuous memory or file system. On confirmed checkpoint, authorize only the next bounded action.

## Decisions

Statuses: `OPEN`, `RESEARCHING`, `RESEARCHED`, `DECIDED`, `DEFERRED`. Distinguish `RESEARCHED` from `DECIDED`. Each decision records origin, date/version, option, reasoning, allowed/disallowed claims, interface effects and reopen criteria. Record a decision in the project ledger before propagating it to packets.