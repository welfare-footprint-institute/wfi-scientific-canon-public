# Module IV: Epidemiological Review

**Status:** Scaffold prepared for scientific review
**Prepared for review by:** Wladimir J. Alonso
**Pending review:** Wladimir J. Alonso
**Additional review:** To be scheduled

---

## Purpose

Module IV estimates the **epidemiological parameters** required to scale
episode-level Affective Quantification outputs (Module III) to the Target
Population. It does **not** calculate Cumulative Pain or Cumulative Pleasure;
that integration is performed in Module V.

Module IV provides:

- **prevalence** — how many animals in the Target Population are affected;
- **occurrence** — how often affected animals experience the Biological
  Consequence during the analysed timeframe;
- **Affective Episode Rate** — the expected number of discrete Affective
  Experiences generated per occurrence, where one Biological Consequence gives
  rise to discrete or repeated Affective Experiences;
- **population denominators** for the Target Population;
- **Life-Fate-specific denominators**;
- **Life-Phase-specific timeframes**;
- **representativeness and uncertainty information** for each parameter.

These parameters are passed to Module V (Econometric Calculation), which
integrates them with Module III episode-level Cumulative Pain and Cumulative
Pleasure estimates to produce Welfare Footprint metrics.

---

## Core entities

> Authoritative WFF definitions and resolved methodological decisions are
> maintained in `canon/`, `glossary/`, the relevant canon files, and
> `review/resolved_methodological_decisions.md`. This section identifies the
> entities used by this module and their module-specific role; it is not an
> independent glossary.

- **Target Population** — canonical WFF entity. **Module IV role:** the
  specific group of animals to which an epidemiological estimate applies,
  defined by Life-Fate, Life-Phase, Production System, geography, and
  timeframe.
- **Life-Fate-specific denominator** — Module IV epidemiological parameter.
  The relevant count or size measure for a given Life-Fate within the
  assessment boundaries.
- **Life-Phase-specific timeframe** — Module IV epidemiological parameter.
  The defined period over which prevalence, occurrence, and Affective
  Episode Rate are estimated for each Life-Phase.
- **Point prevalence** — canonical epidemiological measure. **Module IV
  role:** proportion of the Target Population affected at a given point in
  time.
- **Period prevalence** — canonical epidemiological measure. **Module IV
  role:** proportion affected over a defined interval.
- **Production-cycle or lifetime prevalence** — canonical epidemiological
  measure. **Module IV role:** proportion affected at any point during the
  production cycle or lifespan.
- **Occurrence** — canonical WFF entity. **Module IV role:** the number of
  times an affected animal typically experiences, develops, or is exposed
  to a given Biological Consequence during the analysed timeframe; distinct
  from prevalence, which counts how many animals are affected.
- **Affective Episode Rate** — canonical WFF entity. **Module IV role:**
  the expected number of discrete Affective Experiences generated per
  occurrence of a Biological Consequence; needed when the relationship
  between Biological Consequences and Affective Experiences is not
  one-to-one.
- **Continuous vs. episodic Affective Experience** — Module IV
  characterization. For continuous conditions, total accumulated duration
  per occurrence or exposure period is used directly rather than forcing
  burden into discrete episodes.
- **Population fraction affected** — Module IV characterization. Relevant
  subgroup definitions within the Target Population.
- **Incidence rate** — supporting epidemiological measure. **Module IV
  role:** new cases per unit time; subordinate to prevalence, occurrence,
  and Affective Episode Rate as the primary WFF operational parameters.
- **Confidence intervals, uncertainty ranges, and data quality descriptors**
  — Module IV reporting requirement applied to each parameter above.
- **Representativeness** — Module IV reporting requirement. Whether
  estimates reflect the Production System, Life-Fate, Life-Phase, geography,
  and timeframe of the assessment.

---

## Inputs

- **Module II output:** Biological Consequences and candidate Affective
  Experiences, including whether the relationship between a Biological
  Consequence and its Affective Experiences appears continuous, episodic,
  recurrent, or mixed
- **Optional coordination with Module III** to ensure episode definitions
  are compatible with Pain-Track or Pleasure-Track structure; Module IV does
  not require Module III intensity or duration estimates
- Epidemiological literature (peer-reviewed surveys, cohort studies,
  slaughterhouse data, field surveillance programmes)
- Industry and regulatory monitoring data (with source transparency)
- Expert estimates and elicitation where data are absent

---

## Outputs

For each Biological Consequence and associated Affective Experience:

- Target Population definition (Life-Fate, Life-Phase, Production System,
  geography, timeframe)
- Best-supported prevalence range
- Prevalence type: point / period / production-cycle / lifetime
- Occurrence estimate for affected animals during the analysed timeframe
- Affective Episode Rate, if the Biological Consequence produces discrete or
  repeated Affective Experiences
- Whether the Affective Experience is continuous, episodic, recurrent, or mixed
- Population denominator and relevant subgroup denominator
- Evidence base quality rating
- Notes on representativeness (Production System, Life-Fate, Life-Phase,
  geography)
- Data gaps, extrapolations, and conversion assumptions explicitly flagged

---

## Required distinctions

- **Prevalence ≠ Occurrence ≠ Affective Episode Rate.** Prevalence counts how
  many animals are affected. Occurrence counts how often each affected animal
  experiences the Biological Consequence. Affective Episode Rate counts how
  many Affective Experiences each occurrence generates. Conflating these
  parameters produces systematic under- or over-estimation of welfare burden.
- **Point prevalence vs. period prevalence vs. production-cycle prevalence.**
  These are not interchangeable.
  **Harmonisation rule (RD-004):** Estimates should be harmonised to the
  prevalence type required by the analysis — usually period prevalence over
  the relevant Life-Phase or lifespan segment. If conversion is not possible,
  estimates must not be pooled mechanically; they should be treated as separate
  evidence sources informing a range, with assumptions stated explicitly.
  See `review/resolved_methodological_decisions.md` (RD-004).
- **Individual vs. population level.** Prevalence is a population-level
  quantity; intensity (Module III) is an individual-level quantity.
  Population-level aggregation is performed in Module V.
- **Representative vs. convenience samples.** Studies using convenience
  samples (e.g., single farms, voluntary reporting) must be flagged.
- **Module IV ≠ Module V.** Module IV provides epidemiological scaling
  parameters. Module V performs aggregation, standardization per reference
  denominator, and expression per unit of product or other decision-relevant
  unit.

---

## Common failure modes

- Treating prevalence alone as sufficient to scale welfare estimates; omitting
  Occurrence and Affective Episode Rate.
- Using convenience samples as if they were representative population estimates.
- Mixing prevalence types (e.g., combining point and lifetime prevalence)
  without harmonisation or explicit conversion assumptions.
- Ignoring publication bias toward farms or systems with better welfare records.
- Treating regulatory minimum compliance rates as actual condition prevalence.
- Carrying forward point estimates without uncertainty bounds into Module V.
- Conflating Module IV epidemiological scaling with Module V aggregation and
  standardization.

---

## Related tools

[PLACEHOLDER — list relevant WFI tools or external databases when confirmed]

---

## Open questions

[PLACEHOLDER — document species-specific or system-specific data gaps
when identified]
