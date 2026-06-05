# Australian Law — Version Controlled Reference

**Maintained by [The Pact Australia](https://thepactaustralia.com.au)**
*An advocacy group for independent politicians.*

---

## What This Is

This repository contains Australian federal legislation as plain text
Markdown files, maintained under version control. The `main` branch
always reflects current law. Every amendment is a merged pull request.

**This is the master reference against which The Pact Australia proposes
legislative changes.** A Pact Australia bill that amends an existing Act
is a pull request against this repository — showing exactly what changes,
in red and green, line by line.

## How To Read a Pact Australia Bill

Our proposed bills are at:
**[github.com/the-pact-australia/legislation](https://github.com/the-pact-australia/legislation)**

Each bill that amends an existing Act is a pull request (PR) against
this repository. Open the PR and you see:

```diff
- (a) the person is an Australian resident; and
+ (a) the person is an Australian citizen or the holder of a
+     permanent visa within the meaning of the Migration Act 1958; and
```

Red = removed from current law. Green = what replaces it.
No legal training required to understand what changes.

## How Amendments Work

When Parliament passes an amendment:

1. An automated check detects a new compilation on legislation.gov.au
2. A PR is opened showing the diff — exactly what Parliament changed
3. A reviewer confirms it matches the actual amendment
4. The PR is merged. `main` is updated.
5. Git history records the date and what changed.

## Structure

```
legislation/
├── federal/
│   ├── migration-act-1958.md
│   ├── social-security-act-1991.md
│   └── [one file per Act]
├── nsw/
├── vic/
└── [other states coming]
```

## File Format

Each Act is a single Markdown file. Frontmatter at the top:

```yaml
---
jurisdiction: federal
act-name: Migration Act 1958
series-id: C2004A01468
compilation-id: C2025C00XXX
compiled-date: 2025-06-01
source: https://www.legislation.gov.au/Series/C2004A01468
---
```

## Licence

All Commonwealth legislation is subject to Crown Copyright.
Reproduced under the Open Government Licence v3.0.
https://www.legislation.gov.au/Home/CopyrightPolicy

The Pact Australia contributions to this repository are licensed
under Creative Commons Attribution 4.0 International (CC BY 4.0).
