# 00 – Install & Setup (10 mins)

## 1) Prereqs
- Git, Python 3.10+ (or 3.12), Node (optional)
- A terminal and a code editor

## 2) Create a clean Python env
```bash
python -m venv .venv && source .venv/bin/activate
pip install --upgrade pip
````

## 3) Jentic auth & environment

* Create a free account at [https://app.jentic.com](https://app.jentic.com)
* Get your **Agent API key** (see docs quickstart)
* Create `.env` in your track folder, copy from `.env.example`, fill keys.

## 4) Install per‑track deps

Each track README has:

```bash
make setup     # or: pip install -r requirements.txt
make run       # or: python main.py
```

## 5) Sanity check

* `python --version`
* `pip list | grep requests` (or other deps)
* If using Node, `node -v` / `npm -v`