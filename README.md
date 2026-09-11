# tokenpurse

Estimate LLM cost of a file before you send it

Side project, maintained when I have time.

## Highlights

- Zero dependencies
- Heuristic token estimate (~4 chars/token)
- Reports input/output tokens and USD estimate
- Per-model pricing table in JSON

## Getting started

```bash
# stdlib only
```

## Examples

```bash
python cost.py prompt.txt --model gpt-4o-mini --expect-out 500
```

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── faq.md
│   ├── roadmap.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_smoke.py
├── .editorconfig
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── SECURITY.md
├── cost.py
└── pricing.json
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```
