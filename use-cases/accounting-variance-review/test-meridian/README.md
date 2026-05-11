# Meridian Synthetic Sample Documents

This folder contains a synthetic sample document set for the Rubricks Meridian demo.

## Folder structure

```text
public/samples/meridian/
  references/
  work_to_review/
  review_context/
  document_index.json
  meridian_mock_data.json
  README.md
```

## Product model

Rubricks uses three distinct document roles.

### 1. Work to review

Folder:

```text
work_to_review/
```

These are documents or packets that contain review items Linda judges directly.

A work document can contain multiple review items.

Example:

`Preparer Variance Explanations` contains:
- Office Supplies variance explanation
- Marketing & Advertising variance explanation
- Software Subscriptions variance explanation
- Inbound Freight variance explanation
- Legal & Professional Fees variance explanation

Each review item remains traceable to its source work document.

### 2. Review context

Folder:

```text
review_context/
```

These files provide operational facts that help Linda review a selected item fairly.

Examples:
- NetSuite variance export
- NetSuite transaction detail
- BlackLine support status
- Bill.com AP invoice summary
- Close calendar
- FP&A forecast notes
- February prior-period context

### 3. Reference documents

Folder:

```text
references/
```

These are policies, guides, checklists, and notes Linda reviews against.

Examples:
- Capitalization Policy
- Expense Coding Guide
- Month-End Close Checklist

## Metadata files

### document_index.json

Lists the sample files and their metadata, including file paths, document roles, linked review items, linked guidance, context type, and facts provided.

### meridian_mock_data.json

Contains app-ready structured demo data, including:
- company
- expert
- Rubrick
- work documents
- review items
- review context
- guidance captured
- examples reviewed

## Core product sentence

Work to review is what Linda judges.  
Review context is what helps her judge it fairly.  
Reference documents are what she reviews against.
