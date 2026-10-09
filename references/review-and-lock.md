# Writer, independent review, revisions and lock

## Writer session

The execution agent provisions a fresh isolated writer conversation with the exact approved packet and, where required, grounded excerpts of upstream locked text. First request a short understanding and paragraph plan. Check factual/authorization misread, omissions and scope drift mechanically/against packet. Only then ask for formal text. Save prompt, returned raw text, model/settings and session metadata without silent rewriting.

## Mechanical pre-review

Before sending to independent review, check exact required Unicode/category count (e.g. U+4E00–U+9FFF if specified), both body and total-inclusive counts; headings; tables and caption positions; format; completeness; truncation, duplicate passages, TODO/instruction residue, prohibited source versions and explicit downstream interfaces. Resolve count defects through a narrow writer-directed edit before asking the academic reviewer. Preserve the earlier raw candidate and change diff.

## Independent reviewer

Use a fresh session without writer history; give it the packet, current candidate, and relevant locked interfaces, not the first reviewer's verdict. Require one of `PASS`, `MINOR_REVISION`, `MAJOR_REVISION`, with: `HARD_ERRORS`, `WRITING_ISSUES`, `REVISION_INSTRUCTIONS`, `KEEP` and real source/paragraph locators. Evaluate substance, attribution, evidence scope, law/proposal boundary, interface, overall writing and mature wording. Reject cosmetic over-review.

- `PASS`: eligible for controlled lock after deterministic checks.
- `MINOR_REVISION`: narrowly revise the existing candidate in its original writer session; preserve all differences and re-review independently.
- `MAJOR_REVISION`: prefer a clean writer session with a bounded defect brief; do not loop indefinitely on a contaminated draft.

Round limits belong to the project config; never silently raise them. On exhaustion, stop and request an explicitly scoped exception. For a proven purely mechanical defect, the master controller may authorize a format-only waiver with a fixed transformation and deterministic diff check. Preserve reviewer original verdict; do not fabricate PASS.

## Lock

A locked unit has: immutable content/version, content hash, precise count, packet version, source provenance, actual reviewer outcomes, exception record if any, lock authority/date and links to raw and diff history. Changes require a new derivative version and approved change request; never overwrite the prior lock.

`LOCKED` means locally approved for integration, not already publication-ready. Conduct cross-unit review after all necessary upstream/downstream text exists.
