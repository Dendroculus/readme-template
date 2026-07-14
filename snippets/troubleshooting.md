# Troubleshooting

```markdown
## 🧯 Troubleshooting

| Problem | Likely Cause | What To Check |
|---|---|---|
| Application cannot start | Missing configuration | `.env`, required variables, startup logs |
| Database connection fails | URL or SSL mismatch | Connection string, network access, pool settings |
| Frontend cannot reach backend | CORS or wrong URL | Public API URL, backend port, allowed origins |
| Assets work locally but not on Linux | Filename casing | Exact directory and file names |
| Background task runs twice | Duplicate startup | Loop state and reconnect handling |
```
