# Citation Policy

Status: active
Last reviewed: 2026-05-12

This file defines the citation standards for WFI scientific canon outputs
and any materials that reference the Welfare Footprint Framework.

---

## Current primary citation

All references to the Welfare Footprint Framework methodology must cite:

> Alonso, W. J., & Schuck-Paim, C. (2025). *Welfare Footprint Framework:
> Methodological Foundations and Quantitative Assessment Guidelines.*
> Center for Welfare Metrics (São Paulo).
> https://doi.org/10.17605/osf.io/94bxs

This is the authoritative source for the full framework, module definitions,
notation standards, and quantitative assessment guidelines.

---

## Publication status

The core methodological paper describing the Welfare Footprint Framework is
currently **under review at *Animal Sentience***.

Until the peer-reviewed journal version is published, all materials — internal
documents, canon files, external reports, and agent outputs — should cite the
OSF preprint above.

The OSF preprint contains the complete, current framework. It is the correct
citation in this period.

---

## How to cite before Animal Sentience publication

Use the OSF preprint citation in full (see above).

- Do **not** cite unpublished internal drafts or working documents when the
  OSF preprint is the intended source.
- Do **not** omit the DOI. The DOI (`10.17605/osf.io/94bxs`) is the stable
  identifier that will continue to resolve after journal publication.
- When citing in canon files or review documents, use the format:
  `Alonso & Schuck-Paim (2025), https://doi.org/10.17605/osf.io/94bxs`

---

## Rule for updating citation after journal publication

When the *Animal Sentience* paper is published:

1. A new entry must be added to `sources/source_registry.yaml` with the
   journal citation and DOI.
2. The primary citation in this file must be updated to the journal version.
3. The OSF preprint entry must be retained in the registry with status
   `superseded-by-journal` and a note pointing to the journal DOI.
4. Any canon file that contains an inline citation must be reviewed and
   updated through a PR with explicit human approval.
5. This update requires a commit on a branch and approval before merging
   to `main` — it must not be done silently.

---

## Rule for not citing outdated internal drafts

When the OSF preprint (`10.17605/osf.io/94bxs`) is the intended reference:

- Do **not** substitute older internal working documents, slide decks,
  informal write-ups, or unpublished drafts.
- If a canon file currently references an internal document that has since
  been superseded by the OSF preprint, flag the discrepancy in
  `review/source_conflicts.md` and do not resolve silently.

---

## Secondary source citations

Secondary sources are listed in `sources/source_registry.yaml` with their roles,
citation details, canonical uses, and review status.

When citing a secondary WFI source, use the `preferred_format` recorded in the
registry entry for that source. Do not invent alternative citations.

Secondary sources should be cited only for the specific role assigned to them
in the registry. For example:
- use the Technical Definitions source for operational terminology;
- use the Pain Intensity Categories source for Annoying, Hurtful, Disabling,
  and Excruciating Pain;
- use the Positive Welfare source for Pleasure, Pleasure-Track, and Cumulative
  Pleasure;
- use the Metrics vs Indicators source for the distinction between welfare
  indicators and welfare metrics;
- use the AI Tools & Applications source for current WFI tool names and scopes.

If a secondary source appears to conflict with the primary WFF methodological
source or with existing canon, record the issue in `review/source_conflicts.md`
rather than resolving it silently.

---

## Conflict rule

If a source listed in `sources/source_registry.yaml` contradicts existing
canon wording and no explicit deprecation or terminology rule in this
repository already resolves it:

- Do **not** silently choose one version over the other.
- Create an entry in `review/source_conflicts.md` describing the conflict.
- Await explicit resolution by Wladimir J. Alonso or Cynthia Schuck-Paim.

---

## Agent instruction

Agents must not treat source documents as automatically merged canon.
Source documents inform canon updates; they do not replace the review process.
All canon changes derived from source material must go through a reviewed PR
with explicit human approval before reaching `main`.
