# Open Questions

This file contains **only active unresolved scientific or methodological
questions** within the WFF. Entries here represent real framework-level
uncertainty whose resolution requires explicit scientific review.

**Empirical research directions and engineering/design follow-ups are
tracked in `review/follow_up_items.md`.**
**Resolved decisions are tracked in `review/resolved_methodological_decisions.md`.**

**Status:** active — add and track entries; do not close without human approval
**Last reviewed:** 2026-05-16
**Active reviewer:** Wladimir J. Alonso
**Additional review:** To be scheduled

---

## Companion files

- `review/resolved_methodological_decisions.md` — explicitly resolved methodological positions (`RD-NNN`)
- `review/follow_up_items.md` — empirical research directions, documentation cleanups, engineering and design tasks (`FU-NNN`)

## Scope and classification rule

Only **genuinely unresolved scientific or methodological questions** belong
in this file. Before adding an item, classify it as one of:

- `active_open_question` — a genuinely unresolved scientific or methodological
  question whose resolution is not yet settled in WFF canon. **Belongs in this file.**
- `resolved_methodological_decision` — record in
  `review/resolved_methodological_decisions.md`, not here.
- `implementation_standard` — record as a resolved decision and track the
  implementation update separately; do not record as an open question.
- `empirical_limitation_or_research_direction` — record in
  `review/follow_up_items.md`, not here.
- `future_engineering_task` — record in `review/follow_up_items.md`, not here.
- `documentation_cleanup` — record in `review/follow_up_items.md`, not here.
- `deferred_glossary_work` — record in `review/follow_up_items.md`, not here.

Do not use this file as a place to store content gaps, source limitations,
review leftovers, implementation tasks, or research directions.

## Closure rule

Do not close or remove entries silently. An item may be closed only by:

1. an explicit methodological decision recorded in
   `review/resolved_methodological_decisions.md`,
2. incorporation into canon via an approved PR with a clear resolution note, or
3. transfer to `review/resolved_methodological_decisions.md` or
   `review/follow_up_items.md` with a clear pointer from any canon section
   that previously cited the open question.

Resolution of an `active_open_question` requires explicit scientific review
and approval by Wladimir J. Alonso (additional review to be scheduled).

## Entry format

- **ID** — `OQ-NNN`
- **Title** — short noun phrase
- **Status** — `active_open_question`
- **Affected files** — files where the question is reflected
- **Description** — what is unresolved
- **Why it matters** — framework-level consequence
- **Suggested next step** — concrete next action

---

## Migration log (2026-05-16)

The earlier broader open-question list has been split across three files
to keep this file restricted to genuinely active scientific or
methodological questions:

| Former ID | Disposition                                                                                    | Now recorded as |
|-----------|------------------------------------------------------------------------------------------------|-----------------|
| OQ-001    | Pleasure intensity category set — resolved                                                     | `RD-001`        |
| OQ-002    | Inter-individual variation — reclassified as pragmatic methodological position                 | `RD-002`        |
| OQ-003    | Non-mammalian Pain — framework question resolved; evidence-development item is empirical       | `RD-003` + `FU-001` |
| OQ-004    | Point vs. lifetime prevalence consistency — resolved by Wladimir's decision                    | `RD-004`        |
| OQ-005    | Non-mammalian Pleasure operationalisation — empirical research direction                       | `FU-002`        |
| OQ-006    | Body-integrity-threatening behaviour exemplars — species-specific operationalisation           | `FU-003`        |
| OQ-007    | Maladaptive Pleasure within the four-category scale — retained as active open question         | `OQ-007` (kept) |
| OQ-008    | Cross-valence equivalence at extremes — retained as active open question                       | `OQ-008` (kept) |
| OQ-009    | Concurrent Affective Experiences at segment level — retained as active open question           | `OQ-009` (kept) |
| OQ-010    | Color-code registry / visualization-conventions YAML — implemented at `visualization/intensity_colors.yaml` (see `FU-004`) | `FU-004`        |
| OQ-011    | Per-category glossary entries — deferred glossary work                                         | `FU-005`        |
| OQ-012    | Canon ↔ glossary source-of-truth contract — resolved for Phase 1                               | `RD-005`        |
| OQ-013    | Source attribution for No Pain / No Pleasure — documentation cleanup                           | `FU-006`        |

ID numbering for retained entries (`OQ-007`, `OQ-008`, `OQ-009`) is
preserved unchanged so that cross-references in `RD-NNN`, `FU-NNN`, and
any future canon/module text remain stable. Gaps in numbering are
intentional and reflect the migration above.

