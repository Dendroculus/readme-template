# Runtime Flow Snippets

## Request Flow

```text
Client request
→ middleware
→ authentication and validation
→ application workflow
→ repository or provider
→ response formatter
→ client response
```

## Async Job Flow

```text
Upload initialization
→ direct storage upload
→ job creation
→ queue reservation
→ provider processing
→ result validation
→ status ready
→ retention cleanup
```

## Discord Interaction Flow

```text
Discord interaction
→ command cog
→ feature workflow
→ repository, provider, or renderer
→ Discord view or message
```

## Realtime Flow

```text
Domain change
→ event publisher
→ WebSocket transport
→ authenticated room
→ frontend provider
→ UI state update
```
