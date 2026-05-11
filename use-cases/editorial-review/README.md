# Editorial Review

Editorial Review explores how Rubricks can structure editorial judgment into a repeatable review workflow for drafted content.

This use case is aimed at documents that need more than basic proofreading. The focus is on whether a draft is clear, internally consistent, appropriately sourced, aligned with editorial standards, and ready for publication or further revision.

## What This Use Case Explores

- turning editorial standards into explicit review criteria
- comparing a draft against context, references, and style expectations
- surfacing issues such as unsupported claims, ambiguity, tone mismatch, repetition, and structural gaps
- separating high-confidence edits from cases that need human editor judgment

## Proposed Workflow

The current folder structure supports a simple synthetic evaluation loop built around a concrete sample:

- `test-brightcart/review_context/` for audience, product, and research context
- `test-brightcart/references/` for source materials, style guidance, and review standards
- `test-brightcart/work_to_review/` for the summary and supporting artifacts under review
- `test-brightcart/document_index.json` for sample file indexing
- `test-brightcart/rubrick_mock_data.json` for mock Rubrick data used in the sample

## Current Sample

The current public sample is **BrightCart — Customer Interview Summary Review**.

It demonstrates a review workflow where a consultant pastes an AI-generated interview summary into Rubricks and checks whether the output is accurate, balanced, evidence-backed, and decision-ready.

The sample includes:

- review context about the product, customer, and interview goal
- reference materials that define what a strong summary should look like
- the AI-generated summary to review
- an original interview excerpt for evidence checking
- an example of a stronger revised summary direction

## Boundary

This use case is about structured editorial review support. It is not intended to replace final human editorial approval, especially where accuracy, legal risk, policy compliance, or publication judgment are involved.
