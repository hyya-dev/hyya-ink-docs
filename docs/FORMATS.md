# Supported formats

hYYa ink detects a file's format from its content type, extension and content
signature — then renders it with a purpose-built native view. Every renderer runs
**locally and offline**; nothing is uploaded.

Viewing and previewing every format is **free forever**. Editing requires the
one-time Pro unlock.

---

## Documents & markup

### Markdown (`.md`, `.markdown`, `.mdown`, `.mkd`)
Rendered as a formatted document — headings, lists, tables, blockquotes, task
lists, links and fenced code with syntax highlighting. Pro adds a **Markdown
toolbar** for bold/italic/heading/link/list/code so you can format without
memorizing syntax. Export the rendered result to a paginated PDF.

### AsciiDoc (`.adoc`, `.asciidoc`, `.asc`)
Full AsciiDoc rendering — sections, admonitions, tables and source blocks.

### Org-mode (`.org`)
Outline headings, TODO keywords, tables and source blocks rendered as a document.

### LaTeX (`.tex`, `.latex`, `.sty`)
Math and formulas typeset via KaTeX so equations read as equations, not macros.

### Typst (`.typ`)
Modern typesetting source, rendered.

### Plain text & source code
Syntax-aware display for source files, with the same export and preview pipeline.

---

## Structured data

### JSON (`.json`)
An **interactive, collapsible tree** — expand and collapse objects and arrays,
scan large payloads without counting brackets. Pro allows editing values in place
and writes valid JSON back.

### YAML (`.yaml`, `.yml`)
The same interactive tree treatment, so nesting is visible instead of inferred
from indentation.

### TOML (`.toml`)
Tables and nested keys rendered as a navigable tree.

### XML (`.xml`)
Element tree with attributes, collapsible by node.

### CSV & TSV (`.csv`, `.tsv`)
A real **spreadsheet-style grid** with aligned columns and headers — not comma
soup. Pro allows cell editing, and writes correctly-escaped CSV back out.

### Jupyter notebooks (`.ipynb`)
Cells rendered in order — Markdown cells as prose, code cells with highlighting,
and stored outputs — without launching Jupyter.

---

## Diagrams

### Mermaid (`.mmd`, `.mermaid`)
Flowcharts, sequence diagrams, Gantt charts, class and state diagrams rendered
from text, offline. The rendering bundle ships inside the app — no CDN, no network.

### Graphviz / DOT (`.dot`, `.gv`)
Graph layouts rendered natively from DOT source.

---

## Engineering files

### Diff & patch (`.diff`, `.patch`)
Colour-coded additions and deletions with hunk headers, so a patch reads like a
review instead of a wall of `+`/`-`.

### Log files (`.log`)
Level-aware rendering that makes warnings and errors visible at a glance in long
logs.

---

## PDF

### PDF (`.pdf`)
A first-class document, not an afterthought: view any PDF, **type into form
fields**, **sign by hand** in black or blue ink, resize and rotate your signature,
undo/redo, then export or print. Full walkthrough → **[PDF guide](PDF.md)**.

Viewing and exporting PDFs is free; filling and signing require Pro.

---

## Quick Look

Every format above also previews with the **space bar in Finder** via hYYa ink's
Quick Look extension — no need to open the app.

## Don't see your format?

[Open an issue](https://github.com/hyya-dev/hyya-ink-docs/issues) and tell us what
you'd like rendered.

**→ [Download hYYa ink](https://hyya.com/hyya-ink.html)**
