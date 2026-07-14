<div align="center">

# 🐍 {{PROJECT_NAME}}

### {{PROJECT_SUBTITLE}}

</div>

<p align="center">
  {{TECH_BADGES}}
</p>

## 🚀 Why {{PROJECT_NAME}}

{{PROJECT_DESCRIPTION}}

## ✨ Features

- {{FEATURE_1}}
- {{FEATURE_2}}
- {{FEATURE_3}}
- {{FEATURE_4}}
- {{FEATURE_5}}

## 📦 Installation

### From source

```bash
git clone {{REPOSITORY_URL}}
cd {{REPOSITORY_FOLDER}}
python -m venv .venv

# Windows PowerShell
.venv\Scripts\Activate.ps1

# macOS / Linux
source .venv/bin/activate

pip install -e .
```

### From PyPI

```bash
pip install {{PACKAGE_NAME}}
```

Remove this section until the package is actually published.

## ▶️ Usage

```bash
{{CLI_NAME}} --help
```

### Examples

```bash
{{EXAMPLE_COMMAND_1}}
{{EXAMPLE_COMMAND_2}}
{{EXAMPLE_COMMAND_3}}
```

## 🗂️ Commands

| Command | Description |
|---|---|
| `{{CLI_NAME}} {{COMMAND_1}}` | {{COMMAND_1_DESCRIPTION}} |
| `{{CLI_NAME}} {{COMMAND_2}}` | {{COMMAND_2_DESCRIPTION}} |
| `{{CLI_NAME}} {{COMMAND_3}}` | {{COMMAND_3_DESCRIPTION}} |

## ⚙️ Configuration

```env
{{ENV_VARIABLE_1}}=
{{ENV_VARIABLE_2}}=
```

Or use:

```text
{{CONFIG_FILE_PATH}}
```

## 🧠 Design Notes

- Dry-run is the default for destructive operations
- Explicit flags are required before modifying files
- Exit codes distinguish success, validation failure, and runtime failure
- Paths are resolved without depending on the current shell directory
- Output supports both readable text and machine-readable JSON when useful

## 🏗️ Project Structure

```text
{{PROJECT_STRUCTURE}}
```

## 🧪 Development

```bash
pip install -e ".[dev]"
ruff check .
pytest
python -m build
```

## 🛡️ Safety

- Validate paths before reading or writing
- Refuse unsafe root or system locations
- Use backups for destructive transformations
- Preserve file encoding and line endings deliberately
- Avoid printing secrets
- Return non-zero exit codes on failure

## 📜 License

Licensed under the {{LICENSE_NAME}} License. See [LICENSE]({{LICENSE_PATH}}).
