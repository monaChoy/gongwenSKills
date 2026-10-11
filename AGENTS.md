# Repository Guidelines

## Project Structure & Module Organization

This repository develops Chinese document-writing skills for the maintainer's work. Prioritize workplace needs. The existing skill addresses state-owned enterprise contexts; do not infer the maintainer's role or industry.

- `README.md`: project overview and skill index.
- `skills/<skill-name>/SKILL.md`: skill metadata, workflow, and writing rules.
- `skills/<skill-name>/references/`: supporting templates and examples.

The current skill is `leader-style-briefing`. No application code, tests, or assets exist. Keep shared methods in base skills and business guidance in references. Split skills only for substantially different workflows or applicability. Avoid duplication; update the README index for new skills.

## Build, Test, and Development Commands

No build, dependency installation, or local server is required. Review Markdown directly.

- `rg --files skills`: list skill files and supporting references.
- `git diff --check`: check tracked changes for whitespace errors.
- `git status --short`: identify changed and untracked files; inspect new files separately because ordinary diffs omit them.

## Writing Style & Naming Conventions

Use lowercase, hyphen-separated directory names, such as `leader-style-briefing`. Keep the entry filename exactly `SKILL.md`. Preserve YAML front matter and use two-space indentation for nested YAML fields.

Write skill instructions and templates in clear, formal Chinese. Use descriptive Markdown headings, short paragraphs, and relative links such as `references/templates.md`. Preserve the distinction between verified facts, plans, recommendations, and unresolved information. Mark necessary factual gaps with `【待确认】`. User-provided formats and constraints take precedence over template defaults. No formatter or linter is configured.

## Validation Guidelines

No automated tests or coverage targets are configured. Verify front matter, relative links, supporting files, and workflow/template consistency. Use a fictional writing task to check usability. Review prose directly without code-review workflows.

## Commit & Pull Request Guidelines

There is no commit history establishing a convention. Use concise, imperative messages, for example `Add notice-writing template`. Keep changes focused on one skill or related documentation.

Pull requests should explain the purpose, affected files, and validation performed. Link relevant issues when available. Screenshots are unnecessary for Markdown-only changes.

## Public Repository Safety

De-identification is mandatory when authoring or updating skills. Skill text, templates, examples, filenames, attachments, and metadata must contain no real project names, identifiable organizations or people, contact details, internal addresses, credentials, or local absolute paths. Use placeholders such as `〔项目名〕` and `〔N〕`. Generalize distinctive dates, amounts, locations, and combinations that could identify a case. Retain methods, not internal source documents. Before delivery and publication, inspect every changed file, including untracked files; PR descriptions must record this check.
