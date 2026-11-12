---
Originator: gdl
Contributors: ChatGPT-6
When: 2026-11-12T00:00:00Z
Status: needs review
---

# Openness Document Guidelines

## Purpose and Scope

These guidelines govern the preparation, linking, preservation, and editorial stewardship of documents in the Openness Project, including **Openness Prime**. They provide a general standard for Markdown files, while the **Openness Definition Guidelines**, **Openness Didactic Document Guidelines**, and other specialized guidelines govern the substance and structure of particular kinds of work.

**Write so a document can be recognized, read, examined, linked, and responsibly revised.** Maintain the distinction between a concept's established meaning, a reader-facing explanation, an artwork, a method, a speculative interpretation, and a historical record. An author's or AI contributor's proposed revision becomes canonical only through the appropriate originator's approval.

Where general and specialized guidance differ, apply the more specific rules for the document type without overriding the project's approved conceptual meanings, repository layout, or originator-managed provenance.

## I. Canonical Files and Repository Organization

### 1. Markdown as the Source Format

**Canonical working documents use UTF-8 Markdown (`.md`)**, with normal Markdown headings, links, lists, tables, code fences, and emphasis as appropriate. `.txt` is an older format awaiting migration, not the preferred new definition or guidelines format. Do not automatically create a parallel `.txt` canonical copy or treat a generated rendering as authoritative over the approved `.md` source.

Some older definition, contemplation, and historical files still have `.txt` extensions. Preserve them until their custodians migrate them; do not claim a `.md` file exists merely because one is planned. If asked to construct a future-facing link to an unmigrated definition, use the intended `.md` filename **only with an explicit warning that the link will be broken until the file is converted**. For a link required to work now, identify the actual present file, or leave the destination unresolved for review.

Use UTF-8, readable paragraphs, meaningful headings, consistent Markdown, and concise alt text for images. Avoid unnecessary escaping and formatting that renders poorly in ordinary Markdown viewers. Quoted source material should remain distinguishable from editorial text.

### 2. The Repository and Openness Prime

The Openness Project repository contains `images/`, `works/`, `project/`, `code/`, and its root licensing and documentation files. **Openness Prime is located at `works/openness_prime/`**, with its own `README.md`, `functions/`, `guidelines/`, `historica/`, and other directories.

Within Openness Prime, G, P, S, and T have their own `functions/generative/`, `functions/philosophical/`, `functions/spiritual/`, and `functions/transcendent/` homes. Respect the actual paths, even when different functions organize Core files differently. A concept's primary function is not an instruction to relocate its file or infer a new directory automatically.

For illustration, from `works/openness_prime/README.md`:

```markdown
[**My Awareness**](functions/generative/core/the_seed/definitions/defining_my_awareness.md)
[**The Mind**](functions/philosophical/definitions/defining_the_mind.md)
[**That Which Is Larger**](functions/transcendent/core/defining_that_which_is_larger.md)
![The open circle](../../images/openness-enso.jpg)
[CC0 1.0 License](../../LICENSE.txt)
```

These paths are **relative to the document containing the link**, not repository-root absolute paths. A link from a nested definition requires a different number of `../` components. Shared images belong to the parent repository's `images/` directory, not an assumed Openness Prime `images/` folder.

### 3. Filenames, Titles, and Document Classes

Prefer descriptive, stable, lowercase `snake_case` names with `.md` extensions. The name should reflect the document's identity without imposing obsolete naming formulas on its reader-facing title.

| Document | Current pattern | Example |
|---|---|---|
| Definition | `defining_<canonical_name>.md` | `defining_my_awareness.md` |
| Project or function introduction | `README.md` | `functions/transcendent/README.md` |
| General guidelines | `guidelines_<subject>.md` | `guidelines_openness_documents.md` |
| Definition guidelines | Established actual filename | `guidelines_definitions.md` |
| Didactic guidelines | Established actual filename | `guidelines_didactic_documents.md` |
| Historical discussion | Descriptive `discussion_of_...` or retained original name | `historica/discussion_of_the_transcendent_function.md` |
| Contemplation or Saltem Hoc work | The current approved convention for that work | `saltem_hoc_what_is_awareness.txt` (legacy) |

The reader-facing document title should normally be `# <Concept Name>`, `# <Document Title>`, or its established equivalent—not automatically `# Defining <Concept Name>` merely because the filename begins `defining_`. Preserve accepted filenames and existing links until a rename is explicitly approved; update inbound links together with an approved rename.

