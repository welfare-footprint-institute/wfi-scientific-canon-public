# Security and Sensitive-Information Reporting

This repository is a **scientific canon**, not a software product. It should
**not** contain executable code, services, MCP servers, validators, product
infrastructure, or credentials. As such, traditional software vulnerabilities
are not expected here.

The more relevant concern for this repository is the **accidental disclosure of
sensitive information.**

## What to report

Please report privately if you notice any of the following in the repository,
its history, issues, or pull requests:

- Secrets, tokens, API keys, passwords, or other credentials.
- Private or unpublished links (internal Notion/Drive links, private drafts).
- Unpublished documents (manuscripts, PDFs, DOCX, slide decks) that should not
  be public.
- Private email addresses or contact lists.
- Funder, grant, or financial details.
- HR / personnel / contractor material.
- Legal or board-sensitive material.
- Any other private or sensitive content that should not be world-readable.

## How to report

- **Do not open a public issue or pull request for a sensitive disclosure.**
  A public issue would draw attention to the very content that needs to be
  contained.
- Report privately by email to:

  **wladimir.j.alonso@welfarefootprint.org**

- Alternatively, if enabled for this repository, use GitHub's **private
  security advisory** mechanism.

Please include enough detail to locate the content (file path, commit, issue,
or pull request reference) without restating the sensitive material itself in a
public channel.

## Response

A maintainer will review the report, assess exposure (including git history,
which remains visible once published), and take appropriate corrective action.
Disclosures will be handled with discretion.

## Scope reminder

If you are proposing to add code, services, validators, schemas, or tool
infrastructure to this repository, please note this is **out of scope** — see
`CONTRIBUTING.md` and `manifest.yaml`. Such systems belong in their own
repositories with their own security policies.
