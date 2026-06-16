# Module VI: Welfare Footprints — Expression and Notation

**Status:** Scaffold for scientific review
**Review status:** Pending formal WFI scientific review
**Review record:** Tracked through the WFI canon review workflow

---

## Purpose

Define the canonical notation, scope declarations, and expression conventions
for reporting Welfare Footprint metrics produced by Module V.

Module VI ensures that WFF outputs are interpretable, traceable, and comparable
only under explicitly stated analytical boundaries and assumptions. It does
not generate new primary welfare estimates. It governs how Cumulative Pain,
Cumulative Pleasure, and related Welfare Footprint outputs are expressed for
scientific, policy, industry, advocacy, and public audiences.

Module VI is also the module in which optional Module Ψ / Interspecific Affect
assumptions are declared when cross-species comparisons are attempted. Because
WFF does not presently claim to have solved interspecific welfare weighting,
any cross-species expression must be presented as assumption-dependent,
scenario-based, and clearly separated from species-internal WFF estimates.

---

## Core entities

> Authoritative WFF definitions and resolved methodological decisions are
> maintained in `canon/`, `glossary/`, the relevant canon files, and
> `review/resolved_methodological_decisions.md`. This section identifies the
> entities used by this module and their module-specific role; it is not an
> independent glossary. Module VI is itself the canonical place for WFF
> **expression and notation** scaffolding, so several entries below are
> operational definitions for that scaffolding rather than references
> elsewhere.

- **Welfare Footprint notation** — Module VI scaffolding entity. Formal
  symbolic expression of WFF results.
- **Cumulative Pain notation** — Module VI scaffolding entity for the
  canonical WFF metric Cumulative Pain. Formal expression of time in each
  Pain intensity category (Annoying, Hurtful, Disabling, Excruciating),
  reported separately and never collapsed into a scalar.
- **Cumulative Pleasure notation** — Module VI scaffolding entity for the
  canonical WFF metric Cumulative Pleasure. Formal expression of time in
  each Pleasure intensity category (Satisfaction, Joy, Euphoria, Bliss),
  reported separately and never collapsed into a scalar.
- **Cumulative Affect notation** — Module VI scaffolding entity. Joint
  disaggregated representation of Cumulative Pain and Cumulative Pleasure;
  not a single scalar score.
- **Units of measurement** — Module VI scaffolding entity. Typically time
  units (e.g., hours, days) per intensity category per reference
  denominator.
- **Scope Qualifier** — Module VI scaffolding entity. Mandatory label
  specifying the analytical level and reference period of the estimate
  (e.g., `[Episode]`, `[Life-Phase]`, `[Lifespan]`, `[per kg meat]`,
  `[per dozen eggs]`, `[per intervention scenario]`).
- **Analytical Boundaries** — canonical WFF entity (see
  `canon/terminology.md`). **Module VI role:** the defined scope of an
  assessment — species, Production System, Life-Fates, Life-Phases,
  Affective Experiences, geography, timeframe, and level of analysis —
  declared as part of expression.
- **Reference period** — canonical attribute. **Module VI role:** the time
  interval over which the estimate accumulates, as expressed in notation.
- **Reference denominator** — canonical attribute (defined in Module V).
  **Module VI role:** the unit referenced in the expression — episode,
  Life-Phase, lifespan, animal, population, product unit, intervention
  scenario, dollar spent, person, or other decision-relevant denominator.
- **Disaggregation format** — Module VI scaffolding requirement. Required
  disaggregation by valence, intensity category, Affective Experience,
  Biological Consequence, Life-Phase, Life-Fate, and Production System.
- **Uncertainty representation conventions** — Module VI scaffolding
  entity. Ranges, probability distributions, confidence or credibility
  intervals, scenario-specific outputs, graphical uncertainty bars, and
  explanatory notes.
- **Traceability requirements** — Module VI scaffolding requirement.
  Links from final expressions back to Module I–V intermediate estimates
  and underlying source evidence.
- **Baseline vs Attention-Adjusted expression** — Module VI scaffolding
  requirement. Explicit declaration of whether reported Cumulative Affect
  is `Cumulative Affect [Baseline]` or `Cumulative Affect [Attention-Adjusted]`.
- **Interspecific comparison expression** — Module VI scaffolding entity.
  Applies when Module Ψ scenarios are invoked.
- **Species-internal intensity notation** — Module VI scaffolding entity.
  Unqualified WFF category labels (Annoying, Hurtful, …; Satisfaction,
  Joy, …) referring by default to the species under assessment.
- **Human-anchored reference notation** — Module VI scaffolding entity.
  Explicitly marked categories used in interspecific comparisons:
  Annoying(h), Hurtful(h), Disabling(h), Excruciating(h); Satisfaction(h),
  Joy(h), Euphoria(h), Bliss(h).
- **Scenario labels for optional interspecific assumptions** — Module VI
  scaffolding entity. Formal labels identifying each declared cross-species
  comparison scenario (e.g., "Ψ Scenario A: Disabling(h) ceiling").

---

## Inputs

- **Module V species-internal outputs:** Cumulative Pain and Cumulative
  Pleasure by intensity category, reference denominator, and uncertainty
  bounds
- Traceability data from prior modules: Life-Fates, Life-Phases, Biological
  Consequences, Affective Experiences, and source assumptions
- Analytical Boundaries: species, Production System, geography, timeframe,
  Life-Fates, Life-Phases, Affective Experiences included and explicitly
  excluded
