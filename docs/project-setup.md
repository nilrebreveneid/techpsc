# GitHub Project Setup For TECHPSC

Create one GitHub Project called `TECHPSC Master Board`.

## Fields

Add these fields to the project:

- `Status` as single select
  - Backlog
  - Todo
  - In Progress
  - Review
  - Blocked
  - Done
  - Paid
  - Rejected
- `Category` as single select
  - Development
  - Design
  - Documentation
  - Operations
  - Outreach
  - Research
  - Finance
- `Priority` as single select
  - Low
  - Medium
  - High
  - Urgent
- `Points` as number
- `Budget` as number
- `Payment Status` as single select
  - Pending
  - Under review
  - Approved
  - Paid
  - Rejected
- `Submission Link` as text
- `Proof Link` as text
- `Approved By` as text
- `Due Date` as date
- `Submitted On` as date

## Views

Create these views:

### 1. Contributor Board

Layout: Board  
Group by: `Status`  
Filter: `Category` is not `Finance`

Use this for daily work management.

### 2. Finance Ledger

Layout: Table  
Filter: `Category` is `Finance`

Show these columns:

- Title
- Assignees
- Budget
- Payment Status
- Proof Link
- Approved By
- Due Date

### 3. Submission Queue

Layout: Table  
Filter: `Status` is `Review`

Use this to process contributor submissions.

### 4. Leadership Dashboard

Layout: Table or Roadmap  
Show:

- Priority
- Points
- Budget
- Due Date
- Status

## Automation

Enable built-in project workflows:

- auto-add issues from the repository
- auto-add pull requests from the repository
- auto-archive items when closed or marked done

## Mapping from your current spreadsheets

When migrating spreadsheet rows, use this mapping:

- contributor row -> contributor task issue
- submission entry -> pull request or update issue
- finance row -> finance record issue
- points total -> project `Points` field
- amount or expense -> project `Budget` field
- receipt or proof link -> project `Proof Link` field

## Governance rules

- No work is counted without an issue.
- No points are awarded without review.
- No finance item is considered complete until `Payment Status` is `Paid`.
- Every submission should link back to an issue.