---

## OQ-007: Maladaptive Pleasure

- **ID:** OQ-007
- **Title:** Maladaptive Pleasure within the four-category scale
- **Status:** `active_open_question`
- **Affected files:**
  - `canon/intensity_categories_pleasure.md` (§2.9, §12.2)
- **Description:** The primary source for Pleasure intensity
  (`wfi-positive-welfare-2024`) explicitly notes that high engagement with
  positive experiences can occur in cases that admit maladaptive exceptions —
  addiction in humans and feather-plucking in birds are cited examples. How
  such states are to be classified within the canonical four-category
  Pleasure scale (`RD-001`), and whether they warrant any analytical
  annotation distinct from the intensity assignment itself, is not resolved.
- **Why it matters:** A naive reading of the engagement axis could assign
  high Pleasure intensities to states that drive welfare-degrading or
  self-damaging behaviour, with no separate flag indicating the adverse
  context. This is a methodological hazard for both individual-level and
  population-level Pleasure assessments.
- **Suggested next step:** Defer to a future reviewed PR with explicit
  Wladimir approval (additional review to be scheduled). Likely outcomes
  include either (a) an annotation pattern (e.g., "high engagement,
  maladaptive context") that preserves the intensity classification while
  flagging context, or (b) a paired Pain-side accounting that captures the
  welfare cost. Do not operationalise inside the per-category Pleasure
  definitions in the meantime.

---

## OQ-008: Cross-valence equivalence (Bliss vs Excruciating, and analogues)

- **ID:** OQ-008
- **Title:** Cross-valence equivalence of duration at extremes
- **Status:** `active_open_question` (framework-level)
- **Affected files:**
  - `canon/intensity_categories_pleasure.md` (§10.4, §12.3)
  - `canon/intensity_categories_pain.md` (§2.7)
- **Description:** The primary source for Pleasure intensity raises, as an
  explicit open question, whether (for example) ten seconds of Bliss can be
  considered a direct counterpart of ten seconds of Excruciating Pain. The
  WFF canon currently treats Pain and Pleasure as valence-specific scales
  that are not netted and not equated, and explicitly does not assert any
  such cross-valence equivalence.
- **Scope note:** This question is relevant only to **hypothetical future
  scalar aggregation or cross-valence equivalence assumptions**. It is
  **not** a blocker for the current WFF practice of keeping Cumulative
  Pain and Cumulative Pleasure disaggregated and non-netted. The default
  WFF position remains that no cross-valence equivalence is assumed.
- **Why it matters:** This is the most consequential open question for any
  future analytical layer that would attempt scalar aggregation across
  valences (e.g., a single welfare scalar combining time in Pain and time
  in Pleasure). Premature resolution would commit the framework to an
  empirically unjustified equivalence. Indefinite deferral leaves
  cross-valence comparison without a principled treatment.
- **Suggested next step:** Treat as a framework-level methodological
  question requiring a dedicated review process (potentially with external
  philosophical and welfare-science input). Do not address inside intensity
  category canon files.

---

## OQ-009: Concurrent Affective Experiences at segment level

- **ID:** OQ-009
- **Title:** Interaction of concurrent Affective Experiences at the segment level
- **Status:** `active_open_question`
- **Affected files:**
  - `canon/intensity_categories_pain.md` (§12.5)
  - `canon/intensity_categories_pleasure.md` (§12.6)
  - `modules/iii_affective_quantification.md`
- **Description:** Attention-related effects of concurrent negative and
  positive Affective Experiences at different intensities are addressed at
  the metric level (Cumulative Affect [Attention-Adjusted]). How they should
  interact with intensity classification at the segment level — for example,
  whether the presence of concurrent Pain reduces the inferred Pleasure
  intensity assigned to a segment, or vice versa — remains open.
- **Why it matters:** Real welfare contexts routinely involve concurrent
  positive and negative affect. A clear segment-level rule (or an explicit
  decision not to apply one) is needed for consistent Pain-Track and
  Pleasure-Track construction.
- **Suggested next step:** Defer until at least one worked example with
  concurrent affect is documented; treat as a Module III methodological
  decision rather than an intensity-category decision.

---

## [PLACEHOLDER]

Additional open questions to be added as assessments progress and as
the scientific review process identifies new unresolved issues. Only
items classified as `active_open_question` should be added here;
research directions, documentation cleanups, and engineering tasks
belong in `review/follow_up_items.md`.