- Scope Qualifier required for each estimate
- Audience and communication context (scientific paper, policy brief,
  certification material, consumer-facing summary, dashboard, farm report)
- **Optional Module Ψ assumption sets** (only when interspecific comparison
  is attempted): proposed mapping to human-anchored reference categories,
  intensity-ceiling assumptions, subjective-time assumptions, confidence
  ratings, and sensitivity-analysis scenarios

> Architecture note: Module V provides the species-internal welfare estimates.
> Module Ψ provides the interspecific-affect assumptions. Module VI expresses
> any cross-species comparison scenario by combining Module V outputs with
> declared Module Ψ assumption sets.

---

## Outputs

- Formally expressed Cumulative Pain and Cumulative Pleasure estimates with
  explicit Scope Qualifiers and uncertainty representation
- Welfare Footprint tables and figures with explicit Analytical Boundaries
- Standardized disaggregated representations suitable for comparison when
  Analytical Boundaries and assumptions are aligned
- Documentation of Analytical Boundaries, exclusions, assumptions, and
  uncertainty
- Traceability documentation linking final expressions back to Life-Fates,
  Life-Phases, Biological Consequences, and Affective Experiences
- Audience-specific summaries that preserve access to the underlying
  disaggregated data
- Optional interspecific comparison expressions, clearly labelled as
  assumption-dependent and scenario-based

Primary WFF outputs remain species-internal unless an explicit Module Ψ
scenario is declared. Cross-species expressions must not be presented as
assumption-free or as resolved welfare equivalences.

---

## Required distinctions

- **Expression is not recalculation.** Module VI presents Module V outputs;
  it does not generate new welfare estimates.
- **Scope Qualifier is mandatory.** Every published WFF estimate must include
  an explicit Scope Qualifier; estimates without one are uninterpretable.
- **Analytical Boundaries determine comparability.** Estimates from
  assessments with different Analytical Boundaries are not directly comparable
  unless the differences are explicitly reconciled.
- **Primary disaggregated outputs vs. derived external transformations.**
  Primary WFF outputs preserve disaggregation by valence and intensity
  category. Any scalar transformation, netting, weighting, or value-weighted
  welfare score is an external downstream transformation, not a primary WFF
  output, and must not be presented as one.
- **Species-internal estimates vs. interspecific expressions.** Species-
  internal estimates are the default. Interspecific expressions require an
  explicit Module Ψ scenario.
- **Interspecific comparison is assumption-dependent.** Cross-species
  expressions must declare their assumptions; they must not be presented as
  resolved scientific equivalences.
- **Ceiling assumptions must be declared.** Any assumed Pain or Pleasure
  intensity ceiling for a species must be stated explicitly.
- **Subjective time assumptions must be declared separately.** Assumptions
  about subjective time perception must be distinguished from intensity-
  ceiling assumptions; the two must not be collapsed into a single scalar
  adjustment.
- **Baseline vs Attention-Adjusted expression.** When Cumulative Affect is
  reported, the notation must state whether the estimate is
  `Cumulative Affect [Baseline]` or `Cumulative Affect [Attention-Adjusted]`.
- **Reporting for different audiences must preserve traceability.** Audience
  simplifications may differ in presentation, but the underlying disaggregated
  data must remain accessible and unaltered.
- **Uncertainty representation is required.** Point estimates presented
  without uncertainty bounds are incomplete WFF outputs.

---

## Interspecific comparison conventions

The WFF remains agnostic about definitive interspecific welfare weights. The
primary WFF calculation produces species-internal estimates of Cumulative
Pain and Cumulative Pleasure.

When cross-species comparison is required, Module VI may express optional
Module Ψ scenarios. These scenarios must state:

- the species being compared;
- the species-internal WFF estimates;
- whether human-anchored reference categories are used;
- the proposed mapping between species-internal categories and human-anchored
  reference categories;
- any assumed affective-intensity ceiling;
- any assumed adjustment for subjective time perception;
- whether the scenario reflects empirical evidence, normative weighting,
  sensitivity analysis, or a mixture;
- whether alternative plausible mappings change the conclusion.

Example notation:

- `Cumulative Pain [Lifespan, Species-internal]`
- `Cumulative Pain [per kg, Species-internal]`
- `Cumulative Pain [per kg, Ψ Scenario A: Disabling(h) ceiling]`
- `Cumulative Pain [per kg, Ψ Scenario B: Excruciating(h) ceiling]`
- `Cumulative Pain [per kg, Ψ Scenario C: no interspecific adjustment]`

No interspecific expression should be presented without its scenario label
and declared assumptions.

---

## Common failure modes

- Reporting estimates without Scope Qualifiers.
- Comparing estimates with different Analytical Boundaries as if directly
  commensurable.
- Treating species-internal categories as automatically comparable across
  species.
- Presenting interspecific assumptions as settled scientific facts.
- Failing to distinguish intensity-ceiling assumptions from subjective-time
  assumptions.
- Using human-anchored notation without explaining the underlying mapping
  assumptions.
- Netting Pain against Pleasure, or collapsing intensity categories within
  Cumulative Pain or Cumulative Pleasure into a single scalar, as if this
  were a primary WFF output.
- Allowing audience simplification to propagate back into the primary data
  (i.e., permanently collapsing categories for convenience).
- Omitting uncertainty representation from summary tables.

---

## Related tools

[PLACEHOLDER — list relevant WFI reporting tools when confirmed]

---

## Open questions

[PLACEHOLDER — document notation conventions pending scientific review]
