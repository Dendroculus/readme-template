# Contributing

Thanks for helping improve this README template library.

This repository is a curated collection of reusable README templates, documentation snippets, and real README examples for different project types.

## What You Can Contribute

You can contribute:

- New README templates
- New documentation snippets
- Better example READMEs
- Badge groups for different tech stacks
- Setup instructions for common frameworks
- Grammar, formatting, and readability improvements
- Fixes for broken links, outdated examples, or Markdown rendering issues

## Repository Structure

```txt
templates/  → reusable README templates with placeholders
snippets/   → reusable README sections
examples/   → finished README examples based on real projects
```

## Template Guidelines

When adding a new template, place it in:

```txt
templates/
```

Use lowercase kebab-case file names:

```txt
backend-api.md
mobile-app.md
python-cli.md
machine-learning.md
data-analysis.md
```

A good template should include:

- Project title
- Short project description
- Features
- Tech stack
- Project structure
- Environment variables, if needed
- Local development instructions
- Testing instructions, if needed
- Security notes, if relevant
- License
- Contributors

Use placeholders for project-specific values:

```txt
{{PROJECT_NAME}}
{{PROJECT_SUBTITLE}}
{{PROJECT_DESCRIPTION}}
{{REPOSITORY_URL}}
{{FEATURES}}
{{TECH_STACK}}
{{ENV_VARIABLES}}
{{LOCAL_DEVELOPMENT}}
{{CONTRIBUTORS_TABLE}}
```

## Snippet Guidelines

When adding reusable sections, place them in:

```txt
snippets/
```

Examples:

```txt
docker.md
testing.md
deployment.md
api-endpoints.md
screenshots.md
```

Snippets should be:

- Small
- Focused
- Easy to copy
- Useful across multiple projects

## Example Guidelines

When adding finished examples, place them in:

```txt
examples/
```

Examples should look like completed real-world READMEs.

Before submitting examples, make sure they do not include:

- Real secrets
- Private API keys
- Private database URLs
- Expiring asset links
- Sensitive personal information

Examples should use placeholders for anything that should not be reused directly.

## Markdown Style

Please keep the style:

- Clean and readable
- Beginner-friendly
- Professional enough for portfolio projects
- Consistent with the existing templates
- Markdown-first, with HTML only when it improves layout
- No unnecessary complexity

## Commit Message Guide

Use this format:

```txt
type: short description
```

Examples:

```txt
docs: add backend API README template
feat: add mobile app README template
fix: correct broken markdown table
refactor: reorganize snippet structure
chore: update repository metadata
```

### Common Types

| Type | Use For |
|---|---|
| `docs` | README changes, templates, snippets, examples, contributing docs |
| `feat` | Adding a new template, snippet, example, or major documentation feature |
| `fix` | Fixing typos, broken links, broken Markdown, or incorrect examples |
| `refactor` | Reorganizing files or improving structure without changing meaning |
| `chore` | Repo maintenance, license updates, config files, metadata, cleanup |

For most changes in this repository, `docs:` is the best commit type.

## Branch Naming Guide

Use this format:

```txt
type/short-description
```

Examples:

```txt
docs/add-readme-template-library
docs/add-backend-api-template
feat/add-mobile-app-template
fix/broken-template-links
refactor/reorganize-snippets
chore/update-license
```

### Branch Types

| Type | Use For |
|---|---|
| `docs` | README changes, templates, snippets, examples, and contribution docs |
| `feat` | New template categories or major new documentation features |
| `fix` | Broken links, typos, incorrect examples, or Markdown rendering issues |
| `refactor` | File reorganization or structure cleanup without changing meaning |
| `chore` | Repo maintenance, license updates, config files, or metadata cleanup |

For most changes in this repository, use `docs/`.

## Pull Request Format

Use a clear PR title:

```txt
docs: add reusable README templates and documentation assets
```

Use bullet points in the PR body:

```md
* Add or update the first thing changed.
* Add or update the second thing changed.
* Add or update the third thing changed.

Summary:
Optional short note explaining why the change is useful.
```

The summary section is optional.

## Pull Request Checklist

Before opening a pull request:

- [ ] Files are placed in the correct folder
- [ ] Templates use placeholders where needed
- [ ] Examples do not include secrets or private data
- [ ] Markdown renders correctly
- [ ] Links are working
- [ ] Formatting matches the existing README style