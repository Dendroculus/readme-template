# README Template Library v2 Upgrade Guide

This release aligns the template library with the documentation patterns used by larger, feature-oriented projects.

## What Changed

- Standardized substantial templates around **why → features → architecture → flows → setup → quality**
- Added Backend API and Python CLI templates
- Reworked the Discord template so background workers are optional
- Expanded AI documentation for queues, polling, signed URLs, provider fallback, and cleanup
- Added reusable snippets for architecture, reliability, runtime flows, deployment, testing, and troubleshooting
- Added completed examples for AI, Discord, full-stack, API, and CLI projects
- Added explicit guidance for required versus optional environment variables
- Added cross-platform local-development examples

## Migrating an Existing README

1. Keep your current project title, description, badges, and screenshots.
2. Add a concise **Why This Project** section.
3. Group features by user-facing domain.
4. Separate **Architecture Highlights** from **Architecture & Stack**.
5. Document one or two important runtime flows.
6. Verify the project tree and environment variables against the current code.
7. Add testing, reliability, security, and deployment sections only where relevant.
8. Remove screenshots only when they are outdated, duplicated, or no longer referenced.

## Compatibility

Existing v1 templates remain conceptually compatible. The v2 templates mostly add structure and optional sections rather than forcing a new technology stack.
