# rag-lite

Ask questions over my notes folder

## Getting started

```bash
pip install -r requirements.txt
```

## How to use

```bash
python rag.py ./notes "how do I rotate logs?"
```

## Features

- TF-IDF retrieval: zero external services needed
- Chunk markdown with overlap, keep source paths
- Prints sources with scores for transparency
- Swap in any LLM for the answer step

## Project structure

```text
├── .github/
│   ├── workflows/
│   │   └── ci.yml
│   └── dependabot.yml
├── data/
│   └── sample.md
├── docs/
│   ├── configuration.md
│   ├── development.md
│   ├── roadmap.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_smoke.py
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── LICENSE
├── SECURITY.md
├── rag.py
└── requirements.txt
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## License

MIT. Do whatever you want.
