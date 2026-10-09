# Dispatch agent and tool failure recovery

The dispatcher executes the master controller's approved scope and can organize files, create windows, transmit packets, count/check and report. It can choose ordinary mechanics (file naming within conventions, retrying a failed page) but cannot make contested scholarly or publication decisions.

## Handoff command contract

A controller-to-dispatch message must state: phase, approved inputs and versions, authorized actions, forbidden operations, result filenames, quantitative gates, failure/stop triggers, and return report. Prefer a short change request over resending the full orchestration prompt every turn.

## Browser/session integrity

For each browser GPT writer/reviewer call, record session identifier, role, model configuration, input upload/paste manifest, receipt confirmation where possible, actual output and potential truncation. Separate writer and reviewer contexts. Failed navigation, SSL errors, partial uploads and duplicate sends are **not** evidence of completed output. Retry idempotently: inspect session state and version ledger before re-sending. Do not invoke the same text-generation step twice if an earlier result exists and is awaiting capture.

## Stop and escalate

Stop the affected branch for: no confirmed source/packet, unresolved substantive conflict, illegal or unsupported claim that requires changed policy, exhausted round cap, missing required upstream lock, corrupted file, unknown document element, inconsistent hash, or unauthorized mutation. Unrelated branches may continue within existing user authorization.

Return a decision request with: the exact blocker, its evidence, which unit/versions are affected, options and consequences, safest non-destructive next action. Preserve all records and do not pretend a milestone is complete because the user's goal remains active.
