# AGENTS.md

## Cursor Cloud specific instructions

This is a **static website** project (plain HTML, CSS, JavaScript) with no build step, no package manager, and no runtime dependencies.

### Running the dev server

Serve the project root with any static file server:

```sh
python3 -m http.server 8080 --directory /workspace
```

Then open `http://localhost:8080` in the browser.

### Lint / Test / Build

- **Lint**: No linter is currently configured. If one is added in the future, check `package.json` scripts.
- **Tests**: No automated test suite exists yet.
- **Build**: No build step required — the site is served directly from source files (`index.html`, `styles.css`, `script.js`).

### Project structure

| File | Purpose |
|---|---|
| `index.html` | Main page markup |
| `styles.css` | All styles (CSS custom properties, responsive layout) |
| `script.js` | Mobile menu toggle and dynamic copyright year |
| `README.md` | Project overview |

### Notes

- The site uses Google Fonts (`Inter`) loaded via CDN, so font rendering requires internet access.
- No Node.js dependencies or `package.json` — no `npm install` needed.
