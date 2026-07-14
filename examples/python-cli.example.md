# RepoSweep

A safety-first command-line utility that identifies generated files and optionally moves them into a timestamped backup.

## Features

- Dry-run by default
- Detects Python caches and generated logs
- Preserves repository-relative paths
- Creates timestamped backups
- Generates restoration metadata
- Returns meaningful exit codes

## Usage

```bash
reposweep scan .
reposweep apply . --backup .git/reposweep-backups
reposweep restore .git/reposweep-backups/20260714-170000
```

## Commands

| Command | Description |
|---|---|
| `scan` | Show candidates without changing files |
| `apply` | Move candidates into a backup |
| `restore` | Restore a previous backup |

## Safety

RepoSweep refuses filesystem roots, never follows paths outside the selected repository, and requires an explicit `apply` command before modifying files.

## Development

```bash
pip install -e ".[dev]"
ruff check .
pytest
python -m build
```
