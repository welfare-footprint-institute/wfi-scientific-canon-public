# Module III: Affective Quantification

**Status:** Scaffold for scientific review
**Review status:** Pending formal WFI scientific review
**Review record:** Tracked through the WFI canon review workflow

---

## Purpose

Quantify the **Affective Experiences** — both negative (Pain, distress, fear,
frustration) and positive (Pleasure, comfort, positive engagement) — that arise
from the Biological Consequences identified in Module II.

Module III is the step at which welfare assessment becomes affective: this is
where the WFF chain makes contact with the morally relevant quantity.

`Circumstances → Biological Consequences → Affective Experiences → Welfare Metrics`

Module III produces structured temporal hypotheses — Pain-Tracks and
Pleasure-Tracks — that translate each identified Biological Consequence into an
episode-level welfare estimate for an affected individual.

---

## Core entities

> Authoritative WFF definitions and resolved methodological decisions are
> maintained in `canon/`, `glossary/`, the relevant canon files, and
> `review/resolved_methodological_decisions.md`. This section identifies the
> entities used by this module and their module-specific role; it is not an
> independent glossary.

- **Affective Experience** — canonical WFF entity. **Module III role:**
  the unit of analysis quantified by this module; characterized here by
  valence, intensity, and temporal evolution.
- **Affective State** — canonical WFF entity. **Module III role:** the
  specific valence and intensity condition occupying a given temporal
  segment within an Affective Experience.
- **Valence** — canonical attribute. **Module III role:** negative vs.
  positive classification of each segment, tracked separately throughout.
- **Affective Experience type** — module-specific descriptor.
  **Module III role:** the specific kind of felt state, recorded separately
  from valence and intensity category. Examples: physical Pain, hunger,
  thirst, thermal discomfort, fear, frustration, boredom, comfort, positive
  social engagement, play-related Pleasure, satiety, relief.
- **Pain intensity category** — canonical WFF category set (definitions in
  `canon/intensity_categories_pain.md`). **Module III role:** categorical
  assignment for each negative segment. Categories: No Pain, Annoying,
  Hurtful, Disabling, Excruciating (No Pain is an explicit track state).
  Active negative categories: Annoying → Hurtful → Disabling → Excruciating.
- **Pleasure intensity category** — canonical WFF category set, settled by
  RD-001 (definitions in `canon/intensity_categories_pleasure.md`).
  **Module III role:** categorical assignment for each positive segment. Categories:
  No Pleasure, Satisfaction, Joy, Euphoria, Bliss (No Pleasure is an
  explicit track state). Active positive categories: Satisfaction → Joy →
  Euphoria → Bliss.
- **Pain-Track** — Module III operational construct. Structured temporal
  representation of a negative Affective Experience, decomposed into
  segments each assigned an intensity category with a duration range and
  probability distribution.
- **Pleasure-Track** — Module III operational construct. Structured
  temporal representation of a positive Affective Experience, decomposed
  in the same manner.
- **Temporal segment** — Module III operational construct. A portion of
  an Affective Experience characterized by a relatively stable hypothesized
  intensity; boundaries reflect expected changes in the felt experience
  (e.g., treatment initiation, recovery stage, behavioural transition).
- **Segment duration range** — Module III operational construct. The
  estimated minimum and maximum duration of each temporal segment,
  reflecting biological variation and epistemic uncertainty.
- **Probability distribution across intensity categories** — Module III
  operational construct. For each segment, the estimated relative
  plausibility that the experience falls within each intensity category,
  reflecting uncertainty and individual variation.
- **Cumulative Pain [Episode]** — canonical WFF metric, episode-scope.
  **Module III role:** total estimated time in each Pain intensity category
  across all segments of the Affective Experience; disaggregated by
  intensity category.
- **Cumulative Pleasure [Episode]** — canonical WFF metric, episode-scope.
  **Module III role:** total estimated time in each Pleasure intensity
  category across all segments of the Affective Experience; disaggregated
  by intensity category.
- **Evidence-to-category justification** — Module III operational
  requirement. The explicit evidentiary reasoning linking available welfare
  indicators to the assigned intensity estimate.

---

## Inputs

- Module II output: Biological Consequences, candidate Affective Experiences,
  valence pathways, and pathway classifications for each Life-Fate and
  Life-Phase
- Affective science, pain science, and positive welfare literature
- Behavioural, physiological, neurological, and pharmacological evidence for
  affective state
- Species-specific evidence streams for intensity calibration
- Expert elicitation where empirical data are absent

---

## Outputs

For each Affective Experience arising from a Module II Biological Consequence:

- Affective Experience name and description
- Biological Consequence(s) from which it arises
- Valence classification
- Affective Experience type (e.g., physical Pain, fear, frustration, satiety)
- Pain-Track or Pleasure-Track
- Temporal segments with biologically or behaviourally justified boundaries
- Duration range for each segment
- Probability distribution across intensity categories for each segment
- Cumulative Pain [Episode] or Cumulative Pleasure [Episode], disaggregated
  by intensity category
