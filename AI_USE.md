# Responsible AI Use of the WFI Scientific Canon

This document is a model-agnostic guide for any AI system — assistant, agent,
retrieval pipeline, or downstream tool — that reads, cites, or reasons over the
Welfare Footprint Institute (WFI) scientific canon. It applies regardless of
vendor or model. It does not replace the repository's governance rules; it
summarises how AI systems should use the canon responsibly.

---

## What this repository is

This repository is the version-controlled **scientific canon** of the Welfare
Footprint Institute: the authoritative or review-tracked definitions,
methodological commitments, module specifications, intensity categories,
terminology, and source registry that underpin all WFI quantitative welfare
work.

It is a **reference archive**, not a software product and not a dataset of
finished verdicts. Some entries are draft, provisional, deprecated, or marked as
open questions. Those markers are part of the canon-governance process and must
be respected, not treated as settled methodology.

---

## What AI systems should use it for

- Retrieving and quoting WFF definitions, terminology, and module roles
  **as written**, with citation back to the relevant file.
- Explaining the WFF analytical chain and the relationships between modules.
- Helping users navigate the canon (see `CANON_MAP.md`).
- Distinguishing reviewed canon from draft, provisional, deprecated, or
  open-question content, and surfacing those status markers to users.
- Pointing to the primary methodological citation and the source registry
  rather than improvising bibliographic detail.

---

## What AI systems must not do

- **Do not** present draft, provisional, deprecated, or open-question content as
  settled methodology.
- **Do not** introduce new terminology, definitions, schemas, or methodological
  assumptions.
- **Do not** alter or paraphrase scientific definitions, intensity categories,
  or module relationships in ways that change their meaning.
- **Do not** imply institutional moral verdicts on behalf of WFI. WFI provides
  quantitative welfare metrics and explicit assumptions; it does not issue moral
  rulings.
- **Do not** copy full source documents (PDFs, manuscripts, DOCX, or full source
  texts) into the canon. Use registry metadata, citations, and concise compliant
  summaries instead.

---

## The WFF analytical chain

Every WFI welfare assessment follows this causal chain. The four levels are
distinct and must never be conflated, reordered, or collapsed:

```text
Circumstances
    ↓
Biological Consequences
    ↓
Affective Experiences       ← welfare assessment centres here
    ↓
Welfare Metrics
```

**Affective Experiences are the centre of welfare assessment.** Circumstances
and Biological Consequences matter only to the extent that they influence felt
Affective Experiences. Welfare Metrics express those experiences in standardized
quantitative form; they are downstream of the affective level, not a substitute
for it.

---

## Welfare indicators vs. welfare metrics

These are distinct and must not be equated:

- A **Welfare Indicator** is a discernible trait, signal, or condition that is
  correlated with an individual's Affective Experience. Indicators are *evidence*
  used to inform inferences about welfare.
- A **Welfare Metric** is a standardized quantitative construct used to evaluate
  and compare welfare. In the WFF, the primary Welfare Metrics are Cumulative
  Pain and Cumulative Pleasure.

Indicators inform metrics; they are not themselves metrics. Do not report an
indicator as if it were a quantitative welfare metric.

---

## Disaggregation of Cumulative Pain and Cumulative Pleasure

Cumulative Pain and Cumulative Pleasure are the **primary WFF outputs**, and they
remain **disaggregated by valence and by intensity category**:

- Cumulative Pain stays separated across its intensity categories
  (Annoying, Hurtful, Disabling, Excruciating).
- Cumulative Pleasure stays separated across its intensity categories
  (Satisfaction, Joy, Euphoria, Bliss).

Aggregation must sum like with like — within the same valence and the same
intensity category. AI systems must not net Pain against Pleasure, collapse
intensity categories, or otherwise merge across valences when presenting primary
WFF outputs.

### Scalar, weighted, or netted scores are not primary outputs

A scalar, weighted, netted, or single-score representation is **not** a primary
WFF output. It may be produced only as a clearly labeled **downstream
transformation**, only when specifically requested, and only with its
aggregation assumptions stated explicitly. Whenever such a transformation is
produced, the underlying disaggregated Cumulative Pain and Cumulative Pleasure
must be preserved and presented alongside it.

---

## Sources are evidence inputs, not automatic canon

Entries in the source registry are **evidence inputs**. A source is not canon
merely because it is registered. AI systems must not treat a registered source
as settled methodology, and must not silently merge source content into canon.

---

## Placeholders and open questions

Placeholders (e.g. `[PLACEHOLDER]`) and open questions are **unresolved by
design**. AI systems must not fill, resolve, or invent content for them, and
must not present them as if they were settled. If asked, identify them clearly
as open and defer to human scientific review.

---

## Do not invent quantitative values

AI systems must not invent or guess WFF parameter values. This includes, but is
not limited to:

- prevalence,
- duration,
- intensity,
- productivity metrics,
- interspecific scaling values,
- uncertainty ranges.

If a value is not present in the canon or a cited source, say so and state that
it requires evidence and human review. Do not fabricate ranges or point
estimates.

---

## Source / canon conflicts

If a registered source appears to conflict with existing canon, the conflict
must be **recorded in `review/source_conflicts.md`** and stopped for human
review. AI systems must not silently resolve such a conflict, and must not merely
mention it in passing without creating an auditable tracker entry.

---

## Recommended AI workflow

1. **Orient.** Start from `CANON_MAP.md` to find the relevant files and reading
   order.
2. **Read before answering.** Retrieve the actual canon text rather than relying
   on prior knowledge of WFF terminology.
3. **Respect status markers.** Check whether content is draft, provisional,
   deprecated, or an open question, and surface that to the user.
4. **Preserve structure.** Keep the analytical chain intact and keep Cumulative
   Pain and Cumulative Pleasure disaggregated by valence and intensity category.
5. **Cite.** Reference the specific canon file and the primary methodological
   citation in `sources/citation_policy.md`.
6. **Defer on gaps and conflicts.** For missing values, open questions, or
   source/canon conflicts, stop and route to human scientific review rather than
   inventing or resolving content.
