# BrightCart — Customer Interview Summary Review

This synthetic sample demonstrates a simple Rubricks use case: reviewing a user-created or AI-generated summary.

## Persona

**Laura Bennett** is an independent product and operations consultant. She uses ChatGPT frequently to summarize customer interviews, discovery notes, and client documents. The summaries are often polished, but Laura still needs to check whether they are accurate, balanced, evidence-backed, and useful for decision-making.

## Scenario

Laura pasted an AI-generated summary of a customer discovery interview into Rubricks. The summary is about BrightCart's proposed **Smart Inventory Alerts** feature.

The AI summary looks credible, but it has issues:

- It overstates customer demand.
- It misses hesitation and objections.
- It lacks direct evidence.
- It recommends roadmap action too strongly.
- It does not clearly separate facts, interpretation, and recommendations.
- It does not include uncertainty.

Rubricks evaluates the summary against Laura's Rubrick: **Customer Interview Summary Review**.

## Folder Structure

```text
public/samples/brightcart-summary-review/
  references/
  work_to_review/
  review_context/
  document_index.json
  rubrick_mock_data.json
  README.md
```

## Files

### references/

These are the expert-defined standards and guidance used to create the Rubrick.

- `expert_q_and_a_seed.md` — Laura's guided Q&A answers. Demonstrates that Rubricks can start without formal reference documents.
- `summary_quality_standard.md` — A lightweight standard for high-quality customer interview summaries.
- `ai_summary_review_checklist.md` — Checklist for reviewing AI-generated summaries.

### review_context/

These files provide business context for evaluating the summary.

- `brightcart_product_context.md` — Product background and feature under consideration.
- `interview_goal.md` — Research goals and decision context.
- `customer_profile.md` — Customer profile and current workflow.
- `prior_research_themes.md` — Prior discovery themes relevant to the summary.

### work_to_review/

These are the artifacts Rubricks reviews.

- `pasted_ai_summary.md` — The AI-generated summary Laura pasted into Rubricks.
- `original_interview_excerpt.md` — Optional original source excerpt used for evidence checking.
- `revised_summary_expected.md` — Expected stronger summary direction after review.

## Product Concepts Demonstrated

- A user can paste any AI-generated text or summary for review.
- One work artifact can contain multiple review items.
- Rubricks can start from expert Q&A rather than formal documents.
- References, review context, and examples are useful but not required to begin.
- Starter cases are generated for expert validation, not treated as ground truth.
- Rubricks can output suggested edits, questions, work items, and export-ready fields.
