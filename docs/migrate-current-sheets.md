# Migrating The Current TECHPSC Sheets

This document explains how the two current spreadsheets should be moved into GitHub.

## Source files

- `TechPSC_Contributors_Points_v2.xlsx`
- `TechPSC_Finance_Tracker.xlsx`

## Migration target

Move the spreadsheets into GitHub in this form:

### Contributor points workbook

Each contributor task or submission should become either:

- a `Contributor Task` issue
- a pull request linked to that issue
- a `Weekly Update` issue for reporting-only rows

Map common columns like this:

- contributor name -> assignee or issue body field
- task title -> issue title
- task description -> issue body
- points -> `Points` project field
- submission link -> `Submission Link` field
- submission date -> `Submitted On`
- status -> `Status`
- reviewer -> `Approved By`

### Finance workbook

Each finance line should become a `Finance Record` issue.

Map common columns like this:

- date -> `Due Date` or issue body
- requester -> assignee or issue body field
- amount -> `Budget`
- category -> `Category` set to `Finance`
- approval state -> `Payment Status`
- receipt or invoice link -> `Proof Link`
- approver -> `Approved By`
- notes -> issue body

## Recommended migration order

1. Upload the sheets into this repo as CSV or Excel files.
2. Create the GitHub Project and custom fields.
3. Import contributor rows as issues.
4. Import finance rows as finance issues.
5. Link all future submissions through pull requests.

## Current limitation

The current thread cannot directly read the local Excel files, so the row-by-row migration has not yet been completed. Once the workbook data is available in the repository as CSV, pasted tables, or accessible workbook files, the data can be turned into actual GitHub issues and project items.
