# WFI Scientific Canon

**Organization:** Welfare Footprint Institute
**Repository:** `welfare-footprint-institute/wfi-scientific-canon-public`
**Status:** Curated public mirror of the WFI scientific canon

> **Curated public mirror.** This repository is a curated public mirror of the Welfare Footprint Institute scientific canon, maintained separately from the WFI internal working repository. Some files are marked as draft, provisional, deprecated, or open questions. These markers are part of the canon-governance process and should not be interpreted as settled methodology. The current primary methodological citation is the OSF preprint listed in `sources/citation_policy.md`.

---

## Purpose

This repository is a curated public mirror of the version-controlled scientific
canon of the Welfare Footprint Institute (WFI). It holds the authoritative or review-tracked definitions, methodological
commitments, module specifications, and terminology that underpin all WFI
quantitative welfare work. Some entries remain draft, provisional, or pending
scientific review.

It is a **reference archive**, not a software product. Changes to canonical
content require explicit human scientific review.

---

## Scope and relationship to other WFI repositories

This repository is intended to hold the **public WFF scientific canon**:
methodology, terminology, module specifications, evidence standards, and the
source registry.

- This is **not** the Welfare Footprint Atlas implementation repository.
- Downstream WFI tools — Atlas, Processograms, Hedonic-Track GPT, AffectMap GPT,
  Zootechnical Mapper GPT, Interspecific Affect GPT, and others — may **cite or
  consume** the canon, but they are developed in separate repositories.
- Schemas, validators, MCP servers, dashboards, product code, content studio,
  ops infrastructure, and internal strategy material do **not** belong here.

This public mirror is maintained separately from the WFI internal working
repository, which has its own development history and scientific review
workflow. This mirror may lag behind internal development and should be treated
as the current public teaching and reference snapshot of the canon.

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

These four levels are **distinct and must not be conflated**.
Welfare assessment centres on **Affective Experiences**.

---

## Repository Structure

```
wfi-scientific-canon-public/
├── canon/          Core principles, terminology, intensity scales, evidence standards
├── modules/        WFF module specifications (I–VI + Ψ)
├── sources/        Source registry and citation policy
├── glossary/       Term definitions, deprecated terms, change log
├── examples/       Failure modes, boundary examples, terminology examples
├── visualization/  Machine-readable canonical intensity color palette
└── review/         Open questions, unresolved issues, source conflicts, external review notes
```

---

## WFF Modules

| Module | Name |
|--------|------|
| I      | Zootechnical Description |
| II     | Veterinary Inventory |
| III    | Affective Quantification |
| IV     | Epidemiological Review |
| V      | Econometric Calculation |
| VI     | Welfare Footprints: Expression and Notation |
| Ψ      | Interspecific Scaling / Interspecific Affect |

> Module V was provisionally named "Aggregation and Standardization" in early
> repository scaffolding. That term is **deprecated**. The current term,
> "Econometric Calculation," aligns with the primary WFF methodological source
> and the Technical Definitions source. See `glossary/deprecated_terms.yaml`.

---

## Primary citation

> Alonso, W. J., & Schuck-Paim, C. (2025). *Welfare Footprint Framework:
> Methodological Foundations and Quantitative Assessment Guidelines.*
> Center for Welfare Metrics (São Paulo).
> https://doi.org/10.17605/osf.io/94bxs
>
> *(Under review at Animal Sentience. Cite the OSF preprint until the
> journal version is published. See `sources/citation_policy.md`.)*

---

## Contributing

- All changes to `canon/` and `modules/` require explicit human approval.
- Use `draft/<topic>` branches for work in progress.
- Use `review/<topic>` branches for content under peer review.
- Do not treat placeholders or open questions as settled canon.
- If uncertain, open a review note in `review/` rather than editing canon directly.
- Source documents do not automatically become canon — all canon updates
  require reviewed PRs. See `sources/citation_policy.md`.

See [`CONTRIBUTING.md`](CONTRIBUTING.md) for contribution scope and review
requirements, [`LICENSE.md`](LICENSE.md) for licensing (CC BY 4.0 for the
textual canon), and [`CITATION.cff`](CITATION.cff) for how to cite this work.

---

## What WFI Does and Does Not Do

WFI provides:
- Evidence summaries tied to scientific sources
- Transparent, quantitative welfare metrics
- Structured comparisons across species and conditions
- Explicit assumptions and uncertainty estimates

WFI does **not** issue institutional moral verdicts.

---

## Maintainers

- Wladimir J. Alonso
- Cynthia Schuck-Paim
- Additional maintainers to be added through CODEOWNERS
