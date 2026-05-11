# Editorial Review

Editorial Review explores how Rubricks can structure editorial judgment into a repeatable review workflow for drafted content.

This use case is aimed at documents that need more than basic proofreading. The focus is on whether a draft is clear, internally consistent, appropriately sourced, aligned with editorial standards, and ready for publication or further revision.

## What This Use Case Explores

- turning editorial standards into explicit review criteria
- comparing a draft against context, references, and style expectations
- surfacing issues such as unsupported claims, ambiguity, tone mismatch, repetition, and structural gaps
- separating high-confidence edits from cases that need human editor judgment

## Structure

The use case folder can contain multiple test cases.

Each test case lives in its own folder, typically named `test-*`, and contains a specific persona, document set, and review scenario.

## Current Tests

- `test-brightcart/` — Laura Bennett reviews an AI-generated customer interview summary for the BrightCart product context.

## Typical Test Contents

A test folder for this use case may include:

- `references/` for style standards, checklists, or expert seed material
- `review_context/` for audience, product, research, or assignment context
- `work_to_review/` for the summary, memo, article, or other drafted output under review
- `document_index.json` for file indexing and metadata
- mock Rubrick data for app or demo use

## Boundary

This use case is about structured editorial review support. It is not intended to replace final human editorial approval, especially where accuracy, legal risk, policy compliance, or publication judgment are involved.
