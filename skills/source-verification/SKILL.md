---
name: source-verification
description: Verify claims, manage citations, and maintain an auditable evidence database for strategic research.
---

# Source Verification

## Verification protocol

For every material claim, capture the exact wording, source title, publisher, original URL, publication date, retrieval date, geography, period, locator, and a short excerpt. Prefer the original publication over commentary.

Classify each item as:

- `verified fact`: directly supported within scope;
- `estimate`: calculated from cited inputs;
- `assumption`: chosen input not yet validated;
- `inference`: reasoned interpretation;
- `hypothesis`: testable but unconfirmed;
- `contradicted`: reliable evidence conflicts;
- `unknown`: the checked sources do not answer it.

Check units, denominators, sample, date, currency, population, and whether a source is describing revenue, GMV, users, bookings, or reach. For important claims, seek an independent corroborating source. A source URL alone is not evidence.

## Evidence register

Append to `templates/evidence-register.csv` or a copy of it. Do not delete contrary evidence. Use `qualifies` when scope differs and `contradicts` only when definitions and scope genuinely conflict.

## Output contract

Return a claim ledger with status, confidence rationale, citation, locator, and unresolved check. Explicitly list unsupported statistics and missing primary data. Never fabricate a citation, publication date, quote, or confidence percentage.
