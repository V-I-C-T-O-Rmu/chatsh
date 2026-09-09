# chatsh

Tiny streaming CLI for OpenAI-compatible chat APIs

Side project, maintained when I have time.

## Examples

```bash
chatsh explain this error < error.log
cat diff.patch | chatsh review this diff
```

## Getting started

```bash
pip install -r requirements.txt
export OPENAI_API_KEY=sk-...
```

## Highlights

- Reads the prompt from args or stdin
- Works with any OpenAI-compatible endpoint
- Model and system prompt via flags or env
- Streams tokens as they arrive

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── configuration.md
│   ├── faq.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_smoke.py
├── .gitignore
├── LICENSE
├── Makefile
├── SECURITY.md
├── chatsh.py
└── requirements.txt
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## Notes

- mostly stable, edge cases remain

## License

MIT. Do whatever you want.