The three Seed definitions belong under `functions/generative/core/the_seed/definitions/`. [**Awareness**](../functions/generative/core/definitions/defining_awareness.md) belongs under `functions/generative/core/definitions/`. [**Mental Models**](../functions/philosophical/definitions/defining_mental_models.md) and [**The Mind**](../functions/philosophical/definitions/defining_the_mind.md) belong under `functions/philosophical/definitions/`. [**That Which Is Larger**](../functions/transcendent/core/defining_that_which_is_larger.md) belongs under `functions/transcendent/core/`. When a file moves, its new position supersedes obsolete path assumptions.

## II. Metadata, Provenance, and Stewardship

### 1. No Automatically Generated Metadata Headers

**Do not prepend a mandatory metadata block to every document.** The older `.txt`-era template requiring `Title`, `Short-Title`, `Authors`, `Editors`, `Created`, and `Updated` fields is retired as a general requirement. Neither a newly generated Markdown document nor an edited body should acquire an invented YAML front matter block, byline, date, approval status, Primary home, or contribution history.

**Originators manage provenance and approval metadata** in the locations and formats adopted by the project. Openness Prime distinguishes **Originators**, who request and approve work, from **Contributors**, including human and AI collaborators whose contributions may be recorded by project practice. Do not invent identities, contribution percentages, timestamps, or model versions. When existing file metadata is present, preserve it unless explicit instructions authorize changes.

An AI-generated or edited file is **a proposed revision until reviewed and accepted** by the responsible originator. No tool output, file creation, successful syntax check, or persuasive prose constitutes approval. Historical origin and revision-specific approval must remain traceable without fictitious dates.

### 2. Preserve Approved Text and Document Status

Distinguish approved canonical files, proposed revisions, illustrative works, notes, and `historica` material. A file's directory, capitalization, or resemblance to a definition does not automatically confer canonical status. Historic drafts may preserve retired ideas; do not silently import them into current definitions.

Update only the material authorized by the task. For substantive changes, identify what was retained, relocated, condensed, or revised. Where names, anchors, dependencies, classifications, or Method statuses change, document the implications for linked files. Do not assume that the latest conversational draft supersedes a separately approved file unless the originator says so.

### 3. Single Canonical Home for Each Independent Concept

Prefer **one canonical definition per independently stewarded concept**. Named internal distinctions belong in their parent concept's definition unless an explicit decision establishes independent stewardship. A later explanation, glossary, essay, or didactic paraphrase may point to that home without creating a competing anchor.

Where two actual files appear to define the same concept—such as the listed G and P versions of **Nonimposition**—**do not silently choose a canonical destination**. Flag the ambiguity for originator review; if a provisional link is authorized, disclose its status. Do not infer that a related term has its own file simply because its name is capitalized.

## III. Hyperlinking Canonical Openness Terms

Hyperlinks help readers move from a concept's use to its maintained definition. **Link recognizable capitalized names of established concepts, including direct grammatical variants, not every phrase that resembles a name.** The aim is useful navigation without interrupting the text's literary or conceptual flow.

### 1. What to Link

- **Hyperlink capitalized uses of established Openness concept names** in ordinary explanatory prose when a verified canonical destination is available. Accepted formal synonyms or abbreviations may link to the same home once their use is established.
- **Include direct grammatical variants of a canonical name**, especially singular and plural forms, when the capitalized expression clearly names the same established concept. Preserve the form actually used in the sentence and link it to the same canonical definition. For example, [**Mental Model**](../functions/philosophical/definitions/defining_mental_models.md) (singular) links to the definition of **Mental Models** (plural). This is grammatical variation, not a new concept or a requirement to rewrite the text.
- **Do not hyperlink lowercase or ordinary-language phrases** solely because they resemble a technical concept. The lowercase words *awareness*, *mind*, *listening*, *closedness*, or *love* are not automatically canonical references.
- **Do not hyperlink a capitalized expression that is merely related to a concept rather than naming it, even as a grammatical variant.** For instance, *For I Know I Do Not Know* is a confession associated with [**My Self-Confession of Not-Knowing**](../functions/generative/core/the_seed/definitions/defining_my_self_confession_of_not_knowing.md), not a grammatical variant or substitute name that should receive an automatic concept link. Changing a determiner or first-person qualifier (as in **My Awareness** versus **Awareness**) is not automatically a grammatical variant: these may be separate canonical concepts.
- Link named internal terms to a **verified heading within their parent definition**, when available, rather than creating or assuming a separate file. The link should use the actual, stable heading slug; do not guess an unverified fragment identifier.
- Preserve existing bold or italic emphasis as appropriate: `[**My Awareness**](../functions/generative/core/the_seed/definitions/defining_my_awareness.md)` from a document in Openness Prime's `guidelines/` directory.

