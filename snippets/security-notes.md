# Security Notes

```markdown
## 🔒 Security Notes

- Secrets are loaded from environment variables and are never committed.
- Authentication is verified before protected actions.
- Authorization is enforced at the resource or command boundary.
- Inputs, uploads, filenames, dimensions, and content types are validated.
- Expensive operations use rate limits, quotas, or abuse protection.
- External calls use explicit timeouts.
- Error responses avoid stack traces and private implementation details.
- Logs redact tokens, passwords, signed URLs, and personal data.
- Cleanup removes expired sensitive data.
```

Include only controls the project actually implements.
