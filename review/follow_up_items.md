# Follow-up Items

This file tracks **non-open-question** items: empirical research directions,
documentation cleanups, and future engineering or machine-readable canon
tasks that do not belong in `review/open_questions.md`.

Items here are not scientific or methodological uncertainties about the
framework itself. They are deferred work items whose underlying methodology
is either already settled (see `review/resolved_methodological_decisions.md`)
or non-scientific in nature (engineering, design, documentation).

> **Note for public readers:** Follow-up items are review-tracked development
> notes, not settled canon. Canonical methodology lives in `canon/` and
> `modules/`; this file only records deferred or supporting work.

**Status:** active — append items as they are identified; remove when
completed or transferred to canon/glossary/tools repositories
**Last reviewed:** 2026-05-16
**Active reviewer:** Wladimir J. Alonso
**Review record:** Tracked through the WFI canon review workflow

## Companion files

- `review/open_questions.md` — active unresolved scientific or methodological questions
- `review/resolved_methodological_decisions.md` — explicitly resolved methodological positions

## Entry format

Each entry follows this structure:

- **ID** — `FU-NNN`
- **Title** — short noun phrase
- **Type** — one of `empirical_research_direction`, `documentation_cleanup`,
  `future_engineering_task`, `deferred_glossary_work`
- **Description** — what the follow-up is
- **Why deferred** — why this is not an open scientific question
- **Affected files** — files that will eventually be touched
- **Suggested next step** — concrete next action when the item is picked up
- **Related decisions / questions** — relevant `RD-NNN` or `OQ-NNN` references
- **Date recorded** — when the item was logged

---

## Empirical research directions

### FU-001: Non-mammalian Pain evidence sufficiency

- **ID:** FU-001
- **Title:** Species-specific evidence streams for non-mammalian Pain intensity assignment
- **Type:** `empirical_research_direction`
- **Description:** Research direction — identify which species-specific
  behavioural, physiological, neurological, pharmacological, ecological,
  and functional evidence streams are sufficient to assign WFF Pain
  intensity categories (Annoying, Hurtful, Disabling, Excruciating) in
  fish, crustaceans, insects, and other non-mammalian taxa with adequate
  confidence.
- **Why deferred:** This is **not** a question about whether the WFF Pain
  intensity categories apply to non-mammalian taxa — that is resolved by
  `RD-003` (definitions are not species-specific; evidential application
  is species-specific; interspecific comparison requires Module Ψ
  assumptions). The remaining work is empirical evidence development,
  not framework-level uncertainty.
- **Affected files:**
  - `canon/intensity_categories_pain.md`
  - `modules/iii_affective_quantification.md`
  - `modules/psi_interspecific_scaling.md`
- **Suggested next step:** Commission a taxon-by-taxon evidence-stream
  review, starting with taxa where negative-affect evidence is most
  developed (fish, decapods). Produce species-conditional evidence-sufficiency
  notes rather than altering the canonical category definitions.
- **Related decisions / questions:** `RD-003`; was former `OQ-003` in `open_questions.md`
- **Date recorded:** 2026-05-16

### FU-002: Non-mammalian Pleasure operationalisation

- **ID:** FU-002
- **Title:** Species-specific evidence streams for non-mammalian Pleasure intensity assignment
- **Type:** `empirical_research_direction`
- **Description:** Research direction — develop species-specific evidence
  streams for assigning Satisfaction, Joy, Euphoria, and Bliss in birds,
  fish, cephalopods, decapods, and other plausibly sentient non-mammalian
  taxa. The four active WFF Pleasure intensity categories are operationally
  defined from a primary source whose behavioural, contextual, and
  physiological descriptors are predominantly informed by mammalian evidence;
  the parallel descriptors for non-mammalian taxa require dedicated work.
- **Why deferred:** The identity of the Pleasure intensity categories is
  settled (`RD-001`). The applicability principle parallels `RD-003` for
  Pain: definitions are not species-specific; evidential application is.
  The remaining work is empirical descriptor development per taxon, not
  framework-level uncertainty.
- **Affected files:**
  - `canon/intensity_categories_pleasure.md` (§12.1)
  - `modules/iii_affective_quantification.md`
  - `modules/psi_interspecific_scaling.md`
- **Suggested next step:** Commission a taxon-by-taxon descriptor review,
  starting with taxa for which positive-affect evidence is most developed
  (birds, fish). Produce species-conditional descriptor notes rather than
  altering the canonical category definitions.
- **Related decisions / questions:** `RD-001`, `RD-003`; was former `OQ-005`
  in `open_questions.md`
- **Date recorded:** 2026-05-16

### FU-003: Body-integrity-threatening behaviour exemplars for Excruciating Pain in non-human animals

- **ID:** FU-003
- **Title:** Species-specific exemplars of body-integrity-threatening behaviours
- **Type:** `empirical_research_direction`
- **Description:** The Excruciating Pain category includes, among its
  source-derived analytical criteria, the manifestation of behaviours an
  individual would strongly refrain from displaying under normal
  circumstances because they threaten body integrity (e.g., running into
  hazardous areas, exposing oneself to predators). This criterion is
  well-defined for humans but requires species-specific exemplars in other
  taxa, drawn from ethological literature, not assumed by analogy from
  human pain behaviour.
- **Why deferred:** This is a species-specific operationalisation task,
  not a framework-level methodological uncertainty. The criterion itself
  is settled in `canon/intensity_categories_pain.md`; what remains is
  empirical exemplar development per taxon.