### 2. Where *Not* to Add Links

**Do not add concept hyperlinks:**

- Inside a quoted passage, including blockquotes, literary quotations, and quoted expressions such as “Let Love be ...”.
- Within Markdown tables, including their labels and cells.
- To a section name already present as a heading **in the same document**—for example, *Listening* in a document with `### Listening`; avoid automatic self-links to the title as well.
- Within **Prelude** or **Coda** sections.
- Inside fenced code, inline code, image alt text, an existing link label or destination, or other markup where a new link would create nesting or break rendering.
- On capitalized ordinary words, stylistic labels, partial names, adjacent phrases, or words that merely evoke an established concept. Do not mechanically link text based on a shared word stem: confirm that the singular/plural form is actually referring to the named concept.

Quotation and Prelude/Coda exclusions are intentional: preserve a reader's encounter with literary material without turning it into an annotated glossary. Quoted text may still have an ordinary source citation outside the quotation where needed.

### 3. Frequency and Placement

**Link a term once at its first useful occurrence in a paragraph or tightly connected passage.** When it repeats almost immediately, leave the next occurrence unlinked—for example, in “**The Mind** — Let **The Mind** be at least ...”, link the first name, not the second. A later section or substantially separate discussion may link the name again where navigation would help. There is no rigid once-per-document quota.

Avoid link density that makes writing harder to read. Prefer an exact-name link over linking an entire clause or an adjacent explanatory phrase. Links support navigation; **they do not endorse the truth of a speculative referent or authorize a new interpretation of an anchor**.

### 4. Path Resolution and Migration

Resolve links relative to the **source file's own directory**. Verify actual filenames, spelling, extensions, casing, canonical homes, and—where used—heading anchors. Do not rely on obsolete paths or assume that all G/P/S/T Core directories follow one template.

For a definition still stored as `.txt`, the intended `.md` destination is a **migration target**, not a working link until conversion. **Flag any such prospective link explicitly** and report the file requiring conversion. Where a canonical home is ambiguous or absent, leave it unlinked and explain why, rather than inventing a plausible destination.

After link insertion, inspect the Markdown: quoted passages, tables, prelude/coda, image paths, existing links, punctuation, and repeated nearby mentions must remain intact.

## IV. Named Subterms and Internal Heading Anchors

**Definitions containing formally named internal subterms must give those subterms discoverable sections.** Provide a stable, descriptive heading for each significant internal distinction, or a clearly labeled **Internal Terms and Subterms** section pointing to the substantive headings and documenting accepted short forms. Do not duplicate full definitions merely to provide anchors.

