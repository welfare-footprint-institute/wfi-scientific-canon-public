# Contributing to the WFI Scientific Canon

Thank you for your interest in the Welfare Footprint Institute (WFI) scientific
canon.

## What this repository is

This repository is a **curated public scientific reference** for the Welfare
Footprint Framework (WFF): its established terminology, methodological
commitments, module specifications, evidence standards, source registry, and
review records.

It is a **reference archive, not a software or product repository.** It does
not contain (and will not accept) application code, the Welfare Footprint
Atlas, tool infrastructure, or operational systems. See `manifest.yaml` and
`README.md` for the full scope.

This public repository is also **not the ordinary venue for redesigning the
WFF itself**. The WFF is the substantially consolidated methodology on which
WFI's scientific work is based. Most contributions should therefore improve
how faithfully, clearly, consistently, and transparently that methodology is
represented here.

---

## Contribution boundary: correcting the repository versus changing the WFF

Two very different activities must not be conflated.

### 1. Repository corrections and clarifications

These are the normal subject of Issues and Pull Requests in this public
repository. They include cases where the repository:

- misstates, oversimplifies, or inconsistently represents the established WFF;
- uses deprecated, ambiguous, or non-canonical terminology;
- conflates distinct WFF analytical levels, modules, indicators, or metrics;
- omits an important qualification, status marker, source, or provenance note;
- presents a downstream tool convention as though it were part of the WFF;
- contains a typo, citation error, broken link, formatting problem, or unclear
  explanation;
- fails to preserve WFF commitments such as disaggregation by valence and
  intensity category.

The review question for these contributions is primarily:

> Does the proposed correction make the public repository more faithful to the
> established WFF and its approved source material?

### 2. Substantive revision of the WFF

Proposals to change the WFF's underlying concepts, analytical chain, module
architecture, intensity-category definitions, methodological workflow, or
other foundational commitments are exceptional and belong to a separate,
higher-level scientific process.

Such a process may require:

- review of relevant scientific evidence and competing interpretations;
- formal discussion among WFI scientific leads and, where appropriate,
  external experts;
- development or revision of the primary WFF methodological manuscript or
  other scientific publications;
- explicit documentation of the decision, rationale, uncertainty, and scope;
- approval in the internal scientific-canon workflow before any corresponding
  public-mirror update.

An Issue may record that a foundational methodological question exists and
preserve its traceability. However, opening an Issue, accepting a discussion,
or merging an ordinary Pull Request does **not** by itself revise the WFF.

---

## Acceptable contributions

We welcome:

- **Typos** and obvious textual errors.
- **Citation fixes** consistent with `sources/citation_policy.md`.
- **Formatting corrections** and broken-link fixes.
- **Reports of departures from, or inconsistencies with, the established WFF.**
- **Terminology questions** about WFF terms or definitions.
- **Source-conflict reports** (see below).
- **Review notes** and proposed clarifications.
- **Proposed clarifications** that improve readability without changing
  scientific meaning.
- **Status and provenance corrections** where draft, provisional, deprecated,
  reviewed, or source information is missing or misleading.

For anything beyond a trivial correction, please open an Issue first using one
of the Issue templates so the question can be examined before a Pull Request.

---

## Contributions requiring a different process

The following should not be inserted into the public canon through an ordinary
Pull Request:

- a new WFF concept, intensity category, analytical level, or module;
- a redefinition of an established WFF term or methodological commitment;
- a restructuring of the WFF analytical chain or module workflow;
- a new aggregation or weighting rule presented as part of the WFF;
- a new, unreviewed scientific claim presented as settled canon;
- a substantive response to a source conflict that has not completed the
  appropriate scientific review process.

These questions may be documented for traceability, but they require the
higher-level scientific process described above. If that process results in an
approved internal canon revision, the public mirror can then be updated.

---

## Out-of-scope contributions

The following will not be accepted in this repository:

- Welfare Footprint **Atlas** or other product/tool code.
- **MCP servers**, agents, or tool infrastructure.
- **Validators or schemas**.
- **Full source documents** (PDFs, DOCX, manuscripts, or long source texts).
  Use registry metadata, citations, and short compliant excerpts instead.
- **Private or sensitive material** of any kind (see `SECURITY.md`).

---

## Review requirements for repository content

- **Changes to `canon/` and `modules/` require explicit review for fidelity to
  the established WFF and the approved internal canon.** Review is not a licence
  to redesign the framework through routine repository maintenance.
- **Substantive revisions of the WFF require the separate scientific process
  described above.** They are not settled by an accepted Issue or ordinary
  merged Pull Request.
- **Source registry entries are evidence inputs, not automatically canon.**
  A registered source does not change the WFF or this public canon until the
  appropriate review process has been completed.
- **Placeholders and open questions are not settled.** Markers such as
  `[PLACEHOLDER — requires scientific review]`, `[OPEN QUESTION]`, `[DRAFT]`,
  and `[DEPRECATED]` are part of the canon-governance process and must not be
  treated as final methodology or filled in with invented content.
- **Cumulative Pain and Cumulative Pleasure** are primary WFF outputs and must
  remain disaggregated by valence and intensity category. Do not introduce a
  single netted or weighted score as a primary output.

---

## Reporting a source conflict

If a registered source appears to conflict with the established WFF or existing
canon, **do not edit canon to resolve it.** Instead:

1. Open a **Source conflict report** Issue (see the Issue templates), and/or
2. Add an entry to `review/source_conflicts.md` following the format documented
   there.

A source conflict does not automatically imply that the WFF should change.
It may reflect differences in definitions, scope, evidence quality,
interpretation, or analytical level. Any substantive methodological response
requires the higher-level scientific process described above.

---

## Branching and pull requests

- **Direct commits to `main` are not allowed.** All changes go through a branch
  and a Pull Request.
- Use descriptive branch names, for example:
  - `draft/<topic>` for work in progress;
  - `review/<topic>` for content under formal review;
  - `docs/<topic>` for documentation and governance changes;
  - `fix/<topic>` for corrections.
- Keep Pull Requests small and reviewable. Fill in the Pull Request template.
- Canon and module changes are routed to the maintainers via `CODEOWNERS`.

---

## Questions

For terminology questions, suspected departures from the WFF, or requests for
clarification, please open an Issue so the discussion is visible and traceable.

A foundational methodological question may also be recorded as an Issue, but it
must be labelled and handled as a candidate for separate scientific review, not
as an ordinary public-repository correction.

For sensitive disclosures, follow `SECURITY.md`.
