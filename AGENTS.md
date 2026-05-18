# AGENTS.md

## Stack
- **Single-file static site** — no framework, no bundler, no package manager
- Vanilla HTML/CSS/JS in `index.html`
- **Font Awesome 6.4.0** from CDN (`cdnjs.cloudflare.com`) for icons
- Hosted on **GitHub Pages** at `jrhunter3.github.io`

## Key facts
- All markup, CSS (inline `<style>`), and JS (inline `<script>`) live in one file — `index.html`
- Dark mode persisted via `localStorage` with key `darkMode`
- "Download PDF" calls `window.print()`; expanded job descriptions are toggled open before print and collapsed afterward
- Job descriptions expand/collapse via `toggleDescription()` — click the job header
- Scroll animations use `IntersectionObserver` with a 0.1 threshold
- No tests, no linter, no typechecker, no CI
- Only `.gitignore` entry: `.idea/` (JetBrains)
- Preview image: `og-image.png`

## Making changes
- Edit `index.html` directly — no build step needed
- Open `index.html` in a browser to preview locally
- Push to `main` to deploy (GitHub Pages auto-deploys from the default branch)
