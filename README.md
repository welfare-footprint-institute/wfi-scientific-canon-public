# WFI Scientific Canon

**Organization:** Welfare Footprint Institute
**Repository:** `welfare-footprint-institute/wfi-scientific-canon-public`
**Status:** Curated public mirror of the WFI scientific canon

> **Authority hierarchy.** The ultimate current scientific authority for the Welfare Footprint Framework is the primary WFF methodological paper, together with any formal amendment or addendum jointly approved by Wladimir J. Alonso and Cynthia Schuck-Paim. The private scientific canon is the controlled, versioned operational representation of those scientific sources. This public repository is a curated mirror of that internal representation. Neither repository independently creates or revises WFF scientific authority. See `sources/wff_scientific_authority.md` and `sources/citation_policy.md`.

---

## Purpose

This repository is the curated public teaching, citation, review, and retrieval representation of the WFI scientific canon. It presents established WFF terminology, methodological commitments, module descriptions, source relationships, status, and review records for public human and machine use.

Some files are marked as draft, provisional, deprecated, or open questions. These markers are part of repository governance and should not be interpreted as settled WFF methodology.

It is a **reference archive**, not a software product. Routine public contributions should correct errors, improve clarity and provenance, and ensure faithful representation of the WFF paper, formally adopted amendments, and approved internal canon.

Substantive proposals to revise the framework's underlying concepts or methodological architecture are exceptional. They require a separate higher-level scientific process, formal scientific documentation, and joint approval by Wladimir and Cynthia. Neither author acting alone may unilaterally alter the foundational scientific content of the WFF. Only after such an approved change is represented in the internal canon should this public mirror be updated.

---

## Scope and relationship to other WFI repositories

This repository holds the **public mirror of the WFF scientific canon**: methodology, terminology, module specifications, evidence standards, source governance, and selected review records.

- The primary WFF paper and formally adopted amendments remain scientifically superior to both the private and public canon repositories.
- The private repository has its own development history and review workflow and is the immediate source for this mirror.
- This mirror may lag internal development and should be treated as the current public teaching and reference snapshot.
- This is not the Welfare Footprint Atlas implementation repository.
- Downstream WFI tools — Atlas, Processograms, Custom GPTs, WFKG, and others — may cite or consume this repository, but they are developed separately.
- Schemas, validators, MCP servers, dashboards, product code, content studio, operations infrastructure, and internal strategy material do not belong here.

---

## The WFF Chain

All WFI welfare assessments follow this causal chain:

```
Circumstances
    ↓
Biological Consequences
    ↓
Affective Experiences
    ↓
Welfare Metrics
```

These four levels are distinct and must not be conflated. Welfare assessment centres on Affective Experiences.

---

## Repository Structure

```
wfi-scientific-canon-public/
├── canon/          Core principles, terminology, intensity scales, evidence standards
├── modules/        WFF module specifications (I–VI + Ψ)
├── sources/        Source registry, citation policy, and authority hierarchy
├── glossary/       Term definitions, deprecated terms, change log
├── examples/       Failure modes, boundary examples, terminology examples
├── visualization/  Machine-readable canonical intensity colour palette
└── review/         Open questions, unresolved issues, source conflicts, external review notes
```

---

## WFF Modules

| Module | Name |
|--------|------|
| I | Zootechnical Description |
| II | Veterinary Inventory |
| III | Affective Quantification |
| IV | Epidemiological Review |
| V | Econometric Calculation |
| VI | Welfare Footprints: Expression and Notation |
| Ψ | Interspecific Scaling / Interspecific Affect |

> Module V was provisionally named "Aggregation and Standardization" in early repository scaffolding. That term is deprecated. The current term, "Econometric Calculation," aligns with the primary WFF methodological source and the Technical Definitions source. See `glossary/deprecated_terms.yaml`.

---

## Primary citation

> Alonso, W. J., & Schuck-Paim, C. (2025). *Welfare Footprint Framework: Methodological Foundations and Quantitative Assessment Guidelines.* Center for Welfare Metrics (São Paulo). https://doi.org/10.17605/osf.io/94bxs
>
> *(Under review at Animal Sentience. Cite the OSF preprint until the journal version is published.)*

See `sources/citation_policy.md` and `sources/wff_scientific_authority.md`.

---

## Contributing

- Ordinary contributions should correct errors, ambiguity, provenance problems, or departures from the WFF paper, approved amendments, and internal canon.
- Changes to `canon/` and `modules/` require explicit review for fidelity to those scientific sources.
- Substantive proposals to change WFF concepts, the analytical chain, module architecture, intensity definitions, or methodological workflow require a separate higher-level scientific process and joint approval by Wladimir and Cynthia.
- An Issue or ordinary Pull Request does not itself amend the WFF.
- Use `draft/<topic>` branches for work in progress and `review/<topic>` branches for formal review.
- Do not treat placeholders or open questions as settled methodology.
- Source documents do not automatically become WFF authority.

See [`CONTRIBUTING.md`](CONTRIBUTING.md) for the full distinction between public-repository corrections and substantive WFF revision.

---

## What WFI Does and Does Not Do

WFI provides:
- evidence summaries tied to scientific sources;
- transparent, quantitative welfare metrics;
- structured comparisons across species and conditions;
- explicit assumptions and uncertainty estimates.

WFI does not issue institutional moral verdicts.

---

## Maintainers

- Wladimir J. Alonso
- Cynthia Schuck-Paim
- Additional technical maintainers may be added through CODEOWNERS, but technical repository access does not confer authority to revise the WFF.
