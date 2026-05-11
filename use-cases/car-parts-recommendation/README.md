# Car Parts Recommendation

This use case explores how Rubricks can support expert review of an assistant-generated car part recommendation.

The assistant in this workflow is **Gigi**. Gigi proposes a likely part recommendation based on the vehicle information and the car's check engine code. An expert mechanic then reviews whether the recommendation is technically sound, sufficiently supported, and appropriate before any repair decision is made.

## Persona

The expert user is a mechanic reviewing Gigi's recommendation.

The mechanic is not just checking whether the suggested part sounds plausible. They need to decide whether the recommendation matches the code, fits the vehicle context, avoids common misdiagnosis patterns, and reflects how real repair work should be approached.

## Scenario

A user provides:

- vehicle information
- a check engine code
- a request for a likely part recommendation

Gigi returns a recommendation for what part may be involved.

The mechanic reviews that recommendation for issues such as:

- recommending a part too confidently from a code alone
- confusing a fault code with a confirmed failed component
- ignoring alternate causes
- missing vehicle-specific context
- suggesting a repair path that should start with diagnosis instead
- failing to explain uncertainty clearly

Rubricks helps structure that expert review so the output is more consistent, transparent, and useful.

## Structure

The use case folder can contain multiple test cases.

Each test case lives in its own folder, typically named `test-*`, and contains a specific vehicle scenario, mechanic-review workflow, and supporting materials.

## Current Tests

There is not yet a full public `test-*` sample under this use case.

## Current Folder Structure

```text
use-cases/car-parts-recommendation/
  data-sources/
    obd-trouble-codes.csv
```

## Files

### data-sources/

- `obd-trouble-codes.csv` — Reference list of OBD trouble codes and their descriptions. This supports code interpretation but does not, by itself, confirm the correct replacement part.

## Typical Test Contents

A test folder for this use case may include:

- `references/` for expert troubleshooting guidance or repair heuristics
- `review_context/` for vehicle details, symptoms, and code context
- `work_to_review/` for Gigi's recommendation and supporting rationale
- `document_index.json` for file indexing and metadata
- mock Rubrick data for app or demo use

## Product Concepts Demonstrated

- A parts recommendation can be reviewed as a judgment task, not just a retrieval task.
- A check engine code is an input to diagnosis, not automatic proof of a failed part.
- Expert review is necessary to distinguish likely causes from repair-ready conclusions.
- Rubricks can help evaluate whether Gigi's recommendation is evidence-based, appropriately qualified, and safe to act on.

## Boundary

This use case is about reviewing the quality of a part recommendation. It is not a substitute for vehicle inspection, proper diagnostics, manufacturer procedures, or a mechanic's final judgment.
