# Track 01 – Standard Agent (Discord Bot)

Goal: spin up the Standard Agent as a Discord bot and handle a simple task.

## Setup
```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
cp .env.example .env  # fill DISCORD_BOT_TOKEN, JENTIC_API_KEY, etc.
make run
```

## Tasks

* [ ] Bot responds to `!ping`
* [ ] Bot executes a simple tool call via Jentic (e.g., fetch headlines)
* [ ] Post a short demo video/screenshot

## Troubleshooting

* Invalid token → re‑create bot token in Discord Dev Portal
* No response → check intents and channel permissions