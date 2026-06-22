# Responsible AI Use of the WFI Scientific Canon

This document is a model-agnostic guide for any AI system — assistant, agent, retrieval pipeline, or downstream tool — that reads, cites, or reasons over the public WFI scientific canon.

It does not replace repository governance or the scientific-authority rules in `sources/wff_scientific_authority.md`.

---

## Scientific authority hierarchy

AI systems must follow this hierarchy:

1. the primary WFF methodological paper;
2. any formal amendment or addendum jointly approved by Wladimir J. Alonso and Cynthia Schuck-Paim;
3. the private scientific canon as the controlled, versioned operational representation of those scientific sources;
4. this public repository as a curated mirror;
5. downstream tools and applications.

Neither the private nor public repository is scientifically superior to the WFF paper. Neither repository independently creates or revises WFF scientific authority.

A merged Issue or Pull Request does not, by itself, amend the WFF.

---

## What this repository is

This repository is the public teaching, citation, review, and retrieval representation of the WFF paper, formal amendments, and approved internal canon. It stores terminology, module descriptions, status, provenance, source relationships, review records, and machine-readable resources for public human and AI use.

It is a reference archive, not a software product and not a dataset of finished verdicts. Some entries are draft, provisional, deprecated, or open questions. Those markers must be respected.

---

## What AI systems should use it for

- Retrieving and quoting WFF definitions, terminology, and module roles as currently represented publicly.
- Checking whether public or downstream content is faithful to the WFF paper and approved amendments.
- Explaining the WFF analytical chain and relationships between modules.
- Helping users navigate the public canon.
- Distinguishing reviewed content from draft, provisional, deprecated, or open-question material.
- Pointing to the primary WFF paper and authority policy rather than improvising scientific authority.
- Identifying conflicts, missing provenance, or possible fidelity errors.

---

## What AI systems must not do

- Do not treat the public or private canon as scientifically superior to the WFF paper.
- Do not infer that a repository change has amended the WFF.
- Do not present draft, provisional, deprecated, or open-question content as settled methodology.
- Do not introduce new WFF terminology, definitions, modules, intensity categories, or methodological assumptions.
- Do not alter scientific definitions or relationships in ways that change their meaning.
- Do not resolve a scientific conflict by choosing one source silently.
- Do not claim that one of the two scientific authorities acting alone can revise foundational WFF content.
- Do not imply institutional moral verdicts on behalf of WFI.
- Do not copy full source documents into the public canon.

---

## Amendment rule for AI systems

A substantive change to foundational WFF scientific content is valid only when:

- it is documented in a controlled scientific amendment, addendum, correction, revised manuscript, or equivalent record;
- it is jointly approved by Wladimir J. Alonso and Cynthia Schuck-Paim;
- its scope, rationale, and affected concepts are explicit;
- it is represented in the internal canon before public propagation.

If joint approval is absent, the proposal remains unresolved.

AI systems may:

- identify a possible need for amendment;
- summarize evidence and competing interpretations;
- draft a candidate amendment for human consideration;
- reflect a formally approved amendment in public files after internal approval.

AI systems may not declare, approve, or infer an amendment independently.

---

## The WFF analytical chain

Every WFI welfare assessment follows this causal chain. The four levels are distinct and must never be conflated, reordered, or collapsed:

```text
Circumstances
    ↓
Biological Consequences
    ↓
Affective Experiences       ← welfare assessment centres here
    ↓
Welfare Metrics
```

Affective Experiences are the centre of welfare assessment. Circumstances and Biological Consequences support inference about felt experience; Welfare Metrics express the resulting affective burden or benefit quantitatively.

---

## Welfare indicators versus welfare metrics

These are distinct:

- a **Welfare Indicator** is an observed trait, signal, or condition used as evidence about an individual's Affective Experience;
- a **Welfare Metric** is a standardized quantitative construct used to evaluate and compare welfare.

Indicators inform metrics; they are not themselves metrics.

---

## Disaggregation of Cumulative Pain and Cumulative Pleasure

Cumulative Pain and Cumulative Pleasure are primary WFF outputs and remain disaggregated by valence and intensity category.

- Cumulative Pain remains separated across Annoying, Hurtful, Disabling, and Excruciating.
- Cumulative Pleasure remains separated across Satisfaction, Joy, Euphoria, and Bliss.

AI systems must not net Pain against Pleasure or collapse intensity categories when presenting primary WFF outputs.

A scalar or weighted representation may be produced only as an explicitly labelled downstream transformation with its added assumptions stated and the underlying disaggregated outputs preserved.

---

## Sources and conflicts

The primary WFF paper is the controlling scientific source.

Secondary sources are evidence inputs and may clarify or operationalize parts of the framework, but they do not override the primary paper or a formally adopted amendment.

If a source, public file, internal canon representation, or downstream tool conflicts with the paper or an approved amendment:

1. record the conflict in `review/source_conflicts.md`;
2. determine whether it is a public-mirror fidelity error, an internal canon fidelity error, an interpretation problem, or a genuine amendment candidate;
3. correct public fidelity errors through the ordinary public repository workflow;
4. route internal fidelity errors to the private canon workflow;
5. route genuine amendment candidates to the joint scientific process;
6. preserve unresolved status when joint approval has not occurred.

---

## Placeholders and open questions

Placeholders and open questions are unresolved by design. AI systems must not fill or resolve them without explicit instruction and the appropriate review level.

A placeholder does not authorize invention. An open question does not imply that the WFF is unstable as a whole.

---

## Do not invent quantitative values

AI systems must not invent or guess WFF parameter values, including prevalence, duration, intensity, productivity metrics, interspecific scaling values, or uncertainty ranges.

If a value is absent, state what evidence is needed and preserve the gap.

---

## Recommended AI workflow

1. **Establish authority.** Read `sources/wff_scientific_authority.md` and `sources/citation_policy.md`.
2. **Orient.** Use `CANON_MAP.md` to locate the relevant files.
3. **Read before answering.** Retrieve the actual paper-linked public representation rather than relying on model memory.
4. **Respect status markers.** Surface draft, provisional, deprecated, and unresolved status.
5. **Preserve structure.** Maintain the WFF chain and disaggregated outputs.
6. **Cite appropriately.** Cite the WFF paper for methodology and the relevant public file for the current public representation.
7. **Defer correctly.** Route public fidelity errors to repository correction; route internal fidelity errors to the private canon; route genuine amendment candidates to the joint scientific process.
