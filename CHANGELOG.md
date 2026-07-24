# Changelog

All notable changes to hYYa ink. **→ [Download the latest version](https://hyya.com/hyya-ink.html)**

## 1.2.0 — 2026-07-23

**Mark up PDFs by hand.**

> Live now on the Mac App Store. The iPhone & iPad update — which is the one that
> carries handwritten markup — is in review and rolling out shortly.

- **Handwritten markup on iPhone and iPad.** Annotate any PDF with Apple Pencil —
  or your finger — using pen, marker and highlighter. A single session can span
  several pages, and it commits as one undo step.
- Your handwriting is written **into the page itself**, so it travels with the file
  through export, printing and other PDF apps. It is not re-editable afterwards —
  see [docs/PDF.md](docs/PDF.md) for the full trade-off.
- Handwritten markup is **iPhone and iPad only** — the Mac app does not have it.
- A new launch screen on iPhone and iPad (iOS 18+).
- The formats guide now labels **Typst** and **PlantUML** as "coming soon", so it
  only promises what hYYa ink actually renders today.
- Small fixes and refinements.

> The direct `.dmg` download for Mac was retired with this release. hYYa ink now
> ships through the **App Store only** — one purchase covers Mac, iPad and iPhone.

## 1.1.1 — 2026-07-12

- Clearer AI setup: hYYa ink now reminds you to save your key before leaving
  Settings, so your provider and model are never lost.
- The Pro screen now highlights PDF fill & sign.
- Local AI providers (Ollama, LM Studio) are now correctly shown only on Mac,
  where they can actually be reached.
- Small fixes and refinements.

## 1.1.0 — 2026-07-11

**PDF arrives.**

- Open any PDF as a first-class document.
- Fill forms and flat paperwork: tap anywhere and type, then drag to reposition.
- Sign by hand in black or blue ink; resize, rotate and place your signature.
- Undo and redo buttons for PDF edits.
- Export or print any supported document to a clean, paginated PDF, with
  typographic pagination that never slices a heading or code block across pages.

## 1.0.6 — 2026-07-07

- Larger, easier-to-tap toolbar controls for a more comfortable, accessible
  experience.
- AI actions now wait until your document has content before they run.
- macOS: the welcome window now closes properly once a document is open.

## 1.0.0 — 2026-07-05

Initial release — render and edit Markdown, JSON, YAML, TOML, XML, CSV/TSV,
Mermaid, Graphviz, LaTeX, Typst, Jupyter, diff, logs, AsciiDoc and Org-mode
natively, with a Quick Look extension and bring-your-own-key AI actions.
