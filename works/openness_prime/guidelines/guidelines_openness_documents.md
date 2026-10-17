---
Originator: gdl
Contributors: ChatGPT-6
When: 2026-10-15T10:47:30Z
Status: tentatively accepted; needs review
---

# Openness Document Guidelines

## Scope and canonical format

The canonical Openness Library files are UTF-8 plain-text documents with a .txt extension. Markdown (.md) renderings may be produced for convenience, but are derived copies and do not supersede the corresponding canonical .txt documents. Use simple, readable plain-text formatting in canonical files.

All canonical Library documents, including indices and guidelines, must begin with exactly one metadata block. Do not put a document heading, introductory note, or Markdown fence before it. Document properties belong in that single block, not as a second block or loose key-value fields beneath the reader-facing title.

## Required metadata template

---
Title: <value>
Short-Title: <value>                 [optional; omit entire line when unused]
Authors: <comma-separated people and AI identifiers>
Editors: <comma-separated people and AI identifiers>
Created: <ISO 8601 UTC timestamp ending in Z>
Updated: <ISO 8601 UTC timestamp ending in Z>
---

(The indented lines above illustrate a single opening metadata block, not an additional block within this guidelines document.)

### Metadata rules

The Title is the full document title. A Short-Title is optional, and when present must immediately follow Title.

Exactly one metadata block is permitted per document, always at the top. Additional document-specific fields may be appended within it as needed using one "Key: Value" field per line (e.g. Tradition, Type, Status, Tags). Keep the required fields in their prescribed order; optional fields follow the required fields, except Short-Title, which immediately follows Title.

Do not repeat metadata properties as separate "Key: Value" lines following the reader-facing document title. A prose heading such as "Definition" or a saltem hoc marker such as "At least this:" is content, not metadata.

Authors and Editors list actual contributors to those roles, in a comma-separated list. Include relevant human and AI participants; do not invent real names. Use a neutral descriptor such as "Human collaborator (name not supplied)" when a name is unavailable.

Identify an AI author or editor by product, model, and version separated with hyphens, for example "ChatGPT-GPT-6". The document metadata identifies AI contributors; reader-facing saltem hoc editorial bylines follow different rules.

Created is the canonical document creation time, written as a full ISO 8601 UTC timestamp with a terminal "Z" (e.g. 2026-10-12T14:30:00Z). It does not change when the file is edited.

Updated is the last editorial modification time, also in UTC ISO 8601 with Z. Update it whenever the file's editorial content or metadata changes; this timestamp functions as the version identifier. Render-only exports need not change the canonical Updated timestamp.

If migrating a legacy document whose original creation instant cannot be reliably determined, use the first canonical .txt creation time and explicitly note in the Library index that the original drafting date is unknown. Do not invent exact historical timestamps.

Place one blank line after the closing --- before the document's reader-facing title or text.

## Title and filename conventions

Canonical filenames are lowercase snake_case and end in .txt. Prefer descriptive, stable filenames.

All saltem hoc contemplations must use the rules in Saltem Hoc Guidelines. Their titles are a single plain-language question. The default filename is that question normalized to lowercase snake_case, with punctuation removed.

For a long or awkward question, a Short-Title may be included. The Short-Title must begin "Saltem Hoc:", and the filename must begin "saltem_hoc_" followed by snake_case words from its short title. The canonical Title remains the full question.

Every document defining a named Openness term or concept is a Definition. Its Title must begin "Defining " followed by the term, and its filename must begin "defining_" followed by the lowercase snake_case term. Example: Title "Defining The Refinement Of Choosing", filename "defining_the_refinement_of_choosing.txt".

Every Guidelines document defines the writing, format, or editorial conventions for an Openness document type or for the Library as a whole. Its Title must be "<X> Guidelines", and its canonical filename must be "guidelines_<x>.txt", where x is the lowercase snake_case form of X. Examples: "Saltem Hoc Guidelines" -> "guidelines_saltem_hoc.txt"; "Openness Document Guidelines" -> "guidelines_openness_document.txt".

Record document classes in the single metadata block using "Type: Definition" or "Type: Guidelines" as appropriate. Optional descriptive properties such as Focus or Applies-To may follow the required metadata keys.

Library indices use descriptive titles and lowercase snake_case .txt filenames.

## Attribution distinction

The optional saltem hoc attribution line belongs below the reader-facing question, with NO "Source:" prefix. Use "Philosophical Openness AI v1:", "Spiritual Openness AI v1:", or, for AI material edited by a human, a v1x variant. The "Openness GPT vN" form remains reserved for the existing Openness role-play AI. See the Saltem Hoc Guidelines for details.

## Migration and maintenance

Keep one canonical .txt file for each logical document. Derived aggregate/readable Markdown forms may be generated separately. For compiled readings, preserve a single top-level metadata block and omit the embedded metadata headers of constituent documents; the canonical files remain the source of their metadata.

When a previous document combines definitions of several named concepts, split it into separate "Defining " documents when sensible; do not silently delete substantive commitments.

When a saltem hoc title combines independent questions, refactor into single-question contemplations. Preserve the previous approved work and identify significant rewriting as proposed pending editorial review.

On each edit, update the document's Updated timestamp and synchronize the Library index and exports.

Any cross-references should point to canonical filenames rather than retired Markdown sources.
