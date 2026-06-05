# Contributing

## Reporting Errors

If you find an error in how an Act has been transcribed or converted:

1. Open an Issue describing the discrepancy
2. Reference the relevant section number
3. Provide the correct text from legislation.gov.au

## Proposing Amendments (Pact Australia Bills)

All legislative proposals from The Pact Australia are made as
pull requests against this repository. Each PR:

- Names the Pact Australia Bill that proposes the change
- Links to the full bill text in the legislation repository
- Shows the exact diff against current law

## Branch Naming

Parliamentary amendments:
`amendment/[act-slug]/[amending-act-short-name]-[year]`

Pact Australia bills:
`pact/[bill-number]-[short-description]`

## Adding New Acts

To add a Commonwealth Act not yet in this repository:

1. Find the Act at legislation.gov.au
2. Note the Series ID from the URL
3. Download the current compilation as HTML
4. Convert to Markdown following the format in any existing Act file
5. Add the frontmatter header
6. Submit a PR with title: `Add: [Act Name]`
