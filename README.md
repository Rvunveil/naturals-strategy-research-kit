# Naturals Strategy Research Kit

A lightweight, Claude-compatible Agent Skills stack for the **Naturals NxtGen Innovators Challenge 2026**. It is designed to support disciplined research into bridal beauty discovery, booking, marketplaces, platform economics, growth, and execution without starting the Naturals market research itself.

## Skill inventory

| Skill | Purpose | Claude compatibility |
|---|---|---|
| `deep-research` | Evidence-driven web research and synthesis | Native custom skill |
| `market-intelligence` | Industry, competitor, segmentation, and TAM/SAM/SOM analysis | Native custom skill |
| `business-strategy` | Consulting frameworks, platform strategy, options, and GTM | Native custom skill |
| `financial-modelling` | Revenue, unit economics, scenarios, and sensitivities | Native custom skill |
| `source-verification` | Claim checking and a durable evidence register | Native custom skill |
| `presentation-storytelling` | Executive narrative, slide logic, and visualisation | Native custom skill |
| `critical-review` | Sceptical judge review of assumptions, economics, and recommendations | Native custom skill |

The skills share one research standard: never invent facts, label estimates and assumptions, preserve source URLs and dates, prioritise Indian context, and expose missing data.

## Install in Claude Code

From Claude Code:

```text
/plugin marketplace add Rvunveil/naturals-strategy-research-kit
/plugin install naturals-strategy-research-kit@naturals-strategy-research-kit
```

For a local checkout, copy the seven directories under `skills/` into the location used by your Claude Code custom skills setup. The portable ZIP is `dist/naturals-strategy-research-kit.zip`.

Claude.ai custom-skill upload support varies by plan and product surface. Upload the ZIP when the custom skills UI accepts archives; otherwise upload each skill directory separately.

## Recommended workflow

1. Start with `deep-research` to frame the question and collect dated primary sources.
2. Use `source-verification` continuously; maintain `templates/evidence-register.csv`.
3. Use `market-intelligence` for market structure, competitors, customer segments, and market sizing.
4. Use `business-strategy` to convert evidence into strategic choices and an executable GTM.
5. Use `financial-modelling` to test monetisation, unit economics, scenarios, and sensitivities.
6. Use `critical-review` as a separate challenge pass before accepting a recommendation.
7. Use `presentation-storytelling` last to build the competition narrative and deck.

## Tool boundary

Skills provide operating instructions; they do not provide live browsing, filings, databases, or a finance engine. Claude needs access to a web search/browser tool for current research and optionally spreadsheet/Python tooling for models and charts. Never place API keys in this repository or in prompts.

## Provenance and audit

See:

- `docs/compatibility-security-audit.md` — inspected sources, compatibility decisions, licensing, dependencies, and security findings.
- `docs/source-inventory.md` — original repositories and exact paths reviewed.
- `docs/recommended-workflow.md` — operating sequence and output contracts.
- `templates/` — reusable evidence, sizing, modelling, and slide-story templates.

## Scope limits

This kit does not contain Naturals market findings, proprietary data, paid reports, browser credentials, or an automated market-data connector. It also does not guarantee that a source is accurate: it makes the research trail and uncertainty explicit for human review.

## License

The custom skill text and templates in this repository are released under the MIT License. Referenced upstream projects retain their own licenses; this repository does not redistribute their upstream source files.
