# README for Agents — wfi-scientific-canon-public

This file is written for AI agents (including Claude) working inside this
repository. Read it fully before touching any file.

---

## What this repository is

This is the **scientific canon** of the Welfare Footprint Institute (WFI).
It is not a software project. It is a structured, version-controlled archive
of peer-reviewed scientific commitments, methodological definitions, and
quantitative welfare frameworks.

---

## The WFF Chain — commit it to context

Every welfare assessment in this repository follows this causal chain.
Do not collapse, reorder, or conflate these levels:

```
Circumstances
    ↓
Biological Consequences
    ↓
Affective Experiences       ← welfare assessment centres here
    ↓
Welfare Metrics
```

**Key distinctions you must preserve at all times:**
- Circumstances ≠ Biological Consequences
- Biological Consequences ≠ Affective Experiences
- Welfare indicators ≠ Welfare metrics
- Affective Experiences must remain disaggregated by **valence** (pain vs. pleasure)
  and **intensity category**

---

## Module names — use these exactly

| ID  | Canonical Name |
|-----|----------------|
| I   | Zootechnical Description |
| II  | Veterinary Inventory |
| III | Affective Quantification |
| IV  | Epidemiological Review |
| V   | Econometric Calculation |
| VI  | Welfare Footprints: Expression and Notation |
| Ψ   | Interspecific Scaling / Interspecific Affect |

- **Never use "Aggregation and Standardization"** — deprecated. See `glossary/deprecated_terms.yaml`.
- **The deprecated tool name is "Pain-Track GPT"** when referring to the current broader GPT
  that now covers both Pain and Pleasure. Use "Hedonic-Track GPT" for that current tool.
  **Pain-Track remains a valid and important WFF term.** Do not mechanically replace
  Pain-Track in contexts referring to the Pain-Track method, Pain-Track notation,
  Pain-Track App, historical materials, or Pain-specific workflows.

---

## Rules for agents

### You MUST NOT:
- Change any file in `canon/` or `modules/` without explicit instruction from
  Wladimir J. Alonso or an authorised WFI reviewer.
- Treat a placeholder as settled science or fill it with invented content.
- Treat an open question as resolved.
- Introduce new terminology not approved in `glossary/wff_terms.yaml`.
- Store secrets, credentials, private emails, funder-sensitive details,
  HR/personnel material, legal/board-sensitive material, or operational clutter.
- Create Atlas, WFKG, schemas, validators, MCP servers, agents, dashboards,
  product code, content studio, or ops assistant infrastructure here.
- Migrate large external documents into this repository without explicit approval.
- Commit directly to `main`.

### You MUST:
- Preserve WFF terminology and module boundary definitions.
- **Preserve primary WFF outputs as disaggregated Cumulative Pain and
  Cumulative Pleasure by intensity category.** Do not net Pain against
  Pleasure, collapse intensity categories, or present scalar / value-weighted
  welfare scores as primary WFF outputs.
- **Aggregation must sum like with like** — within the same valence and
  intensity category. Do not collapse, weight, net, or create equivalences
  across intensity categories or across valences as primary WFF outputs.
- If a user asks for a scalar, weighting, netting, or decision-analysis
  transformation, treat it as an **external downstream transformation**,
  label it explicitly as non-primary WFF, preserve the underlying
  disaggregated WFF outputs alongside, and state the added assumptions.
- Make assumptions and uncertainty explicit in any content you draft.
- When uncertain about a scientific claim, create a note in `review/` rather
  than silently editing canon.
- Follow the commit style: imperative subject line, 72-character max, e.g.
  `add: draft uncertainty note for Module III`.

---

## How to read placeholder markers

Files in this repository use the following markers:

| Marker | Meaning |
|--------|---------|
| `[PLACEHOLDER — requires scientific review]` | Content not yet authored; do not fill without human approval |
| `[OPEN QUESTION]` | Genuinely unresolved; do not treat as settled |
| `[DEPRECATED]` | Term or concept superseded; see glossary |
| `[DRAFT]` | Content drafted but not yet reviewed |

---

## Branching

- `main` — stable, reviewed canon only
- `draft/<topic>` — work in progress
- `review/<topic>` — awaiting peer review

Never push directly to `main`. Always work on a branch.

---

## Source documents — critical rules

Source documents are listed in `sources/source_registry.yaml`.
They are **reference material**, not automatically merged canon.

### You MUST NOT:
- Treat a source document as canon simply because it exists in the registry.
- Silently resolve a conflict between a source document and existing canon wording.
- Populate `[PLACEHOLDER]` markers by copying text from source documents
  without explicit human approval.
- Copy full source documents (PDFs, manuscripts, DOCX files) into this repository.

### You MUST:
- If a source document contradicts existing canon wording and no explicit
  deprecation or terminology rule in this repository already resolves it,
  create an entry in `review/source_conflicts.md` and stop.
- Use the citation format defined in `sources/citation_policy.md`.
- Cite the OSF preprint (`https://doi.org/10.17605/osf.io/94bxs`) as the
  primary WFF methodology reference until the Animal Sentience journal
  version is published.

### Known terminology notes from sources:
- "Econometric Calculation" is the current Module V term in canon, aligned with
  the primary WFF methodological source and the Technical Definitions source.
  "Aggregation and Standardization" appeared in earlier repository scaffolding
  and is **deprecated**. See `review/source_conflicts.md` SC-001.
- Some sources may use "Pain-Track GPT" as a tool name.
  The current tool name is "Hedonic-Track GPT."
  Pain-Track itself remains valid for the method, notation, app, and
  negative-affect-specific workflows.

---

## If you are unsure

Create a file in `review/` describing the uncertainty and stop.
Do not guess. Do not fill placeholders. Do not synthesise canon.