- **Affected files:**
  - `canon/intensity_categories_pain.md` (§8, §12.2)
  - `modules/iii_affective_quantification.md`
- **Suggested next step:** Develop species-specific exemplars of
  body-integrity-threatening behaviours alongside the Module Ψ
  interspecific framework. Draw on ethological literature for each taxon
  rather than analogising from human pain behaviour.
- **Related decisions / questions:** was former `OQ-006` in `open_questions.md`
- **Date recorded:** 2026-05-16

---

## Documentation / canon cleanup follow-ups

### FU-006: Source attribution for No Pain and No Pleasure

- **ID:** FU-006
- **Title:** Source attribution and canon placement for "No Pain" and "No Pleasure"
- **Type:** `documentation_cleanup`
- **Description:** The "No Pain" category in `canon/intensity_categories_pain.md`
  is derived from `canon/terminology.md` and the methodological foundations
  source (`wff-methodological-foundations-2025`); the source registered
  for Pain intensities (`wfi-pain-intensities`) defines only the four
  active categories. The "No Pleasure" category in
  `canon/intensity_categories_pleasure.md` is, by contrast, explicitly
  introduced by its primary source (`wfi-positive-welfare-2024`). The
  current state is internally consistent (each file attributes its "No"
  category honestly), but the asymmetry may confuse downstream readers.
- **Why deferred:** This is not a scientific open question — the definitions
  of No Pain and No Pleasure are not uncertain. It is a documentation
  cleanup item about how the asymmetric source attribution is presented.
- **Affected files:**
  - `canon/intensity_categories_pain.md` (§4)
  - `canon/intensity_categories_pleasure.md` (§4)
  - `sources/source_registry.yaml`
- **Suggested next step:** Either (a) accept the asymmetry as documented
  and add a short cross-reference note in each file's §4; or (b) extend
  the Pain intensity source documentation (separate PR with explicit
  approval) to cover No Pain.
- **Related decisions / questions:** was former `OQ-013` in `open_questions.md`
- **Date recorded:** 2026-05-16

---

## Future engineering or machine-readable canon tasks

### FU-004: Color-code registry / visualization-conventions YAML

- **ID:** FU-004
- **Title:** Formal integration of canonical visualization color codes
- **Type:** `future_engineering_task`
- **Status:** Implemented
- **Implemented at:** `visualization/intensity_colors.yaml`
- **Description:** Canonical WFF visualization color codes for Pain and
  Pleasure intensity categories are defined inline in the respective
  canon files. Their formal integration into a machine-readable canon
  artifact — referenced by downstream WFF tools, the Welfare Footprint
  Atlas, and any future agent consumers — is now implemented as
  `visualization/intensity_colors.yaml`, a derived machine-readable
  mirror, with `canon/visualization_conventions.md` documenting the
  conventions. Canon prose remains authoritative per `RD-005`.
- **Why deferred:** This is not a scientific open question. It is an
  engineering / machine-readable canon task. The Phase 1 canon ↔ glossary
  contract (`RD-005`) means canon prose is authoritative during Phase 1;
  any machine-readable conventions resource must conform to that contract
  when it is added.
- **Affected files:**
  - `canon/intensity_categories_pain.md` (§11, §12.3)
  - `canon/intensity_categories_pleasure.md` (§11, §12.4)
  - `visualization/intensity_colors.yaml` (machine-readable palette)
  - `canon/visualization_conventions.md` (conventions document)
- **Resolution:** Implemented via the visualization color-palette change,
  which added `visualization/intensity_colors.yaml` (a derived
  machine-readable mirror) and `canon/visualization_conventions.md` (the
  conventions document), with canon prose remaining authoritative per
  `RD-005`. The earlier illustrative path `conventions/visualization.yaml`
  was not adopted; `visualization/intensity_colors.yaml` is the canonical
  location for the machine-readable palette.
- **Related decisions / questions:** `RD-005`; was former `OQ-010` in `open_questions.md`
- **Date recorded:** 2026-05-16

---

## Deferred glossary / visualization work

### FU-005: Symmetric per-category glossary entries for Pain and Pleasure

- **ID:** FU-005
- **Title:** Whether per-category glossary entries should be added
- **Type:** `deferred_glossary_work`
- **Description:** Whether `glossary/wff_terms.yaml` should gain per-category
  entries (`no_pain`, `annoying`, `hurtful`, `disabling`, `excruciating`,
  `no_pleasure`, `satisfaction`, `joy`, `euphoria`, `bliss`) is deferred.
  The existing `pain_intensity`, `cumulative_pain`, `pleasure_intensity`,
  and `cumulative_pleasure` entries reference the category sets
  collectively. This is a glossary/canon design choice, not a scientific
  uncertainty about the categories themselves (their identity is settled
  in `RD-001`).
- **Why deferred:** Not a scientific open question. Under `RD-005`, canon
  prose is the Phase 1 source of truth; glossary enrichment should not
  proceed until that contract is reflected in the relevant files and the
  generation/audit pattern is chosen.
- **Affected files:**
  - `glossary/wff_terms.yaml`
  - `canon/intensity_categories_pain.md` (§12.4)
  - `canon/intensity_categories_pleasure.md` (§12.5)
- **Suggested next step:** Defer per `RD-005`. When picked up, generate
  per-category glossary entries from canon prose rather than authoring
  them by hand, unless Wladimir explicitly decides the YAML should be
  authoritative.
- **Related decisions / questions:** `RD-001`, `RD-005`; was former `OQ-011`
  in `open_questions.md`
- **Date recorded:** 2026-05-16
