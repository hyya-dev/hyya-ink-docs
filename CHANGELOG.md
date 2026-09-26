# Changelog

All notable changes to hYYa ink. **→ [Download the latest version](https://hyya.com/hyya-ink.html)**

## Android — update on Google Play 2026-09-26

- **Edit right where you read** (Pro) — change a JSON value in the tree, or a CSV or TSV cell in
  the table, and only that value's text changes in the file: keys keep their order, numbers keep
  their digits and line endings stay as they were. Tables also gain Add row and Add column.
- **Contents** — the page browser lists the PDF's own table of contents when it has one; tap a
  heading to go to its page.
- **Organise Pages adds another PDF** — insert the pages of a second PDF, then reorder them.
- **Open with hYYa ink** — open a document straight from another app. If that app lets hYYa ink
  read but not write the file, saving offers a copy instead.
- **Add Text, Sign and Markup open on the page you are reading** — they used to open on page 1.
- **Typing stays readable** — while you type in Add Text, the page keeps its full size and scrolls
  to your text, instead of shrinking into the space above the keyboard.
- **Redaction keeps the rest searchable** — the words you keep on a redacted page are read again,
  so they can still be searched and selected.
- **Smaller fixes** — LaTeX `equation` and `align` blocks show as maths; numbered lists keep their
  first number; AsciiDoc code blocks are readable in Light Mode; buttons and controls use the ink
  colour throughout.

## 1.4.9 — iPhone & iPad 2026-09-25 · Mac 2026-09-25

**Two changes, the same on iPhone, iPad and Mac.**

- **Markdown task lists show done and not done** — `- [x] Signed` reads ☑ and
  `- [ ] Pending` reads ☐ in the document you are reading. They had shown as plain bullets on
  screen while an exported PDF already drew the boxes.
- **Reading a document never reaches the internet** — the four built-in renderers (Mermaid,
  Graphviz, LaTeX and AsciiDoc) now load only what ships inside the app. Until 1.4.9 an AsciiDoc
  `image::https://…[]` line was fetched from the web the moment you opened the document, which
  told that server when the file was read.

## Android — on Google Play 2026-09-25

**hYYa ink is now on Android**, from
[Google Play](https://play.google.com/store/apps/details?id=com.hyya.ink), for Android 9 or
later. It is a separate app with its own version numbers, and its Pro is a separate one-time
purchase through Google Play, tied to your Google account.

- **Formats** — rendered on your device: Markdown, JSON, YAML, TOML, XML, CSV and TSV,
  Mermaid, Graphviz, LaTeX, Jupyter, AsciiDoc, Org-mode, diff, logs and PDF.
- **PDF** — read, search and copy the text; tap the page and type; sign by hand; draw on a pad
  and place the drawing; highlight, underline or strike through a line of text; and open
  password-protected files. Organise pages, protect, compress, watermark, make a scan searchable
  (Latin script and Arabic) and redact — each writes a new file and leaves the PDF you opened
  unchanged — and compare two PDFs to see which pages differ.
- **AI, with your own key** — OpenRouter, OpenAI, Groq, Together AI or another service that
  works the same way, on every format except PDF. Only the open document's text is sent, and
  only when you run an action.
- **Free to read** — every format, Export to PDF and Print. A 7-day trial you start yourself;
  after that, one purchase unlocks editing, the PDF tools and AI.

## 1.4.8 — iPhone & iPad 2026-09-21 · Mac 2026-09-21

**One change: the Settings panel now signs itself off.**

- **Everywhere** — Settings ends with the ink mascot and the app's name beneath it, after
  "Help and more". The mascot used to float between two cards with nothing attached to it, so
  it read as a stray picture rather than as the app putting its name to its own panel. It is
  drawn as the same rounded square, at the same corner ratio, as the lockup on the first
  screen, so the two surfaces read as one app.

That is the whole release. Everything else that happened between 1.4.7 and 1.4.8 was on
Android, which is a separate app with its own version numbers and is not on the App Store.

## 1.4.7 — iPhone & iPad 2026-09-20 · Mac 2026-09-20

**Settings rewritten into five plain cards, an Auto theme that actually follows your device,
and a first screen that is not covered by the Dynamic Island.**

- **Everywhere** — **Settings is five cards**: Appearance, hYYa ink Pro, AI, Formats it opens,
  and Help and more. The long explanatory paragraphs are gone; each card says what it is for
  in a sentence you can act on.
- **Everywhere** — **three appearance modes: Auto, Light Mode and Dark Mode.** Auto follows
  whatever your device is set to and changes with it. ⚠️ **Classic Dark has been removed.**
  If you were using it you are now on Dark Mode, which is the same dark theme; nobody's choice
  was reset.
- **Everywhere** — **Auto now works.** Choosing it used to leave the app in whichever theme it
  was already showing, so it never picked up your device's setting at all. It reads the system
  directly now, on both platforms, and follows it when you change it.
- **iPhone & iPad** — the **first screen** has been rebuilt around the mascot: it is no longer
  hidden behind the Dynamic Island, and the app's name is centred underneath it. On a light
  device that name used to be black on a dark background — effectively invisible.
- **Mac** — **clicking the Dock icon brings the app back.** If you closed the last window the
  app stayed running with nothing on screen, and clicking its icon did nothing.
- **Mac** — the **default-app card** is a title and four steps. The paragraph explaining what
  macOS does and why has been deleted; it was an essay in the middle of a set of instructions.

## 1.4.6 — iPhone & iPad 2026-09-16 · Mac 2026-09-16

**Three things the new OS quietly stopped doing, working again — plus five things a
ten-minute look at the app turned up.**

- **Everywhere** — **Make Searchable** puts text back into a scan. On macOS 27 and iOS 27 it
  had been handing back a file with no text in it at all: no error, no warning, nothing to
  search. ink now reads each page itself and writes the text layer.
- **Everywhere** — this also restores **Redact**. The text you *keep* on a redacted page is
  read again afterwards, so it stays searchable and selectable. What is removed is still
  removed — that never changed.
- **Everywhere** — **Compress** makes a scan smaller again. It had been returning a file very
  slightly *larger* than the one you gave it.
- ⚠️ **Compress is narrower than it used to be, deliberately.** It re-encodes pages that are
  only a picture — a scan or a photo. A page carrying its own text is passed through untouched,
  because shrinking it would mean destroying text you can search and select. Two things follow,
  and they are worth knowing rather than discovering: a mixed page of photographs *and* writing
  no longer gets smaller, and a document you have already run through Make Searchable will not
  compress at all, because every page now has text on it. **Compress first, then make it
  searchable.** The sheet says which case you are in.
- **Mac** — **Add Text** places text on a PDF again. On macOS 27, clicking the page did
  nothing at all.
- **Everywhere** — the **Find** field in a PDF now looks like a field: its own background, its
  own outline, and the theme's accent colour when you are typing in it. It used to be bare text
  on the bar, and it was easy to miss in every theme.
- **Everywhere** — the same **Try free** button no longer appears twice, a few millimetres
  apart, saying the same thing.
- **Everywhere** — the trial screen now says plainly that you are **not charged** when the
  seven days end and that there is nothing to cancel. It always worked that way; it never said so.

## 1.4.5 — iPhone & iPad 2026-09-14 · Mac 2026-09-14

**Select All and Copy, the way every other document app does it.**

- **Everywhere** — the page you read is now a real text view, so **Select All** and **Copy** are
  the system's own commands: ⌘A then ⌘C on the Mac, long-press then Select All on iPhone and
  iPad. Dragging across a document now works too, including across a heading, a quote and a
  table in one sweep — before, a selection could not leave the block it started in.
- **Everywhere** — the **Copy all text** command added in 1.4.4 has been removed. It was a
  button standing in for a capability that should never have needed one, and the capability is
  now there.
- ⚠️ **What lands on the clipboard has changed.** You now copy what you see: a Markdown heading
  arrives as "Lease summary", not "# Lease summary". If you want the raw file with its syntax,
  copy from the **Source** pane. Plain text, code, diffs and logs are unchanged.

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
