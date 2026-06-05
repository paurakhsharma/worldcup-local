# AGENTS.md

## Cursor Cloud specific instructions

### Product overview

Single-file static web app (`index.html`) — FIFA World Cup 2026 match schedule with local timezone conversion and squad rosters. No backend, build step, package manager, or test/lint tooling in this repository.

### Running the app

From `/workspace`:

```bash
python3 -m http.server 8080
```

Open http://localhost:8080/index.html in a browser. Prefer serving over HTTP rather than opening `file://` directly (some browser APIs and automated testing behave more reliably over HTTP).

### Lint / test

There is no configured linter or automated test suite. Verification is manual: confirm the page loads (HTTP 200), match cards render, tabs switch (Matches ↔ Squads), and squad modals open from match cards.

### External dependencies (optional at runtime)

- **Google Fonts** (`fonts.googleapis.com`) — typography; falls back to system fonts if unavailable.
- **SofaScore API** (`api.sofascore.app`) — club logos in squad tables; images fail silently via `onerror`.
- **Wikipedia** — only when users click player/coach links.

Core functionality works fully offline once the page is loaded.

### Data editing

All match and squad data lives inline in `index.html` (`M`, `SQUADS`, `GROUPS` constants). See `README.md` for squad update workflow and Wikipedia API fetch instructions.
