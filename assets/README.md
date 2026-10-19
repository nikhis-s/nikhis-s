# Assets

Self-contained SVG assets for the `nikhis-s` profile README. No scripts, no external images, no fonts loaded remotely.

## Design system

- **Background** — deep navy / charcoal (`#080d18` → `#141d33`)
- **Accents** — restrained cyan (`#22d3ee`) and electric blue (`#3b82f6`)
- **Text** — primary `#f1f5f9` / `#e2e8f0`, muted `#94a3b8`, captions `#64748b`
- **Lines / strokes** — `#1b2c4a`, grid `#16233c`
- **Type** — system UI stack for headings, monospace stack for labels

## profile-header.svg

Hero banner for the top of the README.

- **Dimensions:** 1200 × 300
- **Content:** hexagonal `n` monogram, the `nikhis-s` wordmark, the headline *Building reliable software systems*, and a secondary line spanning Python, applied AI/ML and operations.
- **Motifs:** fine circuit traces in both corners and a faint 30px grid.

## engineering-map.svg

Four connected engineering focus areas, drawn as a schematic bus feeding four cards.

- **Dimensions:** 1200 × 440
- **Content:** Python & application engineering; applied AI & LLM systems; machine learning & data evaluation; reliability, testing & operations.
- **Note:** framed as areas of focus and growth, not verified mastery.

## Editing

Both files are plain XML with no external dependencies. Edit text, colours or geometry directly in any text editor, then open in a browser to preview. Keep each file's accessible `<title>` / `<desc>` metadata in sync with any content changes, and re-validate the XML before committing:

```powershell
[xml](Get-Content -Raw .\assets\profile-header.svg) | Out-Null
[xml](Get-Content -Raw .\assets\engineering-map.svg) | Out-Null
```
