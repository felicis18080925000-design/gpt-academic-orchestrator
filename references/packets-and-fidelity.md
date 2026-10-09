# Architecture, packets and original-document fidelity

## Architecture and units

Build a dependency graph and argument map before splitting. Each unit must have a distinct claim and hand-off conclusion, attainable within its word budget. High-coupling units may be sequenced; independent ones may be concurrent. The execution agent may propose a split, but should not renumber or change substantive ownership without master-controller authorization.

## Minimum packet

Map to existing project conventions; a useful packet contains:

1. `TASK`: unit purpose, scope, word-count rule, output format, preserved/revised/omitted arguments.
2. `CONSTITUTION_EXCERPT`: directly relevant approved positions.
3. `SOURCE_OF_TRUTH_EXCERPT`: claims with verified scope, not a dump of all research.
4. `CURRENT_SOURCE_TEXT`: exact relevant source passages and stable paragraph IDs.
5. `ARGUMENT_PLAN`: paragraph-level reasoning and position/author attributions.
6. `CORE_EVIDENCE` and `LEGAL_SOURCES`: specific quotations/locators plus evidentiary boundaries.
7. `INTERFACE`: input and output contracts, dependency versions.
8. `STYLE_RULES`: target genre and mature wording preservation.
9. `DO_NOT_DRIFT`: highest-risk unauthorized inferences/changes.
10. `DOCUMENT_ELEMENTS` **when needed**: source element ID, type, location, owner, required treatment, output representation, final reattachment, counting rule.

All constraints must be internally consistent, especially if a document element must be retained but the output requests continuous prose only. Run packet QA before writer dispatch.

## Non-prose element contract

Inventory headings, tables, captions, footnotes/anchors, figures, equations, lists, comments, track changes and layout-sensitive empty paragraphs when present. Assign stable IDs and ownership, track retained/modified/removed/moved/deferred decisions with provenance. Check relationships, not mere survival: table-caption pairing, table-intro and following explanation, anchor-note pairing, internal cross-references and order.

The writer may output Markdown versions of simple tables **only if expressly permitted**, or an insertion marker whose corresponding authoritative original object is preserved for assembly. Do not pretend Markdown reproduces complex Word layout or silently flatten merged cells, citations and revisions.

Count words/characters by the project's stated definition, explicitly including titles, tables and captions whenever specified. Prevent duplicated argumentation after both a textual summary and an original table are restored. Report `ELEMENT_MISSING`, `OUTPUT_FORMAT_CONFLICT`, `FOOTNOTE_ANCHOR_LOST`, `OWNER_CONFLICT`, `COUNT_CONFLICT` and unapproved deletions.

For DOCX, extracting paragraphs through a simple document API may omit comments, revision changes or footnotes. Inspect OOXML or report the extraction limitation. Do not silently discard unknown embedded objects.

## Packet QC

Ensure claim and source scope, approved decisions, lengths, all source paragraphs and document elements' single ownership, no contradictions across packets, viable upstream content plans, acceptable context size and valid source IDs. An approved packet contract does not falsely imply that an actual upstream `LOCKED` draft already exists.
