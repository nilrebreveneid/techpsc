# How To Manage TECHPSC On GitHub

This is the operating guide for running TECHPSC through GitHub.

## What to use for what

- Use `Contributor Task` issues for new work assignments.
- Use `Finance Record` issues for payments, reimbursements, budgets, and expense approvals.
- Use `Weekly Update` issues for weekly progress reporting.
- Use pull requests for submissions and reviews.
- Use the GitHub Project to track points, budget, status, proof links, and approvals.

## Daily management

Every day, check these things:

1. Open the `Contributor Board` view.
2. Move new work into the right status.
3. Check `Submission Queue` for items in review.
4. Review pull requests and approve or request changes.
5. Update issue status and project fields.

## Weekly management

Every week, do this:

1. Ask each contributor to submit a `Weekly Update` issue.
2. Review completed work against linked pull requests.
3. Update `Points` only after review is complete.
4. Review all finance issues with `Pending` or `Under review` status.
5. Close finished issues and archive completed project items.

## Monthly management

At the end of each month:

1. Filter the GitHub Project by each contributor.
2. Sum completed `Points`.
3. Review finance totals from items with category `Finance`.
4. Export or summarize work done, submissions, and payments.

## How contributors should work

Contributors should follow this flow:

1. Get assigned an issue.
2. Start the work and move it to `In Progress`.
3. Submit the work through a pull request or update issue.
4. Wait for review.
5. After approval, the issue is marked done and points are updated.

## How finance should work

Finance leads should follow this flow:

1. Open a `Finance Record` issue for each expense or payment item.
2. Fill in amount, requester, date, and proof.
3. Track approval in `Payment Status`.
4. Mark an item complete only when it is actually paid.

## Suggested admin rules

- No task should exist without an issue.
- No points should be awarded without a linked submission or review.
- No payment should be marked complete without proof.
- Every pull request should link to an issue.
- Keep finance records in a private repository if the data is sensitive.

## First setup checklist

- Create the `TECHPSC Master Board` project
- Add all custom fields from `docs/project-setup.md`
- Upload the current contributor and finance sheets
- Convert the spreadsheet rows into issues
- Add actual contributor GitHub usernames
- Replace `CODEOWNERS.example` with real owners when roles are finalized
- Make the repository private if finance data should not be public
- Turn on branch protection for `main`
