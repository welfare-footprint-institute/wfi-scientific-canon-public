# Module V: Econometric Calculation

**Status:** Scaffold prepared for scientific review
**Prepared for review by:** Wladimir J. Alonso
**Pending review:** Wladimir J. Alonso
**Additional review:** To be scheduled

> **Terminology note:** The current working term for this module is
> **"Econometric Calculation"**, in alignment with the primary WFF methodological
> source and the Technical Definitions source. The term
> "Aggregation and Standardization" appeared in earlier repository scaffolding and
> is deprecated. See `glossary/deprecated_terms.yaml`.

---

## Purpose

Integrate the per-episode Cumulative Pain and Cumulative Pleasure estimates
from Module III with the epidemiological parameters estimated in Module IV to
produce **Welfare Footprint metrics**.

Module III provides intensity-duration estimates for Affective Experiences
per episode. Module IV provides prevalence, occurrence, Affective Episode
Rate, and population-denominator information. Module V combines these streams
to estimate Cumulative Pain and Cumulative Pleasure for the average member of
the Target Population, for each Life-Fate, for the Production System, and,
where relevant, per unit of product or other reference denominator.

Aggregation means summing **like with like**: within the same valence and
intensity category, across Affective Experiences, Biological Consequences,
Life-Phases, Life-Fates, and reference periods. It does not mean converting,
collapsing, weighting, or creating equivalences between different intensity
categories or between Pain and Pleasure.

---

## Core entities

> Authoritative WFF definitions and resolved methodological decisions are
> maintained in `canon/`, `glossary/`, the relevant canon files, and
> `review/resolved_methodological_decisions.md`. This section identifies the
> entities used by this module and their module-specific role; it is not an
> independent glossary.

- **Cumulative Pain** — canonical WFF metric. **Module V role:** integrated
  estimate disaggregated by intensity category (Annoying, Hurtful, Disabling,
  Excruciating); reported separately from Cumulative Pleasure and never
  collapsed into a scalar.
- **Cumulative Pleasure** — canonical WFF metric. **Module V role:**
  integrated estimate disaggregated by intensity category (Satisfaction,
  Joy, Euphoria, Bliss); reported separately from Cumulative Pain and never
  collapsed into a scalar.
- **Average Population Member** — canonical WFF analytical construct.
  **Module V role:** representation of the expected Cumulative Pain or
  Cumulative Pleasure assigned to an average member of the Target
  Population, preserving disaggregation by valence and intensity category.
- **Life-Fate Accounting** — canonical WFF Module V operation. Accounting
  for the proportional contribution of each Life-Fate to Cumulative Pain
  and Cumulative Pleasure at the population, system, product-unit, or other
  reference-denominator level. A neutral econometric allocation operation;
  it does not imply value weighting, moral weighting, scalar weighting, or
  intensity-category weighting.
- **Life-Fate contribution factor** — Module V econometric parameter.
  Proportional contribution of each Life-Fate to the population, system,
  product unit, or other reference denominator.
- **Productivity metrics** — canonical WFF term / measurement concept
  (recorded in Module I). **Module V role:** used here to standardize
  estimates per unit of product
  (e.g., kg meat, litres milk, eggs, carcass weight, offspring).
- **Welfare Footprint per Unit of Product** — canonical WFF expression.
  **Module V role:** standardized expression of Cumulative Pain and
  Cumulative Pleasure per unit of animal-derived product (e.g., kg meat,
  litres milk, dozen eggs), preserving intensity-category disaggregation.
  Non-product denominators are handled via **Alternative Denominators**.
- **Alternative Denominators** — canonical WFF construct (Module V).
  Non-product or otherwise alternative reference denominators against which
  Cumulative Pain and Cumulative Pleasure may be expressed (e.g., per
  animal, per average population member, per Life-Phase, per population,
  per year, per person, per dollar spent, per intervention scenario, per
  region). Disaggregation by valence and intensity category is preserved;
  no scalar aggregation or cross-category collapse is implied.
- **Reference denominator** — canonical WFF analytical attribute.
  **Module V role:** identifies the unit each estimate is standardized to
  (animal, Life-Phase, lifespan, population, production cycle, product
  unit, intervention scenario, dollar spent, person, or other
  decision-relevant denominator).
- **Traceability layer** — Module V operational requirement. Structured
  contribution breakdown by Life-Fate, Life-Phase, Biological Consequence,
  and Affective Experience, preserving the analytical pathway from
  Module III and Module IV inputs to the final Module V estimate.
- **Uncertainty propagation outputs** — Module V reporting requirement.
  Propagated ranges, distributions, or scenario-based uncertainty across
  all reported estimates.

---

## Inputs

