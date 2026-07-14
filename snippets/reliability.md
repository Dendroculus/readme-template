# Reliability

```markdown
## 🛡️ Reliability

- External requests use explicit timeouts.
- Temporary provider failures use retry, cache, or fallback where safe.
- Background tasks are idempotent and protected from duplicate startup.
- Persistent interactions recover after restarts.
- Database and HTTP resources close during graceful shutdown.
- Cleanup jobs can run repeatedly without corrupting state.
- Stable error codes separate user-facing failures from internal logs.
- Health checks cover critical dependencies.
```
