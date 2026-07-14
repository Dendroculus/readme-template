<div align="center">

# 🌸 SakuraBot

### A feature-oriented Discord bot for anime discovery, progression, games, and community interaction

</div>

## 🚀 Why SakuraBot

SakuraBot started as an anime image command and developed into a community platform with persistent progression, rendered profile cards, interactive games, polls, trading, and moderation utilities.

## 🎯 Features

### Anime discovery

- Anime metadata search
- High-resolution character image search
- Validation and duplicate filtering
- Provider fallback and cached results

### Progression and economy

- EXP, levels, coins, and title roles
- Rendered profile cards
- Server leaderboards
- Shop, inventory, consumables, and donation

### Games and community

- Trivia and character guessing
- Coin gambling
- Persistent polls
- Announcement modals
- Dynamic command help

## 🧠 Architecture Highlights

- Cogs remain thin
- Feature packages own workflows, views, and repositories
- PostgreSQL stores persistent state
- Optional Redis accelerates selected reads
- Rendering runs outside the event loop
- External APIs use shared asynchronous networking
- Persistent interactions recover after restarts
- Scheduled tasks refresh cached data safely

## 🔄 Command Flow

```text
Discord interaction
→ cog
→ feature workflow
→ repository, provider, or renderer
→ Discord view or response
```

## 🤖 Commands

| Command | Category | Description |
|---|---|---|
| `/anime <query>` | Search | Retrieve anime metadata |
| `/profile [user]` | Progression | Render a profile card |
| `/leaderboard` | Progression | Render top members |
| `/shop` | Economy | Open the shop |
| `/animequiz` | Games | Start a trivia game |
| `/poll` | Community | Create a persistent poll |

## ⚙️ Environment Variables

```env
DISCORD_TOKEN=
DATABASE_URL=

OWNER_ID=
REDIS_URL=
SEARCH_API_KEY=
```

## 🚀 Local Development

```bash
python -m venv .venv
pip install -r requirements.txt
python main.py
```

## 🛡️ Reliability

Scheduled loops are protected from duplicate startup, external requests use timeouts, stale cache can be used during provider outages, and graceful shutdown closes HTTP and database resources.
