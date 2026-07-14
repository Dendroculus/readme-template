<div align="center">

{{LANGUAGE_NAVIGATION}}

</div>

<p align="center">
  {{TECH_BADGES}}
</p>

<div align="center">

# ✨ {{PROJECT_NAME}}

### {{PROJECT_SUBTITLE}}

</div>

## 🚀 Why {{PROJECT_NAME}}

{{PROJECT_DESCRIPTION}}

- 🔍 {{HIGHLIGHT_1}}
- 📈 {{HIGHLIGHT_2}}
- 🎮 {{HIGHLIGHT_3}}
- ⚙️ {{HIGHLIGHT_4}}
- 🛡️ {{HIGHLIGHT_5}}

## 🎯 Features

### A) {{FEATURE_GROUP_1}}

1. **{{FEATURE_1}}** — {{FEATURE_1_DESCRIPTION}}
2. **{{FEATURE_2}}** — {{FEATURE_2_DESCRIPTION}}
3. **{{FEATURE_3}}** — {{FEATURE_3_DESCRIPTION}}

### B) {{FEATURE_GROUP_2}}

1. **{{FEATURE_4}}** — {{FEATURE_4_DESCRIPTION}}
2. **{{FEATURE_5}}** — {{FEATURE_5_DESCRIPTION}}
3. **{{FEATURE_6}}** — {{FEATURE_6_DESCRIPTION}}

### C) Community and administration

- {{COMMUNITY_FEATURE_1}}
- {{COMMUNITY_FEATURE_2}}
- {{ADMIN_FEATURE_1}}
- {{ADMIN_FEATURE_2}}

## 🎥 Command Previews

{{SCREENSHOTS_OR_DEMO}}

## 🧠 Architecture Highlights

- **Thin cogs** register commands, validate Discord context, and orchestrate responses
- **Feature packages** own workflows, services, views, repositories, and integrations
- **Shared core packages** provide reusable Discord, logging, rendering, and persistence infrastructure
- **Persistent storage** keeps progression, economy, polls, or other state across restarts
- **Dedicated views** isolate button, select, and modal interaction state
- **Scheduled tasks** handle maintenance, synchronization, refresh, or presence behavior
- **Recovery workflows** restore persistent interactions after restarts
- **External clients** use timeouts, rate limits, caching, validation, and fallback

Delete architecture points that do not match the project.

## 🔄 Main Runtime Flows

### Command flow

```text
Discord interaction
→ thin cog or command handler
→ feature workflow or service
→ repository, external provider, or renderer
→ response formatter or view
→ Discord response
```

### Optional background-job flow

```text
Discord command
→ job validation
→ queue or worker
→ processing service
→ result storage
→ Discord delivery
```

Keep this only when the bot really uses a worker or queue.

### Optional persistent-view recovery

1. Interaction state is stored with message and channel identifiers
2. Bot reconnects or restarts
3. Recovery workflow loads active records
4. Expired records are finalized or removed
5. Valid views are attached to existing messages

## 🏗️ Project Structure

```text
{{PROJECT_STRUCTURE}}
```

## 🤖 Commands

| Command | Category | Description |
|---|---|---|
| `/{{COMMAND_1}}` | {{CATEGORY_1}} | {{COMMAND_1_DESCRIPTION}} |
| `/{{COMMAND_2}}` | {{CATEGORY_2}} | {{COMMAND_2_DESCRIPTION}} |
| `/{{COMMAND_3}}` | {{CATEGORY_3}} | {{COMMAND_3_DESCRIPTION}} |

## 🏗️ Architecture & Stack

- **Discord framework — {{DISCORD_FRAMEWORK}}**  
  {{DISCORD_FRAMEWORK_DESCRIPTION}}

- **Database — {{DATABASE_STACK}}**  
  {{DATABASE_DESCRIPTION}}

- **Optional cache — {{CACHE_STACK}}**  
  {{CACHE_DESCRIPTION}}

- **Rendering or workers — {{PROCESSING_STACK}}**  
  {{PROCESSING_DESCRIPTION}}

- **External integrations — {{EXTERNAL_APIS}}**  
  {{EXTERNAL_APIS_DESCRIPTION}}

## ⚙️ Environment Variables

```env
# Required
DISCORD_TOKEN=
DATABASE_URL=

# Optional
OWNER_ID=
REDIS_URL=
LOG_LEVEL=INFO
{{OPTIONAL_API_KEY}}=
{{OPTIONAL_API_SECRET}}=
```

## 🚀 Local Development

```bash
git clone {{REPOSITORY_URL}}
cd {{REPOSITORY_FOLDER}}

python -m venv .venv

# Windows PowerShell
.venv\Scripts\Activate.ps1

# macOS / Linux
source .venv/bin/activate

pip install -r requirements.txt
python {{ENTRYPOINT}}
```

### Discord application setup

1. Create a Discord application and bot
2. Enable only the privileged intents the bot requires
3. Configure the OAuth scopes and permissions
4. Add the token to `.env`
5. Invite the bot to a development server
6. Verify slash-command synchronization

## 🧪 Testing and Quality

```bash
ruff check .
pytest
python -m compileall -q .
```

Recommended smoke tests:

- Extension import
- Command synchronization
- Database initialization
- External-provider fallback
- Persistent-view recovery
- Asset and font validation
- Graceful HTTP and database shutdown

## 🚀 Deployment

- Store the token and database URL as platform secrets
- Use a persistent database
- Include local assets in the image or configure an asset mount
- Install browser runtimes when Playwright is used
- Configure a separate worker only when the architecture requires one
- Confirm graceful shutdown closes HTTP, database, cache, and worker resources

## 🛡️ Reliability and Security

- Tokens never appear in source control or logs
- Admin commands enforce Discord permissions or an allowlist
- External requests use timeouts and rate limits
- Scheduled loops are idempotent and do not start twice
- Views isolate per-session state
- Persistent records are recovered or expired safely
- Heavy rendering runs outside the event loop
- Local assets use portable paths
- Failed providers use cache, fallback, or clear user-facing errors

## 🧯 Troubleshooting

| Problem | Check |
|---|---|
| Slash commands are missing | Sync logs, invite scopes, application ID |
| Presence or maintenance task crashes | `@tasks.loop` decorator and duplicate starts |
| Database is unavailable | Connection URL, SSL, pool initialization |
| Images or fonts are missing | Portable asset root and Linux filename casing |
| External search returns nothing | Credentials, provider status, fallback path |

## 🤝 Contributing

Test the affected command flow and include screenshots only when visible output changes.

## 📜 License

Licensed under the {{LICENSE_NAME}} License. See [LICENSE]({{LICENSE_PATH}}).

## 🙏 Acknowledgements

- {{ACKNOWLEDGEMENT_1}}
- {{ACKNOWLEDGEMENT_2}}

## 👤 Author

{{AUTHOR_SECTION}}
