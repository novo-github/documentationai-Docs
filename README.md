# Novo AI Documentation

This repository is the source for the English and German Watchmen Platform documentation published with Documentation.AI.

## Repository structure

- `en/` and `de/` contain the canonical localized documentation.
- `platform-intro/pages/` contains screen-level reference pages.
- `platform-intro/workflows/` contains task-focused procedures.
- `help-center/` contains orientation and symptom-based troubleshooting.
- `api-reference/openapi.yaml` is the single source of truth for the public REST API reference.
- `documentation.json` controls navigation, branding, redirects, and OpenAPI integration.

Keep the English and German trees structurally aligned. Do not create new root-level editorial pages.

## Work with MDX in VS Code

There are two preview levels:

1. **Quick content preview:** use `Ctrl+Shift+V` or `Ctrl+K V` in VS Code. This is useful for reviewing headings, prose, lists, tables, links, and code blocks.
2. **Authoritative rendered preview:** push a branch and open the Documentation.AI branch or pull-request preview. Use this preview to verify Cards, Columns, Tabs, Steps, Callouts, navigation, OpenAPI output, theme behavior, and responsive layout.

The VS Code Markdown preview does not reproduce the Documentation.AI component renderer, navigation, or site theme. Do not treat it as final visual QA.

## Edit content safely

1. Create a documentation branch.
2. Edit the English and German equivalents together.
3. Keep `documentation.json` aligned with added, moved, or removed pages.
4. Use absolute internal links such as `/en/platform-intro/pages/machines`.
5. Review the Git diff.
6. Push the branch and inspect the Documentation.AI preview before merging.

## Editorial ownership

- Page references own screen purpose, visible content, available actions, entities, and empty states.
- Workflows own prerequisites, ordered task steps, decision points, expected results, and troubleshooting.
- Help Center pages orient users and diagnose symptoms; they link to canonical workflows rather than repeating procedures.
- OpenAPI owns endpoint paths, authentication, schemas, examples, and response definitions.
- Changelog entries contain only approved release facts.

Use **Watchmen Platform** in English and **Watchmen-Plattform** in German. Use formal `Sie` throughout German user-facing content.

## Required review

- Product owners approve introductions and capability descriptions.
- Support owners approve Help Center guidance and support channels.
- Backend owners approve API coverage, base URLs, authentication behavior, schemas, examples, and version metadata.
