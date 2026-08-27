# notecrate-api

Tiny REST API for saving and tagging bookmarks

Started as a weekend hack, grew on me.

## How to use

```bash
curl -X POST localhost:3000/api/bookmarks \
  -H 'content-type: application/json' \
  -d '{"url": "https://example.com", "tags": ["reading"]}'
```

## Highlights

- Request validation helpers, no framework magic
- REST endpoints: list / create / delete / search
- Ready for Render/Fly deploy with PORT env
- In-memory store with optional JSON persistence
- Morgan logging and centralized error handler

## Installation

```bash
npm install
npm run dev
```

## Project structure

```text
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   ├── dependabot.yml
│   └── pull_request_template.md
├── docs/
│   ├── configuration.md
│   ├── development.md
│   └── roadmap.md
├── examples/
│   └── quickstart.md
├── src/
│   ├── config.js
│   ├── index.js
│   └── store.js
├── .gitattributes
├── .gitignore
├── CONTRIBUTING.md
├── SECURITY.md
└── package.json
```

## Development

```bash
npm install
npm test
```
