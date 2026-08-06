# Changelog

All notable changes to hYYa ink. **→ [Download the latest version](https://hyya.com/hyya-ink.html)**

## 1.2.5 — 2026-08-02

**Both platforms back in step.**

- iPhone and iPad gain everything the Mac received in 1.2.3 and 1.2.4 — the light
  theme fixes, the undo rework and the large-document crash fix below.
- The Add Text field on a PDF is readable again, and the text no longer freezes in
  place once you tap Done.

> 1.2.2 was withdrawn before release and never shipped on either platform. 1.2.3 and
> 1.2.4 reached the Mac only while the iPhone and iPad release was held; 1.2.5 puts
> every platform back on the same version.

## 1.2.4 — 2026-08-01 · Mac only

- Large documents no longer crash the app.

## 1.2.3 — 2026-07-30 · Mac only

**Light mode fixed.**

- The light themes were unusable. In Classic Light, source text rendered almost
  white-on-white, and cards and code blocks were the same pure white as the
  background behind them. Both now have a real contrast ladder.
- Undo is wired to ⌘Z, routed through the same per-entry undo the toolbar button uses.
- **The redo button is gone.** Undo steps back through your edits; there is no redo.
- **Handwritten markup now stays adjustable.** Your ink remains editable for as long
  as the document is open, and nothing is written until you save. Saving writes a new
  PDF and leaves your original untouched — and only in that saved copy is the ink part
  of the page. This replaces the behaviour described under 1.2.0 and 1.2.1 below,
  where ink was committed into the page as you drew and could not be adjusted
  afterwards.

## 1.2.1 — 2026-07-25

**Markup comes to the Mac.**

- **Handwritten markup on the Mac.** Write, highlight and annotate straight onto the
  page with your trackpad or mouse: pen, marker, pencil and eraser, five ink colours,
  adjustable thickness, and undo stroke by stroke. One session can span several
  pages, then saves once — the same as on iPad.
- Markup ink is now always saved in the colour you chose, in every appearance —
  including Dark Mode.

> The Mac gets its own drawing surface rather than the iPad's: Apple's PencilKit
> supplies the ink on macOS but no ready-made canvas or tool palette. The strokes are
> the same real PencilKit ink, flattened into the page the same way, so a PDF marked
> up on a Mac is indistinguishable from one marked up on an iPad.

## 1.2.0 — 2026-07-23

**Mark up PDFs by hand.**

- **Handwritten markup on iPhone and iPad.** Annotate any PDF with Apple Pencil —
  or your finger — using pen, marker and highlighter. A single session can span
  several pages, and it commits as one undo step.
- Your handwriting is written **into the page itself**, not as a removable
  annotation layer — so recipients can't strip your notes, no author metadata rides
  along in the file, and the marks render anywhere. They're permanent once
  committed; see [docs/PDF.md](docs/PDF.md).
- Handwritten markup is **iPhone and iPad only** in this version — the Mac gained it
  in 1.2.1.
- A new launch screen on iPhone and iPad (iOS 18+).
- The formats guide is clearer about which formats render and which open as source.
  ⚠️ This release labelled **Typst** and **PlantUML** as "coming soon". That promise
  has since been retracted: neither is planned, both open as readable, syntax-aware
  source, and rendering them was ruled out — see [docs/FORMATS.md](docs/FORMATS.md).
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
- Add text anywhere on a PDF: tap the exact spot you want and type, then drag to
  reposition. hYYa ink detects no form fields — you place every piece of text
  yourself, which is what lets it work on scans and flat paperwork as well.
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
Mermaid, Graphviz, LaTeX, Jupyter, diff, logs, AsciiDoc and Org-mode natively,
with a Quick Look extension (Mac) and bring-your-own-key AI actions.
Typst (`.typ`) files open as readable source; rendering them is not planned.