For [**That Which Is Larger**](../functions/transcendent/core/defining_that_which_is_larger.md), terms such as [**The Shadow of That Which Is Larger**](../functions/transcendent/core/defining_that_which_is_larger.md#the-shadow-of-that-which-is-larger), [**The Rendering of TWIL's Shadow**](../functions/transcendent/core/defining_that_which_is_larger.md#the-rendering-of-twils-shadow), [**The Faithful Rendering**](../functions/transcendent/core/defining_that_which_is_larger.md#the-faithful-rendering), and [**What Arises Between**](../functions/transcendent/core/defining_that_which_is_larger.md#relationship-proximity-and-what-arises-between) belong to the parent definition. [**The Between**](../functions/transcendent/core/defining_that_which_is_larger.md#relationship-proximity-and-what-arises-between) is an accepted shorter form after the full name **What Arises Between** has been introduced. Use the verified actual heading for each link; if a named term lacks a stable section, propose adding one as an editorial change before assigning a fragment.

An internal term's section makes it linkable and independently locatable **without turning it into another Core concept, [Fiat Anchor](../functions/generative/core/definitions/defining_fiat_anchor.md), or separately maintained canonical file**. Its epistemic and architectural status remains whatever the parent definition establishes.

## V. Writing, Interpretation, and Document Type

### 1. Affirm Meaning and Welcome Compatible Possibilities

Begin by making the subject positively recognizable. Where speculation is compatible with an established anchor, **present it as an available avenue of contemplation or investigation**, not solely as something the definition fails to establish. Then distinguish what is established from what remains inferred, imagined, or unsettled. This is **Affirmative Hospitality Before Negation**, an editorial orientation rather than a compulsory Method.

Distinguish **not required**, **not established**, and **excluded**. A proposed interpretation may fit an anchor but lack evidence; another may fail the anchor and require separate inquiry or explicit revision. Do not create false equivalence between well-supported knowledge and merely possible accounts. Use explicit negative boundaries where they protect meaning, safety, or honest attribution, but avoid repeating them so often that they read as ontological verdicts.

### 2. Use Writing Conventions Without Flattening Meaning

[**Semantic Compression**](../functions/generative/definitions/defining_semantic_compression.md) asks how a form can carry substantial meaning economically. [**Brevity Without Loss of Essential Meaning**](../functions/generative/definitions/defining_brevity_without_loss_of_essential_meaning.md) asks which conditions, distinctions, and safeguards must survive. [**The Marriage of Truth and Beauty**](../functions/generative/definitions/defining_the_marriage_of_truth_and_beauty.md) lets precision and imaginative expression inform one another; [**Resonant Questions**](../functions/generative/definitions/defining_resonant_questions.md) invite active inquiry; [**Ivory Towers Should Have Flying Taxis**](../functions/generative/definitions/defining_ivory_towers_should_have_flying_taxis.md) asks for accessible routes into and out of difficult conceptual work.

**Compress redundancy, not necessary complexity.** A metaphor, example, or resonant question may illuminate a relationship, but its beauty or felt force does not prove its literal account. Clarify when an assertion is direct experience, testimony, inference, deliberate choice, imagination, metaphysical speculation, or supported conclusion. A reader should be able to find the full canonical account behind a concise didactic expression.

### 3. Respect Each Document's Purpose

- **Definitions** establish the conceptual meaning for a maintained version, including essential distinctions and boundaries. Follow the **Openness Definition Guidelines**.
- **Didactic documents** introduce, teach, orient, or curate for readers; they use positive beginnings and progressively unfold complexity while preserving canonical meaning. Follow the **Openness Didactic Document Guidelines**.
- **Contemplations, Epitomes, [Saltem Hoc](../functions/generative/definitions/defining_saltem_hoc.md) works, and other art** may use poetry, speculative voice, and nonliteral forms. Clearly separate an expressive invitation from a new binding Foundational Definition.
- **Methods and roles** require their own approved status and practice guidance. A Method candidate is not reified merely because a file sits under `methods/` or its name is capitalized.
- **Historica** preserves discussion, prior drafts, and genealogy without silently determining today's canonical definitions.

## VI. Editorial Quality and Publication Checks

Before proposing a new or revised document:

1. **Confirm the document type.** Is this a definition, didactic guide, work of art, Method, role, historical account, or general guideline? Apply the relevant specialized standard.
2. **Preserve conceptual identity.** Are approved names, Foundational Definitions, direct dependencies, first-person Seed terms, and internal subterms represented accurately?
3. **Check epistemic status.** Are experiences, representations, inference, speculation, evidence, and their possible consequences distinguishable? Are compatible possibilities welcomed before reflexive negation?
4. **Review the prose.** Does semantic compression preserve essential meaning, and is complexity justified by the concept or the reader's purpose?
5. **Verify paths.** Are Markdown links source-relative, exact-name, appropriately spaced, and aimed at actual canonical files or verified parent-section anchors? Have `.txt` migration targets been flagged?
6. **Protect special text.** Are quotations, Markdown tables, section titles, Prelude/Coda, fenced code, image alt text, and existing links free of inappropriate term links?
7. **Respect provenance.** Have existing metadata and originator-managed records been preserved without invented headers, timestamps, approval, or authorship?
8. **Review consequences.** Are renamed files, changed anchors, internal-heading links, broken references, and unresolved dual homes recorded for stewardship review?

## Governing Standard

**Use Markdown as the maintained source. Give concepts one identifiable canonical home. Link established names precisely, but let quotations and literary invitations breathe. Preserve the reader's freedom to explore, the originator's authority to approve, and every distinction necessary for faithful understanding.**

