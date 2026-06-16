# Contributing to the WFI Scientific Canon

Thank you for your interest in the Welfare Footprint Institute (WFI) scientific
canon.

## What this repository is

This repository is a **scientific canon** — the version-controlled source of
truth for Welfare Footprint Framework (WFF) methodology, terminology, module
specifications, evidence standards, the source registry, and review notes.

It is a **reference archive, not a software or product repository.** It does
not contain (and will not accept) application code, the Welfare Footprint
Atlas, tool infrastructure, or operational systems. See `manifest.yaml` and
`README.md` for the full scope.

---

## Acceptable contributions

We welcome:

- **Typos** and obvious textual errors.
- **Citation fixes** (consistent with `sources/citation_policy.md`).
- **Formatting corrections** and broken-link fixes.
- **Terminology questions** about WFF terms or definitions.
- **Source-conflict reports** (see below).
- **Review notes** and proposed clarifications.
- **Proposed clarifications** that improve readability without changing
  scientific meaning.

For anything beyond a trivial correction, please open an issue first using one
of the issue templates so the change can be discussed before a pull request.

---

## Out-of-scope contributions

The following will not be accepted in this repository:

- Welfare Footprint **Atlas** or other product/tool code.
- **MCP servers**, agents, or tool infrastructure.
- **Validators or schemas**.
- **New, unreviewed scientific claims** inserted as canon.
- **Full source documents** (PDFs, DOCX, manuscripts, or long source texts).
  Use registry metadata, citations, and short compliant excerpts instead.
- **Private or sensitive material** of any kind (see `SECURITY.md`).

---

## Review requirements for scientific content

- **All changes to `canon/` and `modules/` require explicit human scientific
  approval.** Do not assume that an accepted issue or merged discussion settles
  a scientific question.
- **Source registry entries are evidence inputs, not automatically canon.**
  A registered source does not change canon until a reviewed change is approved.
- **Placeholders and open questions are not settled.** Markers such as
  `[PLACEHOLDER — requires scientific review]`, `[OPEN QUESTION]`, `[DRAFT]`,
  and `[DEPRECATED]` are part of the canon-governance process and must not be
  treated as final methodology or filled in with invented content.
- **Cumulative Pain and Cumulative Pleasure** are primary WFF outputs and must
  remain disaggregated by valence and intensity category. Do not introduce a
  single netted or weighted score as a primary output.

---

## Reporting a source conflict

If a registered source appears to conflict with existing canon, **do not edit
canon to resolve it.** Instead:

1. Open a **Source conflict report** issue (see the issue templates), and/or
2. Add an entry to `review/source_conflicts.md` following the format documented
   there.

Conflicts are resolved only through explicit human review.

---

## Branching and pull requests

- **Direct commits to `main` are not allowed.** All changes go through a branch
  and a pull request.
- Use descriptive branch names, for example:
  - `draft/<topic>` for work in progress;
  - `review/<topic>` for content under peer review;
  - `docs/<topic>` for documentation and governance changes;
  - `fix/<topic>` for corrections.
- Keep pull requests small and reviewable. Fill in the pull request template.
- Canon and module changes are routed to the maintainers via `CODEOWNERS`.

---

## Questions

For terminology or methodological questions, please open an issue rather than
emailing directly, so the discussion is visible and traceable. For sensitive
disclosures, follow `SECURITY.md`.
