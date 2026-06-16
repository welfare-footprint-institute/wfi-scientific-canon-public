# Resolved Methodological Decisions

This file records WFF methodological questions that have been **explicitly
resolved**, so they are not repeatedly reintroduced as open questions.

Entries here are settled in current WFF canon or by explicit methodological
decision. They are not placeholders for future content and they are not
candidates for `review/open_questions.md`.

**Status:** active — append new resolved decisions as they are finalised;
do not silently reopen entries
**Last reviewed:** 2026-05-16
**Active reviewer:** Wladimir J. Alonso
**Review record:** Tracked through the WFI canon review workflow

---

## Entry format

Each entry follows this structure:

- **ID** — `RD-NNN`
- **Title** — short noun phrase
- **Decision** — the resolved methodological position
- **Implication** — what this means for future canon work and assessments
- **Canonical files** — files where the decision is reflected (existing or future)
- **Source basis** — registered sources or explicit decision authority
- **Date recorded** — when the decision was logged in this file

---

## RD-001: Pleasure intensity category set

- **ID:** RD-001
- **Title:** Pleasure intensity category set
- **Decision:** The WFF Pleasure intensity categories are
  **No Pleasure, Satisfaction, Joy, Euphoria, and Bliss**. No Pleasure is
  the zero / absence-of-Pleasure state and does not contribute to Cumulative
  Pleasure totals. The active positive categories are
  **Satisfaction → Joy → Euphoria → Bliss**.
- **Implication:** Do not list the identity of the Pleasure intensity
  categories as an open question. Future work may refine operational
  descriptors, species-specific application, or glossary representation,
  but the category names and ordering are settled in current canon.
- **Canonical files:**
  - `canon/intensity_categories_pleasure.md`
  - `canon/terminology.md`
- **Source basis:**
  - `wfi-positive-welfare-2024`
  - `wff-methodological-foundations-2025`
  - `wfi-technical-definitions`
- **Supersedes:** former `OQ-001` in `review/open_questions.md`
- **Date recorded:** 2026-05-16

---

## RD-002: Pragmatic treatment of inter-individual variation

- **ID:** RD-002
- **Title:** Pragmatic treatment of inter-individual variation
- **Decision:** The WFF acknowledges natural variation and epistemic
  uncertainty, but it does **not** require full individual-level modelling
  as a default implementation burden. When evidence supports variation in
  intensity or duration, estimates should be represented through probability
  distributions across intensity categories, ranges for duration, or
  sensitivity analysis. When such evidence is sparse, assumptions and
  uncertainty should be stated explicitly rather than requiring infeasible
  individual-level modelling.
- **Implication:** Do not treat lack of formal individual-level modelling
  as a blocker for WFF implementation. Future research may improve
  representation of individual variation, but routine assessments may
  proceed with explicit uncertainty ranges and evidence-based probability
  distributions.
- **Canonical files:**
  - `canon/terminology.md`
  - `canon/intensity_categories_pain.md`
  - `canon/intensity_categories_pleasure.md`
- **Source basis:**
  - `wff-methodological-foundations-2025`
  - `wfi-technical-definitions`
- **Supersedes:** former `OQ-002` in `review/open_questions.md`
- **Date recorded:** 2026-05-16

---

## RD-003: Species-internal use of WFF intensity categories

- **ID:** RD-003
- **Title:** Species-internal use of WFF intensity categories
- **Decision:** The WFF Pain intensity categories are **not species-specific
  in their definitions**. They can be used for fish, crustaceans, insects,
  and other plausibly sentient taxa as operational hypotheses about negative
  affective intensity. However, assigning an episode to Annoying, Hurtful,
  Disabling, or Excruciating requires species-specific calibration against
  behavioural, physiological, neurological, pharmacological, ecological,
  and functional evidence. Direct cross-species comparison requires explicit
  **Module Ψ / Interspecific Scaling** assumptions.
- **Implication:** Do not frame the question "do the categories apply to
  non-mammalian taxa?" as unresolved. The correct distinction is:
  - definitions are shared;
  - evidential application is species-specific;
  - interspecific comparison requires explicit scaling assumptions.

  A narrower, genuinely open evidence-development question — which
  species-specific evidence streams are sufficient to assign Pain intensity
  categories in non-mammalian taxa — is retained as `OQ-003` in
  `review/open_questions.md`.
- **Canonical files:**
  - `canon/intensity_categories_pain.md`
  - `canon/terminology.md`
  - `modules/psi_interspecific_scaling.md`
- **Source basis:**
  - `wff-methodological-foundations-2025`
  - `wfi-technical-definitions`
  - `wfi-pain-intensities`
- **Supersedes:** former framework-level reading of `OQ-003` in
  `review/open_questions.md` (narrow evidence-development question retained
  under the same ID)
- **Date recorded:** 2026-05-16

---

## RD-004: Harmonising prevalence types

- **ID:** RD-004
- **Title:** Harmonising prevalence types
- **Decision:** When prevalence estimates come from different prevalence
  types, they must be **harmonised before use**. Point prevalence, period
  prevalence, and lifetime prevalence are not interchangeable. Each estimate
  should be converted, where possible, to the prevalence type required by
  the analysis, usually period prevalence over the relevant Life-Phase or
  lifespan segment. If conversion is not possible, the estimates should not
  be pooled mechanically; they should be treated as separate evidence sources
  informing a range, with assumptions stated explicitly.
- **Implication:** Do not mechanically pool point, period, and lifetime
  prevalence estimates. Treat prevalence-type harmonisation as a Module IV
  implementation standard. This standard should later be incorporated into
  `modules/iv_epidemiological_review.md`.
- **Canonical files:**
  - `modules/iv_epidemiological_review.md` *(future update needed)*
  - `canon/terminology.md`
- **Source basis:**
  - Wladimir J. Alonso, methodological decision (2026-05-16)
  - `wff-methodological-foundations-2025`
  - `wfi-technical-definitions`
- **Supersedes:** former `OQ-004` in `review/open_questions.md`
- **Date recorded:** 2026-05-16

---

## RD-005: Phase 1 canon ↔ glossary source-of-truth contract

- **ID:** RD-005
- **Title:** Phase 1 canon ↔ glossary source-of-truth contract
- **Decision:** During Phase 1, **human-readable canon prose is authoritative**.
  Machine-readable files such as `glossary/wff_terms.yaml` are companion
  artifacts derived from and constrained by the canon prose. They may
  support agents and future tooling, but they do not override the prose
  canon. A future reviewed schema phase may promote selected machine-readable
  files to canonical status once their structure, validation rules, and
  governance are explicitly defined.
- **Implication:** Do not treat mismatches between canon prose and glossary
  YAML as two equally authoritative sources. If they conflict during
  Phase 1, revise the YAML or companion artifact to align with the
  human-readable canon, unless Wladimir explicitly decides otherwise.
  Glossary enrichment and validation should not proceed until this contract
  is reflected in the relevant files.
- **Canonical files:**
  - `canon/terminology.md`
  - `glossary/wff_terms.yaml`
  - `README_FOR_AGENTS.md` *(future update may be needed)*
- **Source basis:**
  - Wladimir J. Alonso, methodological / repository-governance decision (2026-05-16)
- **Supersedes:** former `OQ-012` in `review/open_questions.md`
- **Date recorded:** 2026-05-16
