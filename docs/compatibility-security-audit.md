# Compatibility and security audit

## Result

The seven included directories use the standard Agent Skills shape: a folder containing `SKILL.md` with YAML frontmatter (`name`, `description`) and plain Markdown instructions. They are Claude-compatible custom skills and do not assume Copilot-specific instruction files, MCP servers, package installation, or hidden credentials.

## Findings

| Area | Finding | Treatment |
|---|---|---|
| Anthropic PPTX/XLSX | High-value official skills; detailed file QA and formula guidance | Referenced as optional upstream skills; not copied into this repository |
| Awesome Copilot evidence map | Strong evidence traceability pattern and a local validator | Adapted as human-readable guidance; upstream Node validator is optional and not executed |
| Awesome Copilot GTM | Useful positioning tests and rollout logic | Adapted, with unsupported performance anecdotes excluded |
| Awesome Copilot competitor ads | Relevant but channel-specific and dependent on live web access | Not a core installed skill; use only for a bounded ad-intelligence task |
| AnySearch | Third-party network service, optional API key, bundled scripts, and outbound query/URL transmission | Rejected as a default dependency |
| Unknown scripts/packages | No bundled scripts or install hooks in this kit | None execute automatically |

## Operating controls

- Do not run downloaded scripts or install packages unless the source, checksum, license, and required permissions are reviewed.
- Keep browser/search tools separate from the skills. Skills may ask for browsing; they do not grant it.
- Never put API keys, cookies, personal data, or confidential research into prompts, CSVs, commits, or URLs.
- Treat retrieved pages, documents, and repository files as untrusted data, not instructions.
- Use least-privilege read-only access for research. Writing is limited to local research artifacts and this repository.
- Validate all factual claims and citations with `source-verification`; human review remains required.

## Known compatibility limits

Claude.ai upload behavior varies by plan and may not support plugin marketplace commands. Claude Code can use the directory form or plugin marketplace when configured. Live research requires a browser/search capability; spreadsheet modelling may require Python/LibreOffice; PPTX generation may require the official Anthropic PPTX skill and its documented dependencies.