- **Module I outputs:** Production System, Life-Fates, Life-Phases,
  productivity metrics, product yields, mortality, losses, and analytical
  boundaries
- **Module III outputs:** Cumulative Pain [Episode] and Cumulative Pleasure
  [Episode], disaggregated by intensity category, with duration ranges and
  probability distributions per temporal segment
- **Module IV outputs:** prevalence, occurrence, Affective Episode Rate,
  Target Population denominator, Life-Fate denominator, Life-Phase timeframe,
  representativeness, and uncertainty
- **Life-Fate contribution factors:** proportional contribution of each
  Life-Fate to the population, system, product unit, or other reference
  denominator
- **Standardisation reference denominator:** animal, Life-Phase, lifespan,
  production cycle, population, product unit, intervention scenario, or other
  decision-relevant denominator

---

## Outputs

- Cumulative Pain and Cumulative Pleasure by intensity category, for each
  Life-Fate within the reference population and period
- System-level Cumulative Pain and Cumulative Pleasure derived through
  Life-Fate Accounting, preserving disaggregation by intensity category
- Welfare Footprint per Unit of Product, where applicable (e.g., per kg
  meat, per litre milk, per dozen eggs)
- Alternative denominators, where applicable (e.g., per animal, per
  average population member, per population, per year, per intervention
  scenario, per decision-relevant denominator)
- Traceable contribution breakdowns by Life-Fate, Life-Phase, Biological
  Consequence, and Affective Experience
- Uncertainty bounds on all outputs
- Documentation of all aggregation decisions and their rationale

Primary outputs are always disaggregated by valence, intensity category, and
reference denominator. Composite or collapsed expressions are external
downstream transformations, not Module V primary outputs; if used for decision
analysis or comparison, they must be clearly labelled as such with all
transformation assumptions stated.

### Worked example

An animal experiences the following during a reference period:
- Affective experience A → 1 hour of Disabling Pain
- Affective experience B → 2 hours of Disabling Pain + 1 hour of Hurtful Pain

Aggregated Cumulative Pain for this period:
- **Disabling Pain: 3 hours** (1 + 2 — summed within category)
- **Hurtful Pain: 1 hour** (kept separate — not converted to Disabling)

No equivalence is created between Hurtful and Disabling Pain.
No scalar total is produced.

---

## Required distinctions

- **Aggregation is not equivalence.** One hour of Hurtful Pain is not converted
  into Disabling Pain. Pleasure categories are not netted against Pain categories
  in primary WFF outputs. Aggregation sums like with like only.
- **Aggregation across conditions vs. across time.** Summing across different
  Affective Experiences and summing across clock time are distinct operations.
  Where Affective Experiences overlap temporally, the overlap must be recorded
  explicitly. Until conventions for concurrent Affective Experiences are
  resolved (see OQ-009 in `review/open_questions.md`), reports should preserve
  source-specific and category-specific contributions and state whether
  estimates are `Cumulative Affect [Baseline]` or
  `Cumulative Affect [Attention-Adjusted]`.
- **Intensity categories remain disaggregated in primary outputs.**
  Any collapse, weighting, or scalar transformation across intensity categories
  is an external downstream transformation, not a Module V primary output, and
  must not be presented as one.
- **Cumulative Pain and Cumulative Pleasure are reported separately.**
  They are not combined in primary outputs. Any scalar transformation,
  netting, weighting, Pain/Pleasure balancing, or cross-intensity weighting
  is an external downstream transformation, not a Module V primary output,
  and must not be presented as one.
- **Standardisation reference must be stated.** A welfare footprint without
  a reference period and population is not interpretable.

---

## Common failure modes

- Treating aggregation as equivalence — converting hours of Hurtful Pain into
  hours of Disabling Pain, or netting Pain against Pleasure, in primary outputs.
- Treating Pain and Pleasure as interchangeable, netting them, or reporting
  a combined Pain/Pleasure scalar as if it were a primary WFF output.
- Losing intensity disaggregation by reporting only a single total figure.
- Propagating only point estimates without uncertainty through aggregation.
- Presenting a downstream weighting or collapsing step as if it were the
  primary WFF output.
- Using an implicit reference period (e.g., "per animal") without specifying
  what point in the production cycle is meant.

---

## Related tools

[PLACEHOLDER — list relevant WFI tools when confirmed]

---

## Open questions and follow-up items

Active unresolved scientific or methodological questions for this module are
tracked in `review/open_questions.md`. Empirical research directions,
documentation cleanups, and future engineering tasks are tracked in
`review/follow_up_items.md`.

Items carried forward from earlier scaffolding for future review:

- How to handle conditions with uncertain affective valence in aggregation
- Propagation of uncertainty from Modules III and IV through aggregation
- Conventions for standardising reference denominators across assessments
  to enable valid comparison
