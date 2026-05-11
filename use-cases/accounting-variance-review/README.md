# Accounting Variance Review

This use case explores how Rubricks can structure expert review of monthly accounting variance reports and the explanations prepared during the close process.

The goal is not just to identify whether a variance is above a threshold. The goal is to review whether the explanation is complete, supported, correctly classified, aligned with policy, and ready for inclusion in management reporting.

## What This Use Case Explores

- reviewing variance explanations as a judgment task, not just a threshold check
- comparing preparer explanations against accounting policy, close rules, and transaction support
- surfacing issues such as weak root-cause analysis, missing support, miscoding, prepaid treatment, capitalization concerns, and unresolved close items
- helping accounting leaders decide what is ready for sign-off and what needs follow-up

## Structure

The use case folder can contain multiple test cases.

Each test case lives in its own folder, typically named `test-*`, and contains a specific company scenario, persona, and review packet.

## Current Tests

- `test-meridian/` — Linda, the Corporate Controller at Meridian Apparel, reviews the March 2026 variance report prepared by the accounting team.

## Typical Test Contents

A test folder for this use case may include:

- `references/` for accounting policies, close checklists, and coding guidance
- `review_context/` for ERP exports, transaction detail, support status, and planning context
- `work_to_review/` for the variance packet and preparer explanations
- `document_index.json` for file indexing and metadata
- mock Rubrick data for app or demo use

## Boundary

This use case supports controller and accounting-review workflows. It does not replace final accounting judgment, required support review, or company policy approval.
