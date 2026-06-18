# Public Canon Mirror Policy

This repository is the curated public mirror of the internal WFI scientific canon repository.

## Intentional duplication

Some files in this repository intentionally duplicate or closely mirror files in
`welfare-footprint-institute/wfi-scientific-canon`.

This duplication is not an audit defect. It is part of the public/private canon
architecture:

- the private canon is the internal working and review repository;
- the public canon is the curated public reference snapshot;
- public files may mirror internal files when the mirrored content is appropriate
  for public release.

## Source of truth

The internal repository remains the upstream working source for canon development.
This public repository is a curated mirror, not an independent methodological
source.

If public and private canon files diverge, the divergence should be interpreted
as one of the following:

1. intentional public redaction or simplification;
2. publication lag;
3. unresolved sync issue requiring review.

It should not be silently resolved.

## Sync policy to define

TODO: Define the operational sync policy, including:

- which files are mirrored automatically, manually, or never;
- who approves public mirror updates;
- how public redactions are recorded;
- how divergence between private and public files is detected;
- how often the public mirror should be reviewed;
- where sync decisions are logged.

## Audit note

Future repository audits should not flag private/public canon duplication as
unwanted duplication unless the duplicated content lacks an explicit mirror
rationale or has drifted without documentation.
