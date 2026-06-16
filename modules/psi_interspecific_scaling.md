# Module Ψ: Interspecific Affect

**Status:** Scaffold — open; high uncertainty; requires extensive scientific review
**Review status:** Pending formal WFI scientific review
**Review record:** Tracked through the WFI canon review workflow

> **Warning:** This module covers one of the most scientifically contested
> areas in welfare science. Treat all content here as provisional. Do not
> carry forward any specific affective-capacity assumptions, intensity
> ceilings, or candidate mappings as settled canon without explicit review
> and approval.

> **Filename note:** This file is `modules/psi_interspecific_scaling.md` for
> historical reasons. The current module name is **Module Ψ: Interspecific
> Affect**. Renaming the file is a separate operation deferred from this PR.

---

## Purpose

Provide a principled framework for assessing interspecific differences in
**affective capacity**.

Module Ψ evaluates what can be responsibly inferred about a species' capacity
for affective experience, including its plausible affective repertoire,
maximum intensity of Pain and Pleasure, and possible differences in
subjective time perception.

The module is designed to inform interspecific comparisons, but it does not
itself produce species-adjusted Welfare Footprint estimates. Its outputs
should be usable by any welfare metric or decision framework that requires
assumptions about interspecific affective capacity, not only by the WFF.

Within WFF, Module Ψ provides assumption sets and evidential profiles that
may later be used in Module VI when cross-species comparisons are attempted.
These assumptions must remain explicit, provisional, and scenario-based.

---

## Non-goals

Module Ψ does **not**:

- calculate Cumulative Pain or Cumulative Pleasure;
- modify Module III intensity assignments within a species;
- modify Module V Welfare Footprint estimates;
- directly produce species-adjusted Welfare Footprint estimates as primary
  Module Ψ outputs;
- assign definitive sentience weights;
- rank species by moral importance;
- provide a single universal interspecific conversion factor;
- imply that human experience is the universal maximum of affective
  intensity.

Its role is to document and structure provisional assumptions about
interspecific affective capacity so that downstream comparison is explicit,
auditable, and open to revision.

---

## Core entities

> Authoritative WFF definitions and resolved methodological decisions are
> maintained in `canon/`, `glossary/`, the relevant canon files, and
> `review/resolved_methodological_decisions.md`. This section identifies the
> entities used by this module and their module-specific role; it is not an
> independent glossary. Several Module Ψ entities below are **provisional
> constructs**, not settled WFF canon — see the Warning above and the
> per-entity notes.

- **Species** — canonical WFF entity. **Module Ψ role:** the taxonomic
  unit under analysis for interspecific-affect characterization.
- **Taxon or phylogenetic group** — Module Ψ provisional working concept.
  Broader grouping used when species-level evidence is sparse and
  group-level extrapolation is necessary.
- **Hedonic Capacity** — Module Ψ provisional concept (not settled canon).
  **Module Ψ role:** the inferred range and intensity of affective
  experience available to a species, conditional on sentience; distinct
  from the question of whether, or to what degree, the species is sentient.
- **Affective repertoire** — Module Ψ provisional concept. **Module Ψ
  role:** the kinds of affective experiences plausibly available to a
  species (e.g., physical Pain, fear, frustration, social affiliation,
  play, satiety).
- **Pain intensity ceiling** — Module Ψ provisional concept (scenario-
  based, not a settled scaling factor). **Module Ψ role:** the plausibly
  maximum intensity of negative affective experience attributable to a
  species, given current evidence.
- **Pleasure intensity ceiling** — Module Ψ provisional concept (scenario-
  based, not a settled scaling factor). **Module Ψ role:** the plausibly
  maximum intensity of positive affective experience attributable to a
  species, given current evidence.
- **Species-Internal Intensity Categories** — canonical WFF category sets
  (definitions in `canon/intensity_categories_pain.md` and
  `canon/intensity_categories_pleasure.md`). **Module Ψ role:** the
  unqualified WFF intensity categories used by default within a single
  species' welfare assessment.
- **Human-Anchored Reference Categories** — Module Ψ scenario-based
  reference set (not a settled canonical mapping). **Module Ψ role:**
  explicitly marked categories used in interspecific comparisons —
  Annoying(h), Hurtful(h), Disabling(h), Excruciating(h); Satisfaction(h),
  Joy(h), Euphoria(h), Bliss(h).
- **Candidate mapping** between species-internal categories and
  human-anchored reference categories — Module Ψ provisional scenario.
  A provisional, scenario-based hypothesis about how the two scales
  relate; never a single fixed mapping.
- **Subjective time perception assumptions** — Module Ψ provisional
  concept. Explicit assumptions about whether a unit of clock time
  corresponds to the same amount of subjectively experienced duration
  across species; must be distinguished from intensity-ceiling assumptions.
- **Sentience-relevant neurobiological features** — Module Ψ evidential
  input category. Anatomical, neural, and physiological features
  considered when assessing affective capacity; treated as proxies, not
  as direct measures of affective capacity.
- **Behavioural and motivational evidence relevant to affective capacity**
  — Module Ψ evidential input category (motivational trade-offs,
  conditioned place preference/aversion, learning, play, social
  behaviour).
- **Pharmacological evidence relevant to affective capacity** — Module Ψ
  evidential input category. Responsiveness to analgesics, anaesthetics,
  anxiolytics.
- **Evolutionary and ecological evidence relevant to affective capacity**
  — Module Ψ evidential input category.
- **Confidence level and uncertainty range** — Module Ψ reporting
  requirement applied to each assumption.
- **Plausible interspecific comparison scenarios** — Module Ψ output
  construct. Explicit scenario bundles ready for downstream use in
  Module VI.

