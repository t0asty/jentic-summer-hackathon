# Track 03 – Arazzo Runner Basics

Goal: run a simple Arazzo workflow that calls a public API.

## Steps
1. Read **[Runner quickstart](../../guides/03-arazzo-runner-quickstart.md)**
2. Use the included `workflows/hello.yaml` or point to a public API
3. Run the workflow and capture output

## Commands
```bash
python -m venv .venv && source .venv/bin/activate
pip install arazzo-runner  # if published; otherwise pip install -e from repo
arazzo-runner run workflows/hello.yaml
```

## Deliverables

* Screenshot/logs of successful run
* Optional: a second workflow with parameters