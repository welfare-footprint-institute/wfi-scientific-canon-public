# Contributing to the WFI Scientific Canon

Thank you for your interest in the Welfare Footprint Institute (WFI) scientific canon.

## What this repository is

This repository is a **curated public representation** of the Welfare Footprint Framework (WFF): its established terminology, methodological commitments, module specifications, evidence standards, source registry, and review records.

It is not the ultimate scientific source of the WFF. That authority resides in:

1. the primary WFF methodological paper; and
2. any formal amendment or addendum jointly approved by Wladimir J. Alonso and Cynthia Schuck-Paim.

See `sources/wff_scientific_authority.md` and `sources/citation_policy.md`.

This repository is a **reference archive, not a software or product repository.** It does not contain application code, the Welfare Footprint Atlas, tool infrastructure, or operational systems. See `manifest.yaml` and `README.md` for the full scope.

Most contributions should improve how faithfully, clearly, consistently, and transparently the WFF paper, formal amendments, and approved internal canon are represented publicly.

---

## Contribution boundary: correcting the public repository versus revising the WFF

Two very different activities must not be conflated.

### 1. Public-repository corrections and clarifications

These are the normal subject of Issues and Pull Requests in this repository. They include cases where the public repository:

- misstates, oversimplifies, or inconsistently represents the WFF paper, an approved amendment, or the internal canon;
- uses deprecated, ambiguous, or non-canonical terminology;
- conflates distinct WFF analytical levels, modules, indicators, or metrics;
- omits an important qualification, status marker, source, or provenance note;
- presents a downstream tool convention as though it were part of the WFF;
- contains a typo, citation error, broken link, formatting problem, or unclear explanation;
- fails to preserve WFF commitments such as disaggregation by valence and intensity category.

The review question for these contributions is primarily:

> Does the proposed correction make the public repository more faithful to the WFF paper, formally adopted amendments, and approved internal canon?

### 2. Substantive revision of the WFF

Proposals to change the WFF's underlying concepts, analytical chain, module architecture, intensity-category definitions, methodological workflow, or other foundational commitments are exceptional and belong to a separate, higher-level scientific process.

Such a process may require:

- review of relevant scientific evidence and competing interpretations;
- formal discussion between Wladimir J. Alonso and Cynthia Schuck-Paim and, where appropriate, external experts;
- development or revision of the primary WFF methodological manuscript or another controlled scientific publication;
- explicit documentation of the decision, rationale, uncertainty, and scope;
- **joint approval by Wladimir and Cynthia** before the resulting change is represented as part of the WFF.

Neither author acting alone may unilaterally alter the foundational scientific content of the WFF.

If they do not agree, the proposed change remains unresolved and must not be represented as part of the WFF.

An Issue may record that a foundational methodological question exists and preserve its traceability. However, opening an Issue, accepting a discussion, or merging an ordinary Pull Request does **not** by itself revise the WFF.

Only after the higher-level scientific process reaches a jointly approved conclusion, and that conclusion is represented in the internal canon, should the public mirror be updated.

---

## Acceptable contributions

We welcome:

- **Typos** and obvious textual errors.
- **Citation fixes** consistent with `sources/citation_policy.md`.
- **Formatting corrections** and broken-link fixes.
- **Reports of departures from, or inconsistencies with, the WFF paper, approved amendments, or internal canon.**
- **Terminology questions** about WFF terms or definitions.
- **Source-conflict reports**.
- **Review notes** and proposed clarifications.
- **Proposed clarifications** that improve readability without changing scientific meaning.
- **Status and provenance corrections** where draft, provisional, deprecated, reviewed, or source information is missing or misleading.

For anything beyond a trivial correction, open an Issue first so the question can be examined before a Pull Request.

---

## Contributions requiring a different process

The following should not be inserted into the public canon through an ordinary Pull Request:

- a new WFF concept, intensity category, analytical level, or module;
- a redefinition of an established WFF term or methodological commitment;
- a restructuring of the WFF analytical chain or module workflow;
- a new aggregation or weighting rule presented as part of the WFF;
- a new, unreviewed scientific claim presented as settled WFF methodology;
- a substantive response to a source conflict that has not completed the joint scientific review process.

These questions may be documented for traceability, but they require the higher-level scientific process described above.

---

## Out-of-scope contributions

The following will not be accepted in this repository:

- Welfare Footprint **Atlas** or other product/tool code.
- **MCP servers**, agents, or tool infrastructure.
- **Validators or schemas**.
- **Full source documents** such as PDFs, DOCX files, manuscripts, or long source texts. Use registry metadata, citations, and short compliant excerpts instead.
- **Private or sensitive material** of any kind. See `SECURITY.md`.

---

## Review requirements for repository content

- **Changes to `canon/` and `modules/` require explicit review for fidelity to the WFF paper, formally adopted amendments, and approved internal canon.** Review is not authority to redesign the WFF through routine repository maintenance.
- **Substantive revisions of the WFF require joint approval by Wladimir and Cynthia through the separate scientific process.** They are not settled by an accepted Issue or ordinary merged Pull Request.
- **Source registry entries are evidence inputs, not automatically WFF authority.** A registered source does not change the WFF unless the joint scientific process formally adopts the change.
- **Placeholders and open questions are not settled.** Markers such as `[PLACEHOLDER — requires scientific review]`, `[OPEN QUESTION]`, `[DRAFT]`, and `[DEPRECATED]` must not be treated as final methodology or filled in with invented content.
- **Cumulative Pain and Cumulative Pleasure** remain disaggregated by valence and intensity category. Do not introduce a single netted or weighted score as a primary output.

---

## Reporting a source conflict

If a registered source appears to conflict with the WFF paper, a formal amendment, the internal canon, or this public mirror:

1. do not edit the WFF silently;
2. record the conflict in `review/source_conflicts.md` and, where useful, open an Issue;
3. determine whether the problem is a public-mirror fidelity error, an internal canon fidelity error, an interpretation problem, or a genuine candidate for amendment;
4. correct public fidelity errors through the ordinary public repository workflow;
5. route internal fidelity errors to the private canon workflow;
6. route genuine amendment candidates to the joint scientific process;
7. leave disagreements unresolved when joint approval has not occurred.

A source conflict does not automatically imply that the WFF should change.

---

## Branching and pull requests

- **Direct commits to `main` are not allowed.** All changes go through a branch and a Pull Request.
- Use descriptive branch names, for example:
  - `draft/<topic>` for work in progress;
  - `review/<topic>` for content under formal review;
  - `docs/<topic>` for documentation and governance changes;
  - `fix/<topic>` for corrections.
- Keep Pull Requests small and reviewable.
- Canon and module changes are routed to maintainers via `CODEOWNERS`.
- Repository approval confirms an accepted file change; it does not by itself amend the WFF.

---

## Questions

For terminology questions, suspected departures from the WFF, or requests for clarification, open an Issue so the discussion is visible and traceable.

A foundational methodological question may also be recorded as an Issue, but it must be handled as a candidate for separate joint scientific review, not as an ordinary public-repository correction.

For sensitive disclosures, follow `SECURITY.md`.
