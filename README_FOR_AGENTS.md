# README for Agents — wfi-scientific-canon-public

Read this file fully before changing any repository file.

## Scientific authority hierarchy

The authority order is:

1. the primary WFF methodological paper;
2. any formal amendment or addendum jointly approved by Wladimir J. Alonso and Cynthia Schuck-Paim;
3. the private scientific canon as the controlled, versioned operational representation of those scientific sources;
4. this public repository as a curated mirror;
5. downstream tools and applications.

Neither the private nor public repository independently creates or revises WFF scientific authority.

An Issue, review discussion, or merged Pull Request does not by itself amend the WFF.

See:

- `sources/wff_scientific_authority.md`
- `sources/citation_policy.md`
- `CONTRIBUTING.md`

## Repository role

This is not a software project. It stores the public teaching, citation, review, and retrieval representation of WFF terminology, module descriptions, source relationships, status, provenance, and review records.

Agents should normally improve fidelity to the WFF paper, approved amendments, and internal canon—not invent or redesign the framework.

## The WFF chain

Preserve this causal chain exactly:

```text
Circumstances
    ↓
Biological Consequences
    ↓
Affective Experiences       ← welfare assessment centres here
    ↓
Welfare Metrics
```

Key distinctions:

- Circumstances ≠ Biological Consequences
- Biological Consequences ≠ Affective Experiences
- Welfare indicators ≠ welfare metrics
- Pain ≠ Pleasure
- intensity categories remain disaggregated

## Module names

| ID | Name |
|---|---|
| I | Zootechnical Description |
| II | Veterinary Inventory |
| III | Affective Quantification |
| IV | Epidemiological Review |
| V | Econometric Calculation |
| VI | Welfare Footprints: Expression and Notation |
| Ψ | Interspecific Scaling / Interspecific Affect |

“Aggregation and Standardization” is deprecated for Module V.

## Agent prohibitions

Agents must not:

- change foundational WFF scientific content without a formal, jointly approved amendment record;
- treat instruction from one scientific authority acting alone as sufficient to amend the WFF;
- infer an amendment from a merged repository change;
- treat a placeholder as settled science;
- treat an open question as resolved;
- introduce new WFF terminology, modules, intensity categories, or methodological rules;
- silently resolve a conflict between the WFF paper, an amendment, repository wording, or a secondary source;
- net Pain against Pleasure or collapse intensity categories in primary outputs;
- create scalar or weighted primary WFF scores;
- store credentials, private data, funder-sensitive details, HR material, legal/board-sensitive material, or operational clutter;
- create Atlas, WFKG, connectors, schemas, validators, dashboards, product code, or other downstream infrastructure here;
- commit directly to `main`.

## Agent duties

Agents must:

- preserve fidelity to the WFF paper, formally adopted amendments, and approved internal canon;
- distinguish public-repository correction from substantive WFF revision;
- preserve terminology, module boundaries, analytical levels, and disaggregation safeguards;
- make assumptions and uncertainty explicit;
- identify the exact source and status of any proposed correction;
- record unresolved conflicts rather than choosing silently;
- route internal fidelity problems to the private canon workflow;
- route genuine amendment candidates to the joint scientific process;
- follow branch and review rules.

## Public corrections versus amendments

An ordinary public correction may:

- fix a typo, citation, broken link, or formatting problem;
- restore canonical terminology;
- reconcile the public mirror with the internal canon;
- correct a departure from the WFF paper or approved amendment;
- improve provenance, status, clarity, or machine readability;
- reflect a previously approved amendment after internal implementation.

A public correction may not independently:

- create or redefine a WFF concept;
- change the analytical chain;
- change module architecture;
- redefine intensity categories;
- introduce a new aggregation or weighting rule;
- revise foundational workflow.

Substantive WFF revision requires a controlled scientific record and joint approval by Wladimir and Cynthia. If they do not agree, the proposal remains unresolved.

## Placeholder markers

| Marker | Meaning |
|---|---|
| `[PLACEHOLDER — requires scientific review]` | Content not yet authored; do not fill without proper approval |
| `[OPEN QUESTION]` | Unresolved; do not treat as settled |
| `[DEPRECATED]` | Superseded term or representation |
| `[DRAFT]` | Drafted but not approved |

## Branching

- `main` — stable reviewed public representation
- `draft/<topic>` — work in progress
- `review/<topic>` — formal review
- `docs/<topic>` — documentation/governance
- `fix/<topic>` — fidelity or technical correction

Never push directly to `main`.

## Source rules

- Cite the primary WFF paper as the controlling scientific source.
- Treat secondary sources as evidence or operational clarification, not automatic authority over the WFF paper.
- If a secondary source conflicts with the paper or a formal amendment, record the conflict and stop.
- Determine whether the problem is a public fidelity error, internal canon fidelity error, interpretation issue, or amendment candidate.
- Correct public fidelity errors through the public workflow.
- Route internal fidelity errors to the private canon.
- Route amendment candidates to the joint scientific process.

## If uncertain

Create a review note describing:

- the relevant file and passage;
- the controlling scientific source;
- the apparent conflict or ambiguity;
- whether it appears to be a public fidelity correction, an internal canon issue, or a possible amendment question.

Then stop. Do not guess, fill placeholders, synthesize new canon, or infer joint approval.
