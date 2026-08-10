# Changesets

This directory contains changesets for the shadcn/ui project. Changesets are used to manage versioning and changelogs for the packages in this repository.

## Adding a changeset

To add a changeset, run `pnpm changeset` from the root of the repository. This will guide you through creating a changeset file that describes your changes.

## Changeset format

Each changeset is a markdown file with a frontmatter block that specifies the packages affected and the type of change (major, minor, patch).

Example:

```md
---
"@shadcn/ui": minor
---

Add support for custom themes.
```

## Reviewing changesets

When reviewing a pull request, check that the changeset is properly formatted and that the description is clear and concise.

## Publishing

Changesets are consumed by the changesets GitHub action, which will automatically create version bumps and publish packages to npm when changesets are merged into the main branch.

For more details, see [CONTRIBUTING.md](../CONTRIBUTING.md).