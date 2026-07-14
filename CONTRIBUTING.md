# Contributing

Thanks for helping improve this README template library.

## What You Can Contribute

- New project-type templates
- Focused documentation snippets
- Completed, sanitized example READMEs
- Better badge groups
- Cross-platform setup instructions
- Deployment and testing guidance
- Fixes for broken links, formatting, or inaccurate examples

## Repository Areas

```text
templates/  Reusable README skeletons with placeholders
snippets/   Small copy-ready sections
examples/   Completed examples without secrets
```

## Template Requirements

Use lowercase kebab-case filenames such as:

```text
backend-api.md
mobile-app.md
python-cli.md
machine-learning.md
```

A substantial template should normally provide:

- Project title and subtitle
- Why the project exists
- Grouped features
- Architecture highlights
- Runtime flows
- Project structure
- Commands or endpoints
- Environment variables
- Local development
- Testing
- Reliability and security notes
- Deployment when relevant
- License and acknowledgements

Use clear placeholders:

```text
{{PROJECT_NAME}}
{{PROJECT_SUBTITLE}}
{{PROJECT_DESCRIPTION}}
{{REPOSITORY_URL}}
{{FEATURE_GROUPS}}
{{PROJECT_STRUCTURE}}
{{ENV_VARIABLES}}
{{TEST_COMMANDS}}
```

Remove technology-specific assumptions unless the template is explicitly technology-specific.

## Snippet Requirements

Snippets should be:

- Focused on one documentation problem
- Easy to copy independently
- Shorter than a full template
- Explicit about which lines should be removed when unused
- Safe to publish without secrets

## Example Requirements

Examples should look like finished project READMEs, but must not include:

- Real secrets
- Private connection strings
- Personal access tokens
- Private infrastructure addresses
- Expiring links
- Sensitive user data

Public project names may be used as inspiration, but examples should remain reusable.

## Markdown Style

- Prefer clear Markdown over decorative HTML
- Use HTML only for alignment, badges, media sizing, or collapsible presentation
- Keep heading levels consistent
- Avoid enormous ungrouped feature lists
- Explain engineering decisions in plain language
- Use sentence case for headings and descriptions
- Verify rendering on GitHub before submitting

## Commit Messages

Conventional commit examples:

```text
docs(templates): add backend API template
docs(snippets): add deployment checklist
docs(examples): refresh Discord bot example
fix(markdown): correct broken relative links
refactor(structure): reorganize snippet index
```

## Pull Request Checklist

- [ ] Files are in the correct folder
- [ ] New templates use placeholders
- [ ] Examples contain no secrets
- [ ] Relative links resolve
- [ ] Markdown renders correctly
- [ ] Commands are syntactically valid
- [ ] Unused template sections were not left empty
- [ ] The root indexes were updated
