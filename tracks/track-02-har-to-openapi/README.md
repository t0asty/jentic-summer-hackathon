# Track 02 – HAR → OpenAPI

Goal: capture a HAR from a real site, convert to OpenAPI 3.0+, submit spec to `jentic-public-apis`.

## Steps
1. Read **[HAR guide](../../guides/04-har-file-how-to.md)**
2. Capture & sanitize `sample.har`
3. Create `openapi.yaml` (manual/script/LLM‑assist)
4. Validate (`openapi-spec-validator`, Swagger Editor)
5. Open PR to `jentic/jentic-public-apis`

## Run validator locally
```bash
python -m venv .venv && source .venv/bin/activate
pip install openapi-spec-validator
python - << 'PY'
from openapi_spec_validator import validate_spec
import yaml, sys
with open('openapi.yaml') as f:
    spec = yaml.safe_load(f)
validate_spec(spec)
print("✅ Spec is valid")
PY
````

## Deliverables

* `openapi.yaml`
* Notes: endpoints, auth, examples
* PR link in your submission issue