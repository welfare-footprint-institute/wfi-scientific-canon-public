# Canon Map — Reading Path Through the WFI Scientific Canon

This is a **navigation document** for humans and AI tools. It gives an explicit
reading path through the WFI scientific canon. It does not define methodology and
makes no new scientific claims; the canonical content lives in the files it
points to. Where a status marker (draft, provisional, deprecated, open question)
applies, defer to the referenced file.

See also `AI_USE.md` for responsible-use rules and `README_FOR_AGENTS.md` for the
agent-facing summary.

---

## Start here

If you are new to the canon, read in this order:

1. [`README.md`](README.md) — what the repository is, its scope, and the WFF
   chain at a glance.
2. [`AI_USE.md`](AI_USE.md) — responsible-use rules for AI systems.
3. [`canon/terminology.md`](canon/terminology.md) — the core human-readable
   terminology canon and the spine of the framework.
4. This map — to locate module-specific and topic-specific files.

---

## Canonical reading order

1. [`canon/principles.md`](canon/principles.md) — foundational principles.
2. [`canon/terminology.md`](canon/terminology.md) — core terms, grouped by
   conceptual role and module.
3. [`canon/intensity_categories_pain.md`](canon/intensity_categories_pain.md) and
   [`canon/intensity_categories_pleasure.md`](canon/intensity_categories_pleasure.md)
   — operational definitions of the intensity categories.
4. [`canon/evidence_standards.md`](canon/evidence_standards.md) and
   [`canon/uncertainty_principles.md`](canon/uncertainty_principles.md) — how
   evidence and uncertainty are handled.
5. [`canon/scientific_lane.md`](canon/scientific_lane.md) and
   [`canon/visualization_conventions.md`](canon/visualization_conventions.md) —
   scope of scientific claims and presentation conventions.
6. The module files (below), in numerical order I → VI, with Ψ as an optional
   module.
7. [`glossary/wff_terms.yaml`](glossary/wff_terms.yaml) — machine-readable term
   definitions.
8. [`sources/`](sources/) — source registry and citation policy.
9. [`review/`](review/) — open questions, unresolved issues, resolved decisions,
   and source conflicts.

---

## Module-specific reading map

Each module is specified in its module file and elaborated in the corresponding
section of `canon/terminology.md`. The WFF analytical chain
(`Circumstances → Biological Consequences → Affective Experiences →
Welfare Metrics`) runs through the modules in order.

### Module I — Zootechnical Description
- [`modules/i_zootechnical_description.md`](modules/i_zootechnical_description.md)
- `canon/terminology.md` §3 (Module I terms)

### Module II — Veterinary Inventory
- [`modules/ii_veterinary_inventory.md`](modules/ii_veterinary_inventory.md)
- `canon/terminology.md` §4 (Module II terms)

### Module III — Affective Quantification
- [`modules/iii_affective_quantification.md`](modules/iii_affective_quantification.md)
- `canon/terminology.md` §5 (Module III terms)
- `canon/intensity_categories_pain.md` and
  `canon/intensity_categories_pleasure.md` (intensity-category definitions)

### Module IV — Epidemiological Review
- [`modules/iv_epidemiological_review.md`](modules/iv_epidemiological_review.md)
- `canon/terminology.md` §6 (Module IV terms)

### Module V — Econometric Calculation
- [`modules/v_econometric_calculation.md`](modules/v_econometric_calculation.md)
- `canon/terminology.md` §7 (Module V terms)
- Note: "Aggregation and Standardization" is the **deprecated** name for this
  module. See `glossary/deprecated_terms.yaml`.

### Module VI — Welfare Footprints: Expression and Notation
- [`modules/vi_expression_notation.md`](modules/vi_expression_notation.md)
- `canon/terminology.md` §8 (Module VI terms)

### Module Ψ — Interspecific Scaling / Interspecific Affect
- [`modules/psi_interspecific_scaling.md`](modules/psi_interspecific_scaling.md)
- `canon/terminology.md` §9 (Module Ψ terms)
- This is an **optional** module and parts of it are marked provisional; defer to
  the status markers in the referenced files.

---

## Pain and pleasure intensity categories

The intensity categories are valence-specific and must not be treated as opposite
points on a single common scale.

- Pain: [`canon/intensity_categories_pain.md`](canon/intensity_categories_pain.md)
- Pleasure: [`canon/intensity_categories_pleasure.md`](canon/intensity_categories_pleasure.md)
- Surrounding terminology (Pain, Pleasure, Affective State, Pain-Track,
  Pleasure-Track, Cumulative Pain, Cumulative Pleasure):
  `canon/terminology.md` §5.

Cumulative Pain and Cumulative Pleasure are the primary WFF outputs and remain
disaggregated by valence and intensity category. For how AI systems must handle
this, see `AI_USE.md`.

---

## Terminology and deprecated terms

- Human-readable terminology: [`canon/terminology.md`](canon/terminology.md)
- Machine-readable terms: [`glossary/wff_terms.yaml`](glossary/wff_terms.yaml)
- Deprecated terms and their replacements:
  [`glossary/deprecated_terms.yaml`](glossary/deprecated_terms.yaml)
- Change history of terms:
  [`glossary/term_change_log.md`](glossary/term_change_log.md)
- Worked terminology examples:
  [`examples/terminology_examples.md`](examples/terminology_examples.md)

---

## Sources, citations, and source conflicts

- Source registry: [`sources/source_registry.yaml`](sources/source_registry.yaml)
- Citation policy and primary citation:
  [`sources/citation_policy.md`](sources/citation_policy.md)
- Recorded source/canon conflicts:
  [`review/source_conflicts.md`](review/source_conflicts.md)

Registered sources are evidence inputs, not automatically canon. A source/canon
conflict must be recorded in `review/source_conflicts.md` and routed to human
review, not silently resolved.

---

## What to read when terms appear to conflict

When files or interpretations appear to disagree, consult these in order and stop
at the first that resolves the question:

1. [`canon/terminology.md`](canon/terminology.md)
2. [`glossary/wff_terms.yaml`](glossary/wff_terms.yaml)
3. [`review/resolved_methodological_decisions.md`](review/resolved_methodological_decisions.md)
4. The relevant module file's role descriptions (the `modules/` file for the
   module in question)
5. [`sources/source_registry.yaml`](sources/source_registry.yaml)

Module role descriptions are module-specific and are not independent glossaries.
If a module file appears to conflict with canon, flag the discrepancy for human
review rather than silently resolving it.