- Evidence streams used for intensity and duration estimates
- Confidence level and uncertainty notes
- Flags for unresolved or contested calibrations

These outputs are paired with epidemiological parameters estimated in
Module IV — prevalence, occurrence, Affective Episode Rate, and relevant
denominators — and integrated in Module V (Econometric Calculation).
Module IV supplies the epidemiological parameters; Module V performs the
integration into population-, Life-Fate-, system-, or product-level
Welfare Footprint metrics.

---

## Required distinctions

- **Affective Experiences ≠ Biological Consequences.** The Pain caused by
  a footpad lesion is an Affective Experience; the lesion itself is a
  Biological Consequence. Maintain this distinction at all times.
- **Intensity ≠ Prevalence.** Intensity describes the severity of experience
  for an affected individual. Prevalence (Module IV) describes how many animals
  are affected. Do not conflate these axes.
- **Affective Experience type ≠ intensity category.** "Fear" names the kind
  of experience; "Hurtful" or "Disabling" names its intensity. Both must be
  recorded separately.
- **Pain and Pleasure are WFF umbrella operational terms.** More specific
  Affective Experience types (fear, frustration, satiety, comfort) should be
  recorded alongside valence and intensity category; do not flatten the full
  type description into just "Pain" or "Pleasure."
- **No Pain and No Pleasure are explicit track states.** They must be
  represented in temporal accounting so that segments without negative or
  positive affect are recorded rather than left implicit.
- **Valence and intensity-category disaggregation must be preserved.**
  Negative and positive Affective Experiences are tracked separately as
  Cumulative Pain and Cumulative Pleasure. Cumulative Pain and Cumulative
  Pleasure remain disaggregated by their respective intensity categories.
  Module III does not combine Pain and Pleasure, and Module V must not present
  such combination or any collapse across intensity categories as a primary
  WFF output. Any scalar transformation, netting, weighting, or value-weighted
  welfare score is an external downstream transformation, not a primary WFF
  output at any module level.
- **Welfare indicators require bridging.** A behavioural or physiological
  indicator must be connected to an Affective State by explicit evidence or
  reasoning; it cannot be used as a direct affective measure.

---

## Common failure modes

- Assigning a single intensity value to an entire Affective Experience rather
  than decomposing it into temporal segments.
- Collapsing Pain and Pleasure into a single welfare score, or collapsing
  intensity categories within Cumulative Pain or Cumulative Pleasure into a
  single scalar, as if this were a primary WFF output.
- Assigning intensity categories based on intuition rather than evidence.
- Treating absence of evidence for distress as evidence of absence of distress.
- Ignoring positive Affective Experiences and quantifying only negative ones.
- Omitting Pain-Track or Pleasure-Track structure and recording only a summary
  estimate without temporal segmentation.
- Using the same intensity mapping across species without species-specific
  calibration (see RD-003).
- Conflating Affective Experience type (fear, frustration) with intensity
  category, or omitting type records entirely.

---

## Related tools

- Hedonic-Track GPT (current preferred tool for this module's workflow)
  [NOTE: formerly referred to as Pain-Track GPT — that term is deprecated;
  see `glossary/deprecated_terms.yaml`]

---

## Resolved decisions relevant to this module

The following items that appeared as open questions in earlier scaffolding have
been resolved. Do not reintroduce them as open questions.

- **Pleasure intensity category set** — resolved by RD-001
  (`review/resolved_methodological_decisions.md`). The categories are
  No Pleasure, Satisfaction, Joy, Euphoria, and Bliss; definitions are in
  `canon/intensity_categories_pleasure.md`.
- **Inter-individual variation** — resolved by RD-002
  (`review/resolved_methodological_decisions.md`). The WFF does not require
  full individual-level modelling; uncertainty is represented through
  probability distributions, ranges, and sensitivity analysis.
- **Species-internal use of intensity categories** — resolved by RD-003
  (`review/resolved_methodological_decisions.md`). Category definitions are
  not species-specific; evidential application is species-specific;
  interspecific comparison requires explicit Module Ψ assumptions.

## Follow-up items

Active empirical research directions for this module are tracked in
`review/follow_up_items.md`:

- FU-001 — species-specific evidence streams for non-mammalian Pain
  intensity assignment
- FU-002 — species-specific evidence streams for non-mammalian Pleasure
  intensity assignment
- FU-003 — body-integrity-threatening behaviour exemplars for Excruciating
  Pain in non-human animals

## Open questions

Active unresolved scientific or methodological questions for this module are
tracked in `review/open_questions.md`. See OQ-009 (concurrent Affective
Experiences at the segment level) for the current open question most directly
relevant to Module III intensity assignment.
