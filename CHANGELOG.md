# Changelog

All notable changes to hYYa ink. **→ [Download the latest version](https://hyya.com/hyya-ink.html)**

## 1.4.4 — iPhone & iPad 2026-09-13 · Mac 2026-09-13

**Getting the text out of a document.**

- **Everywhere** — text that could not be selected now selects. Headings and table cells in
  Markdown were skipped, so you could highlight a paragraph but not the title above it.
- **Everywhere** — **Copy all text** takes a whole document in one action. A highlight can only
  ever cover one block at a time, so taking the entire file was not just awkward, it was not
  possible. It's free, like reading, exporting and printing. On the Mac it's Edit ▸ Copy All
  Text (⇧⌘C); on iPad it sits beside Export and Print; on iPhone the three share the ••• menu.
  What lands on the clipboard is the file itself — `# Heading` and `**bold**` survive, so what
  you paste is what you opened.
- PDFs are unchanged: they already answer Select All and Copy on their own.

## 1.4.3 — iPhone & iPad 2026-09-13 · Mac 2026-09-13

**A small update.**

- **Mac** — Quick Look now shows **TSV** files as a table, the same as CSV. Pressing the space
  bar on a `.tsv` file in Finder used to fall back to plain text.
- **iPhone & iPad** — no changes to the app itself in this version.

## 1.4.2 — iPhone & iPad 2026-09-09 · Mac 2026-09-11

**A small update.**

- **iPhone & iPad** — a **Text size** setting in Settings ▸ Appearance, with a Reset. It adds
  to Larger Text (Dynamic Type) rather than replacing it, so a size you already chose for the
  whole device still counts.
- **Mac** — the help for making hYYa ink your default app now explains, in plain words, what
  setting it does for your documents.

## 1.4.1 — iPhone & iPad 2026-09-03 · Mac 2026-09-02

**A small follow-up.**

- **iPhone & iPad** — a live page count over every PDF, so you always know where you are; on
  iPad the page browser opens as a panel beside the page (on iPhone it remains a sheet); small
  fixes.
- **Mac** — View ▸ Actual Size (100 %) and View ▸ Zoom to Fit (⌘9) are two commands, and the
  zoom commands are greyed out on a window that is not a PDF; small fixes.

## 1.4.0 — iPhone & iPad 2026-09-02 · Mac 2026-09-02

**The PDF reader gets the ordinary things it was missing.**

- **Print a PDF** — previously offered only for the text formats. Both platforms.
- **Tables read row by row with VoiceOver**, each cell announcing its column. Both platforms.
- **When a JSON, YAML or TOML file will not parse, the app says so** and shows the source
  instead of showing nothing. Both platforms.
- **AI actions that rewrite your document ask first, and can be undone.** Both platforms.
- **Mac** — View ▸ Zoom In / Zoom Out on PDFs, with a live page readout in the toolbar; a
  **Text size** preference in Settings that every screen honours; drag a file onto a window to
  open it; Quick Look previews `.yaml` and `.toml`.
- **iPhone & iPad** — Larger Text (Dynamic Type) is honoured on every screen; going back with
  unsaved text, a signature or markup asks before discarding.

## 1.3.3 — iPhone & iPad 2026-08-27 · Mac 2026-08-29

**Two new PDF tools that remove text rather than hide it, and a clearer free trial.**

- **Redact** — remove text from a PDF for good. Not a black bar drawn on top: the
  affected page is rasterised, so the words leave the file and cannot be selected,
  copied or searched afterwards. Only pages you redact are rasterised; the rest of the
  document keeps its selectable text. On-device recognition then runs over the redacted
  page, so the text you kept stays searchable there too — the removed words cannot return,
  because the bars go on before the page is photographed.
- **Cover and replace** — swap a date or a figure for new text. The original is removed
  too, rather than hiding underneath the replacement. It uses the same engine as Redact,
  so a replaced document cannot display one value and extract another.
- **Mac: make hYYa ink your default.** Settings now explains how to open your files in
  ink from Finder. Instructions only — macOS does not permit an app to change that
  binding itself, so there is no button that pretends to.
- The free 7-day trial is now named on the control that opens the Pro screen. It used to
  read only "Unlock Pro", so the trial was easy to miss; it now reads "Try free", and
  becomes "Unlock Pro" only once a trial has been used.
- If you have never started a trial, the app no longer tells you that one has ended.

⚠️ **What Redact does and does not promise.** It removes the text you select on the pages
you redact. It does **not** scrub document metadata, attachments or embedded files, so it
sanitises a page — not a whole document.

Every tool still writes a NEW file. The document you opened is never modified.

## 1.3.2 — 2026-08-12

**Four fixes, all of them about reading.**

- Text in a PDF can be selected and copied again.
- Values in a JSON, YAML or TOML file can be selected and copied.
- `.yaml`, `.yml` and `.toml` files now open. They were greyed out before.
- A selection made while reading no longer lingers when you switch to Add Text.

Every tool still writes a NEW file. The document you opened is never modified.

## 1.3.1 — 2026-08-09

**The ten PDF tools reach iPhone and iPad, and three fixes land on the Mac.**

- **iPhone and iPad** gain everything the Mac received in 1.3.0 below — Find in
  document, Pages and contents, Make Searchable, Organise Pages, Protect, Compress,
  Watermark, Compare, Mark Up Text, and opening password-protected PDFs.
- **Print is back on PDFs.** It had been hidden whenever the open document was a PDF —
  the one kind of file people print most — on both platforms.
- Printing a PDF now includes what you added on screen: typed text, a signature, markup.
- "Insert pages from another PDF…" in Organise Pages now opens a file chooser.

> iPhone and iPad went straight from 1.2.5 to 1.3.1; there was no 1.3.0 on those
> platforms.

## 1.3.0 — 2026-08-06 · Mac only

**Ten new PDF tools — including the one that changes what hYYa ink can read.**

- **Make Searchable** — on-device text recognition turns a scanned page into a PDF you
  can search and select. AI actions work on scans now too. Nothing is uploaded.
- **Find in document** — every match highlighted, with a live count.
- **Pages and contents** — page thumbnails and the document's own contents.
- **Organise Pages** — reorder, rotate and remove pages.
- **Protect** — set an open password, and allow or block printing and copying.
- **Compress** — the exact before-and-after size, shown before you save.
- **Watermark** — a live preview as you type.
- **Compare** — see which pages differ between two versions.
- **Mark Up Text** — highlight, underline or strike through what you select.
- Password-protected PDFs now open properly.

Every tool writes a NEW file. The PDF you opened is never modified.
Find, Pages and contents, and opening protected PDFs are free; the rest are Pro.

Also in this release: the 7-day trial is now something you **start yourself** rather
than something that begins on first launch, and it runs once per Apple Account.

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
