# Track 05 – OpenAPI Minifier

Goal: given a giant OpenAPI, extract a **minimal** spec containing only operations needed for a task (e.g., “create Jira task”).

## Approach
- Input: `openapi-full.yaml` + a list of operations you need
- Output: `openapi-min.yaml` with only:
  - referenced paths/operations
  - required schemas/components
  - servers & auth
- CLI usage:
```bash
python minify.py --input openapi-full.yaml --ops POST:/rest/api/3/issue --output openapi-min.yaml
```

## Deliverables

* `minify.py` (MVP is fine)
* Before/after size comparison
* Example run output