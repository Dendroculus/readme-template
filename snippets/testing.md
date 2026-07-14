# Testing and Quality

## Copy-ready section

```markdown
## 🧪 Testing and Quality
```

```bash
# Python
ruff check .
pytest
python -m compileall -q .

# JavaScript
npm run lint
npm test
npm run build
```

Test layers:

- **Unit tests** for isolated domain rules
- **Integration tests** for database and provider boundaries
- **End-to-end tests** for important user flows
- **Smoke tests** for imports, startup, and configuration
- **Manual tests** only for flows that cannot be automated reliably
