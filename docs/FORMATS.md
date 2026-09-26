# Supported formats

hYYa ink detects a file's format from its content type, extension and content
signature — then renders it with a purpose-built view inside the app. Every renderer runs
**locally and offline**; nothing is uploaded.

Viewing and previewing every format is **free forever**. Editing requires the
one-time Pro unlock.

---

## Documents & markup

### Markdown (`.md`, `.markdown`, `.mdown`, `.mkd`)
Rendered as a formatted document — headings, lists, tables, blockquotes, task
lists, links and fenced code blocks. Pro adds a **Markdown
toolbar** for bold/italic/heading/link/list/code so you can format without
memorizing syntax. Export the rendered result to a paginated PDF.

### AsciiDoc (`.adoc`, `.asciidoc`, `.asc`)
Rendered as a document — sections, admonitions, tables and source blocks.

### Org-mode (`.org`)
Outline headings, lists and source blocks rendered as a document.

### LaTeX (`.tex`, `.latex`, `.sty`)
Maths written between `$…$`, `$$…$$`, `\(…\)` or `\[…\]` is typeset via KaTeX, so
equations read as equations, not macros. The rest of the file is shown as its LaTeX text.

### Typst (`.typ`) — rendering not planned
On Android, Typst files open as readable source. **Rendering Typst documents is not
planned.** This is not a licensing question — Typst is Apache-2.0 and
embeddable in commercial software, and its fonts are SIL OFL, GUST-LPPL and Bitstream
Vera, so the licence cost is nothing. It is a size question: the WASM compiler alone is
27 MB, and 5–7 MB of fonts have to be bundled with it, because `typst.ts` fetches fonts
over the network by default and every hYYa ink renderer works offline. Together that is
roughly 6× the entire current offline renderer payload, which covers four formats in
5.8 MB.

### Plain text & source code
Shown as clean monospaced text, with the same free export and print as every other format.

---

## Structured data

### JSON (`.json`)
An **interactive, collapsible tree** — expand and collapse objects and arrays,
scan large payloads without counting brackets. Pro lets you edit values
right in the tree, or the file itself in the **Edit** view.

### YAML (`.yaml`, `.yml`)
The same interactive tree, so nesting is visible instead of inferred from
indentation. The tree is for reading; with Pro, edit the YAML itself in the **Edit**
view.

### TOML (`.toml`)
Tables and nested keys rendered as a navigable tree, for reading; with Pro, edit the
TOML itself in the **Edit** view.

### XML (`.xml`)
Element tree with attributes, collapsible by node.

### CSV & TSV (`.csv`, `.tsv`)
A real **spreadsheet-style grid** with aligned columns and headers — not comma
soup. Pro lets you edit cells right in the grid.

### Jupyter notebooks (`.ipynb`)
Cells rendered in order — Markdown cells as prose, code cells in monospace, and
their text output — without launching Jupyter.

---

## Diagrams

### Mermaid (`.mmd`, `.mermaid`)
Flowcharts, sequence diagrams, Gantt charts, class and state diagrams rendered
from text, offline. The rendering bundle ships inside the app — no CDN, no network.

### Graphviz / DOT (`.gv`)
Graph layouts rendered from DOT source, inside the app and offline. **Save Graphviz files as `.gv`.** On macOS the `.dot`
extension belongs to Word templates, and hYYa ink deliberately does not claim it — doing
so would mean claiming every Word template on the Mac.

### PlantUML (`.puml`, `.plantuml`, `.iuml`) — rendering not planned
On Android, PlantUML files open as readable source. **Rendering PlantUML diagrams is
not planned.** PlantUML's engine is Java, and the browser builds
that would let it run offline are not licensable for a commercial app — the CheerpJ
build is explicitly non-commercial, and a server-side renderer would mean sending your
diagram source off your device, which hYYa ink will not do.

For diagrams that render today, use **Mermaid** or **Graphviz** — both render locally
and offline.

### Diff & patch (`.diff`, `.patch`)
Colour-coded additions and deletions with hunk headers, so a patch reads like a
review instead of a wall of `+`/`-`.

### Log files (`.log`)
Level-aware rendering that makes warnings and errors visible at a glance in long
logs.

---

## PDF

### PDF (`.pdf`)
A first-class document, not an afterthought: view any PDF, **add text anywhere** by
clicking the exact spot and typing, **sign by hand** in black or blue ink, resize and
rotate your signature, undo, mark up by hand, then save a copy or print. Further PDF
tools — Find in document, Pages and contents, Make Searchable, Organise Pages, Protect,
Compress, Watermark, Compare, Mark Up Text and Redact & Replace — are covered in the
**[PDF guide](PDF.md)**.

> hYYa ink detects **no form fields** and never hunts for boxes — you place every piece
> of text yourself. That is what lets it work on flat, scanned paperwork.

Viewing and printing PDFs are free, and so are Find in document, Pages and
contents, and opening password-protected PDFs. Adding text, signing, marking up, saving
a copy and the document tools require Pro.

---

## Quick Look

**On the Mac**, pressing the **space bar in Finder** shows these files without opening the
app, via hYYa ink's Quick Look extension:

- **As a table:** CSV and TSV
- **Pretty-printed:** JSON
- **As source:** Markdown, YAML, TOML, Mermaid, Graphviz (`.gv`), LaTeX, Jupyter, AsciiDoc,
  Org, diff / patch, log files, plain text and source code

It is a quick look at the file, not the rendered document — Markdown, diagrams and maths
render when you open the file in hYYa ink. **XML and PDF** use macOS's own preview, and
Typst and PlantUML files are not previewed by hYYa ink. The Quick Look extension is
macOS-only; there is no equivalent on iPhone or iPad.

## Don't see your format?

[Open an issue](https://github.com/hyya-dev/hyya-ink-docs/issues) and tell us what
you'd like rendered.

**→ [Download hYYa ink](https://hyya.com/hyya-ink.html)**
