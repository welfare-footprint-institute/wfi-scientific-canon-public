# Citation and Scientific Authority Policy

Status: active  
Last reviewed: 2026-06-22

This file defines the citation standards and scientific-authority hierarchy for WFI materials that reference the Welfare Footprint Framework (WFF).

See also `sources/wff_scientific_authority.md`.

---

## Current primary citation and ultimate scientific authority

All references to the Welfare Footprint Framework methodology must cite:

> Alonso, W. J., & Schuck-Paim, C. (2025). *Welfare Footprint Framework:
> Methodological Foundations and Quantitative Assessment Guidelines.*
> Center for Welfare Metrics (São Paulo).
> https://doi.org/10.17605/osf.io/94bxs

This paper is the ultimate current scientific authority for the WFF: its full framework, module definitions, notation standards, and quantitative assessment guidelines.

Until a peer-reviewed journal version supersedes the OSF preprint, the OSF version is the controlling methodological source.

---

## Authority hierarchy

The hierarchy is:

1. **Primary WFF methodological paper** — ultimate current scientific authority.
2. **Formally adopted amendments or addenda** — valid only when jointly approved by Wladimir J. Alonso and Cynthia Schuck-Paim and recorded in a controlled scientific document.
3. **Internal scientific canon repository** — controlled, versioned operational representation of the paper and formally adopted amendments.
4. **Public scientific canon mirror** — curated public representation of the internal canon.
5. **Downstream tools and applications** — consumers of the paper, amendments, and canon representations.

The public repository does not independently create WFF scientific authority.

---

## Amendment rule

A substantive change to the WFF's foundational concepts, analytical chain, module architecture, intensity definitions, methodological workflow, or other core commitments requires:

- scientific rationale and supporting evidence;
- formal discussion between Wladimir J. Alonso and Cynthia Schuck-Paim;
- their explicit joint agreement;
- a dated amendment, addendum, correction, revised manuscript, or equivalent controlled scientific record;
- subsequent implementation in the internal canon before propagation to this public mirror and downstream artifacts.

Neither Wladimir nor Cynthia acting alone may unilaterally alter the foundational scientific content of the WFF.

If they do not agree, the proposed change remains unresolved and must not be represented as part of the WFF.

A public Issue or Pull Request may document a question or correct fidelity, but it does not itself create scientific authority.

---

## Publication status

The core methodological paper describing the Welfare Footprint Framework is currently **under review at *Animal Sentience***.

Until the peer-reviewed journal version is published, all materials — internal documents, canon files, external reports, and agent outputs — should cite the OSF preprint above.

The OSF preprint contains the complete, current framework and is the correct controlling citation in this period.

---

## How to cite before Animal Sentience publication

Use the OSF preprint citation in full.

- Do **not** cite unpublished internal drafts or working documents when the OSF preprint is the intended source.
- Do **not** omit the DOI. The DOI (`10.17605/osf.io/94bxs`) is the stable identifier that will continue to resolve after journal publication.
- When citing in canon files or review documents, use:
  `Alonso & Schuck-Paim (2025), https://doi.org/10.17605/osf.io/94bxs`

---

## Rule for updating citation after journal publication

When the *Animal Sentience* paper is published:

1. add the journal citation and DOI to `sources/source_registry.yaml`;
2. update the primary citation in this file to the journal version;
3. retain the OSF preprint entry with status `superseded-by-journal` and a note pointing to the journal DOI;
4. review all public canon files containing inline citations;
5. update them through a Pull Request with explicit approval;
6. do not make the transition silently.

This citation update does not itself change the scientific content of the WFF unless the published version differs substantively. Any substantive difference must be handled under the joint amendment rule above.

---

## Rule for not citing outdated internal drafts

When the OSF preprint (`10.17605/osf.io/94bxs`) is the intended reference:

- do **not** substitute older internal working documents, slide decks, informal write-ups, or unpublished drafts;
- if a public canon file references an internal document superseded by the OSF preprint, flag the discrepancy in `review/source_conflicts.md` and do not resolve it silently.

---

## Secondary source citations

Secondary sources are listed in `sources/source_registry.yaml` with their roles, citation details, canonical uses, and review status.

When citing a secondary WFI source, use the `preferred_format` recorded in the registry entry. Do not invent alternative citations.

Secondary sources should be cited only for their assigned role. For example:

- use the Technical Definitions source for operational terminology;
- use the Pain Intensity Categories source for Annoying, Hurtful, Disabling, and Excruciating Pain;
- use the Positive Welfare source for Pleasure, Pleasure-Track, and Cumulative Pleasure;
- use the Metrics vs Indicators source for the distinction between welfare indicators and welfare metrics;
- use the AI Tools & Applications source for current WFI tool names and scopes.

Secondary sources may clarify or operationalize parts of the WFF, but they do not override the primary methodological paper or a formally adopted amendment.

---

## Conflict rule

If a secondary source, public repository file, or downstream tool conflicts with the primary WFF paper or a formally adopted amendment:

- do not silently choose one version;
- record the conflict in `review/source_conflicts.md`;
- determine whether the conflict is a public-mirror fidelity error, an internal canon fidelity error, an interpretation problem, or a genuine candidate for scientific amendment;
- correct public fidelity errors through the ordinary repository workflow;
- route internal fidelity errors to the private canon workflow;
- route genuine amendment candidates to the joint scientific process;
- leave unresolved disagreements explicitly unresolved.

A source conflict does not automatically imply that the WFF should change.

---

## Agent instruction

Agents must follow this authority hierarchy.

They must not:

- treat the public or internal canon as superior to the WFF paper;
- infer that a merged Pull Request has amended the WFF;
- treat a secondary source as overriding the primary paper;
- invent an amendment when sources conflict.

Agents may propose fidelity corrections, identify conflicts, and reflect formally approved amendments. They must preserve unresolved status when joint approval has not occurred.
