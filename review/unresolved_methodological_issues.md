# Unresolved Methodological Issues

This file tracks methodological issues that require resolution before
WFF assessments in the relevant area can be considered fully rigorous.
Unlike open questions (which may be descriptive), entries here identify
specific gaps in the methodology that need formal decisions.

Do not close entries without documented scientific review and approval.

Status: active
Last reviewed: [PLACEHOLDER]

> **Scope and reading note (not canon).** This file is an unresolved-issues
> tracker, **not** canon. Its entries record open methodological questions and
> must be read alongside `canon/principles.md`, `canon/terminology.md`,
> `AI_USE.md`, and the relevant module files. Nothing in this file overrides the
> canon or defines new WFF outputs. In particular:
>
> - Primary WFF outputs remain **Cumulative Pain and Cumulative Pleasure,
>   disaggregated by valence and intensity category**.
> - Any scalar, weighted, composite, netted, or single-score representation is an
>   **external downstream transformation only** — never a primary WFF output. Such
>   a transformation requires explicit assumptions and must preserve and present
>   the underlying disaggregated Cumulative Pain and Cumulative Pleasure alongside
>   it.

---

## UMI-001: Weighting scheme for optional external composite / scalar-summary transformations

**Scope:** This issue concerns only **optional external downstream**
decision-analysis or scalar-summary transformations (for example, a weighted
composite or single-score representation). It does **not** concern primary
Module V outputs. Primary Module V outputs are Cumulative Pain and Cumulative
Pleasure, disaggregated by valence and intensity category; they are not a
weighted composite and do not require a weighting scheme (see
`canon/principles.md`, `modules/v_econometric_calculation.md`, and `AI_USE.md`).

**Issue (unresolved):** If an external transformation chooses to combine
intensity categories into a composite or scalar summary, it must apply some
weighting scheme. No formally approved weighting scheme exists in the current
WFF canon — and none is required for primary WFF outputs.

**What is needed:** Should such an external transformation be standardised, it
would require a principled, reviewable weighting scheme with documented
rationale, explicit assumptions, uncertainty analysis, and sensitivity testing
across alternative weight specifications. Any such transformation must preserve
and present the underlying disaggregated Cumulative Pain and Cumulative Pleasure
alongside it, and must be clearly labelled as a non-primary, downstream output.

**Impact:** Affects only optional external downstream decision-analysis or
scalar-summary transformations. It does **not** define or replace primary
Module V outputs, which remain disaggregated by valence and intensity category.

**Status:** unresolved.

**Assigned to:** Wladimir J. Alonso / Cynthia

---

## UMI-002: Evidential basis for optional Module Ψ interspecific assumptions

**Scope:** Module Ψ concerns **optional** interspecific scaling / interspecific
affect. A single interspecific scaling factor is **not** a primary Module Ψ
entity. Any numerical factors are scenario-specific assumptions or external
transformation parameters, not a primary or canonical output. The scenario-based
approach defined in `modules/psi_interspecific_scaling.md` remains controlling.

**Issue (unresolved):** When an optional cross-species comparison is attempted,
it relies on explicit, scenario-specific assumptions about relative affective
capacity across species. No approved method for deriving or updating such
scenario assumptions is documented in canon.

**What is needed:** A transparent, scenario-based methodology for deriving and
documenting any such interspecific assumptions — including the neurobiological,
behavioural, or other evidence base, explicit uncertainty bounds, and an update
procedure as new evidence accumulates — consistent with
`modules/psi_interspecific_scaling.md`. Any numerical factor must be presented as
a scenario-specific assumption or external transformation parameter requiring
explicit uncertainty and review, never as a single settled scaling constant.

**Impact:** Affects only optional cross-species comparisons and multi-species
portfolio assessments. It does **not** change within-species WFF outputs, which
remain disaggregated Cumulative Pain and Cumulative Pleasure by valence and
intensity category.

**Status:** unresolved.

**Assigned to:** Wladimir J. Alonso / Cynthia

---

## UMI-003: Duration estimation protocols

**Issue:** Estimates of how long a given affective experience persists in an
affected individual are required for Module III but no standardised elicitation
or estimation protocol has been approved.

**What is needed:** A protocol specifying how duration estimates are derived
(from literature, expert elicitation, or modelling), how uncertainty is
characterised, and how estimates are updated.

**Impact:** Affects all Module III outputs and downstream aggregation.

---

## UMI-004: Bridging welfare indicators to affective experiences

**Issue:** The methodology for translating welfare indicators (e.g., gait scores,
lesion grades, corticosteroid levels) into affective intensity categories lacks
a formal, species-specific calibration framework.

**What is needed:** A documented approach to indicator-to-affect bridging,
including the evidence required and the uncertainty to be attached.

**Impact:** Affects Module II → Module III transitions across all assessments.

---

## [PLACEHOLDER]

Additional methodological issues to be added as assessments progress.