> Note: An "interspecific scaling factor" is **not** a primary Module Ψ entity.
> If used at all, it is at most a downstream simplification that loses
> scenario detail; it is not preferred in canon and must not be presented as
> a Module Ψ output.

---

## Inputs

Module Ψ takes **species and evidence** as inputs, not Module V outputs.
Welfare Footprint calculation is downstream of Module Ψ assumption sets,
not a prerequisite for them.

- Species or taxa under consideration and the welfare-assessment context in
  which interspecific comparison is being attempted
- Comparative neurobiology and neuroanatomy
- Comparative cognition
- Affective neuroscience
- Pain, nociception, analgesia, and anaesthesia evidence
- Behavioural evidence (motivational trade-offs, conditioned place
  preference/aversion, learning, social behaviour, play)
- Pharmacological evidence
- Evolutionary and ecological evidence
- Temporal-resolution and sensory-physiology evidence relevant to subjective
  time
- Expert elicitation where empirical evidence is sparse, indirect, or
  contradictory

---

## Outputs

- **Species-level interspecific affect profile** — structured summary of
  what is and is not plausibly attributable to the species, across negative
  and positive affect
- **Evidence summary for affective capacity** — annotated evidence base
  used to support the profile
- **Plausible Pain intensity ceiling scenarios** — bounded provisional
  conclusions, not point estimates, where evidence is contested
- **Plausible Pleasure intensity ceiling scenarios** — same, for positive
  affect
- **Candidate mapping between species-internal intensity categories and
  human-anchored reference categories** — where attempted; always presented
  as one scenario among alternatives
- **Subjective time perception assumptions** — where relevant, stated
  separately from intensity-ceiling assumptions
- **Confidence rating for each assumption**
- **Sensitivity-analysis ranges for downstream comparisons**
- **Explicit statement of unresolved uncertainties and evidential gaps**
- **Recommendations for how Module VI should label any cross-species
  comparison** that uses these assumptions (e.g., scenario labels and
  required caveats)

Module Ψ does not output species-adjusted Welfare Footprint estimates. Any
species-adjusted, human-anchored, or interspecifically scaled expression is
a derived downstream expression and belongs in Module VI, with all
assumptions declared.

---

## Required distinctions

- **Interspecific Affect ≠ Welfare Footprint calculation.** Module Ψ
  characterizes affective capacity; it does not compute Cumulative Pain or
  Cumulative Pleasure.
- **Species input ≠ WFF output input.** Module Ψ takes species and evidence
  as inputs, not Module V outputs.
- **Species-internal categories ≠ human-anchored reference categories.**
  Unqualified WFF intensity terms refer to within-species categories by
  default; cross-species mappings require explicit (h) notation.
- **Hedonic Capacity ≠ sentience.** Sentience is a precondition; hedonic
  capacity addresses the range and intensity of affective experience given
  sentience.
- **Affective capacity ≠ moral weight.** Capacity is a descriptive,
  evidence-informed inference; moral weight is a normative judgment that is
  not produced by this module.
- **Neurobiological proxies ≠ affective capacity.** Brain-to-body ratio,
  neuron counts, and similar measures are proxies; they do not directly
  measure affective capacity.
- **Intensity ceiling ≠ subjective time perception.** These are two
  conceptually distinct assumptions that must not be collapsed into a single
  scalar.
- **Scenario-based assumptions ≠ settled scaling factors.** Module Ψ
  produces scenario bundles, not interspecific conversion constants.

---

## Common failure modes

- Treating Module Ψ as a standalone calculator that directly outputs
  species-adjusted Welfare Footprints, rather than as a source of explicit,
  provisional interspecific-affect assumptions for downstream scenario-based
  expression in Module VI.
- Using Module V outputs as required inputs to Module Ψ.
- Presenting a single interspecific scaling factor without scenario ranges.
- Treating human affective experience as the automatic maximum reference
  point for any species.
- Treating neurobiological proxies as direct measures of affective capacity.
- Conflating sentience, hedonic capacity, capacity for suffering, and moral
  weight.
- Applying assumptions derived for one taxonomic group to another without
  re-evaluation.
- Collapsing intensity-ceiling and subjective-time assumptions into a single
  unexplained scalar adjustment.
- Using interspecific assumptions without preserving the original
  species-internal estimates alongside.

---

## Related tools

[PLACEHOLDER]

---

## Open questions

This module contains more open questions than settled science. Active
unresolved questions are tracked in `review/open_questions.md`. Empirical
research directions and follow-up items (including non-mammalian evidence
development) are tracked in `review/follow_up_items.md` (see FU-001, FU-002,
FU-003). The resolved decision on species-internal use of WFF intensity
categories is recorded in `review/resolved_methodological_decisions.md`
(RD-003).

Key unresolved issues include:

- Which evidence streams are most informative about affective capacity, and
  what is their relative weight when streams conflict?
- How should Pain capacity and Pleasure capacity be evaluated separately,
  given that evidence bases differ across valences and across taxa?
- How should plausible intensity ceilings be assigned when direct
  measurement of subjective experience is impossible?
- When are human-anchored reference categories appropriate, and when do they
  introduce more distortion than insight?
- How should subjective time perception be represented independently of
  intensity ceilings?
- How should uncertainty be represented so that it remains usable by
  different welfare metrics and decision frameworks?
- How should the module treat taxa with sparse, indirect, or contradictory
  evidence?
- How should Module VI express cross-species comparisons in a way that does
  not imply that interspecific weighting has been solved?

Do not treat any current answer to these questions as settled canon.
