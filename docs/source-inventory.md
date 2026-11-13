# Source inventory

Inspected on 2026-11-13. These are references and patterns, not bundled upstream code.

| Source | Exact path | Decision | License / reuse |
|---|---|---|---|
| [Anthropic skills](https://github.com/anthropics/skills) | `skills/pptx/SKILL.md`, `skills/xlsx/SKILL.md` | Reuse concepts for presentation QA and transparent spreadsheet modelling | Individual skills include `LICENSE.txt`; repository README states open-source skills are Apache 2.0. Verify the file before redistributing upstream text. |
| [Awesome Copilot](https://github.com/github/awesome-copilot) | `skills/build-evidence-map/SKILL.md`, `skills/build-evidence-map/scripts/validate.mjs`, `skills/build-evidence-map/references/map-schema.md` | Adopt evidence-map ideas; do not include script by default | Repository is MIT; preserve attribution if code is later copied. |
| [Awesome Copilot](https://github.com/github/awesome-copilot) | `skills/gtm-positioning-strategy/SKILL.md` | Adapt positioning and Crawl-Walk-Run concepts | MIT repository; this kit uses original concise guidance rather than copied prose. |
| [Awesome Copilot](https://github.com/github/awesome-copilot) | `skills/competitor-ad-intelligence/SKILL.md` | Considered for ad research; not included as a dependency | MIT repository; requires live web access and relies on public ad libraries. |
| [AnySearch skill](https://github.com/anysearch-ai/anysearch-skill) | `SKILL.md` | Rejected as a required dependency | Apache-2.0; sends queries and URLs to a third-party API and bundles network CLIs. Use only after separate provider review and explicit consent. |
| [Serenity skill](https://github.com/muxuuu/serenity-skill) | `SKILL.md` | Rejected as out of scope | MIT; investment/A-share focus does not fit this business research mission. |
