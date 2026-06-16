# Source Conflicts

This file records conflicts between source documents listed in
`sources/source_registry.yaml` and existing canon wording.

Entries here are **not** resolved automatically. Each requires explicit
review and approval by Wladimir J. Alonso or Cynthia Schuck-Paim before
any canon file is updated.

Do not edit canon files to resolve a conflict logged here without a
reviewed PR and explicit human approval.

---

## Format for entries

Each entry should record:
- **Conflict ID** (e.g. SC-001)
- **Date logged**
- **Source(s) in conflict** (use source IDs from `sources/source_registry.yaml`)
- **Canon file(s) affected**
- **Description of conflict**
- **Status** (open | under-review | resolved)
- **Resolution** (if resolved: brief description and commit reference)

---

## Known terminology conflicts (pre-logged)

### SC-001 — "Aggregation and Standardization" vs "Econometric Calculation"

- **Date logged:** 2026-05-12 (revised 2026-05-14)
- **Sources:** none in active conflict with current canon
- **Canon files affected:** `modules/v_econometric_calculation.md`,
  `glossary/deprecated_terms.yaml`
- **Description:** Early repository scaffolding (Phase 1.1) provisionally used
  "Aggregation and Standardization" as a descriptive working name for Module V.
  On re-reading the updated primary WFF methodological source
  (`wff-methodological-foundations-2025`) and the updated Technical Definitions
  source (`wfi-technical-definitions`), both dated 2026-05-14, both use
  "Econometric Calculation" exclusively. The repository term has been realigned
  with the canonical source terminology.
- **Status:** resolved
- **Resolution:** "Econometric Calculation" is the current Module V term in this
  repository, aligned with both registered methodological sources.
  "Aggregation and Standardization" is recorded as deprecated in
  `glossary/deprecated_terms.yaml` and should not be used in new canon or
  documentation. No registered source is in conflict with current canon on
  Module V terminology. No further action required unless a future registered
  source introduces a different term.

---

## Open conflicts

*No open conflicts.*

Add new entries above this line as conflicts are identified.

---

## Resolved conflicts

### SC-002 — Circumstance: internal/genetic conditions included vs. external-only

- **Date logged:** 2026-05-12
- **Sources:** `wfi-technical-definitions`, `wff-methodological-foundations-2025`
- **Canon files affected:** `canon/terminology.md`, `glossary/wff_terms.yaml`
- **Description:** The Technical Definitions source defines Circumstance as
  "internal and external conditions — physical, social, environmental, genetic,
  and procedural" and explicitly includes "inherited traits such as breed or
  genotype" as examples. The Phase 1.1 canon skeleton defined Circumstances as
  "the physical, social, and management conditions in which an animal lives,"
  implying exclusively external and management-related factors, with no mention
  of genetic or internal conditions. The source definition is substantively broader
  and includes a class of factors (genetic predispositions, breed) absent from the
  prior canon entry.
- **Status:** resolved
- **Resolution:** Resolved in favor of the corrected primary WFF methodological
  source and the Technical Definitions source. Circumstances include internal and
  external conditions that shape animal lives, including physical, social,
  environmental, genetic, and procedural factors. The canon clarifies that
  Circumstances must not be conflated with Biological Consequences, which are
  organism-level changes arising from Circumstances or prior Affective Experiences.
  Genetic background, breed, line, genotype, sex, age, or developmental status may
  be recorded in Module I when they shape vulnerability, exposure, or the
  interpretation of Circumstances. Commit references: b880335, 70b0d04
