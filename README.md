# hYYa ink — read and edit every document, natively on Mac, iPad, iPhone and Android

**Stop reading syntax. Start reading/editing documents.**

hYYa ink is a native app for macOS, iPadOS, iOS and Android that opens developer,
academic and everyday file formats as *rendered, editable documents* instead of walls
of plain text — and it works with **PDFs** too: view, add text anywhere on the page,
sign by hand, mark up by hand, save a copy and print.

**→ [Download and full details at hyya.com/hyya-ink.html](https://hyya.com/hyya-ink.html)**

[![Mac App Store](https://img.shields.io/badge/Mac%20App%20Store-Download-0071e3)](https://hyya.com/hyya-ink.html)
[![App Store](https://img.shields.io/badge/iPhone%20%26%20iPad-App%20Store-0071e3)](https://hyya.com/hyya-ink.html)
[![Google Play](https://img.shields.io/badge/Android-Google%20Play-34a853)](https://play.google.com/store/apps/details?id=com.hyya.ink)

---

## What it does

Open a `.json`, `.md`, `.csv`, `.mmd` or `.pdf` file and you get a real document —
formatted headings, an interactive data tree, a readable table, a rendered diagram,
a paginated page — not raw syntax. Everything renders **locally and offline**.

| | |
|---|---|
| 📄 **Read anything** | 16 formats rendered inside the app, PDF included — see [Supported formats](docs/FORMATS.md) |
| ✍️ **Edit in place** | Markdown tools; JSON values in the tree and CSV/TSV cells in the table; any text format, YAML and TOML included, in the **Edit** view |
| 🖊️ **PDF: add text, sign & mark up** | Add text anywhere by clicking the spot and typing, hand-sign in black or blue ink, mark up by hand, find, OCR a scan, organise pages, redact text permanently, save a copy or print — see [PDF guide](docs/PDF.md) |
| 🤖 **AI, your own key** | Explain, summarize, reformat, fix errors, or write Mermaid code for a diagram — bring your own API key (OpenRouter, OpenAI, Groq, Together AI or a custom endpoint), or run a local model on your Mac via Ollama / LM Studio |
| 👁️ **Quick Look** *(Mac only)* | Press Space in Finder to look at a text file without opening the app — CSV and TSV as a table, JSON pretty-printed, the rest as source. It shows the file, not the rendered document; see [Quick Look](docs/FORMATS.md#quick-look) |
| 🔒 **Local-first** | No account and no server. The Apple apps send no telemetry; on Android, Google's built-in text-recognition library sends Google its own diagnostics — never your documents. Your documents never leave your device unless you run an AI action |

## Supported formats

Markdown · JSON · YAML · TOML · XML · CSV / TSV · **PDF** · Mermaid · Graphviz ·
LaTeX · Jupyter notebooks · diff / patch · log files · AsciiDoc · Org-mode ·
plain text · source code

Rendering Typst (`.typ`) documents is **not planned** — not a licensing question
(Typst is Apache-2.0 and its fonts are freely embeddable) but a size one: the WASM
compiler alone is 27 MB, plus 5–7 MB of fonts that must ship inside the app because
every hYYa ink renderer works offline. That is roughly 6× the entire current renderer
payload. On Android, `.typ` files open as readable source.

Rendering PlantUML (`.puml`) diagrams is **not planned** — the engine is Java, and the
builds that could run it offline inside the app can't be licensed for a commercial app.
On Android, `.puml` files open as readable source. For diagrams that render today, use
**Mermaid** or **Graphviz**.

Full breakdown of what each format renders → **[docs/FORMATS.md](docs/FORMATS.md)**

## Platforms

- **macOS** 14+ — Mac App Store
- **iPadOS / iOS** 17+ — App Store (Universal Purchase with the Mac app)
- **Android** 9+ — Google Play

## Pricing

Free to download and **free forever to read and preview** — including PDF export.
Editing, signing and AI actions are a **one-time purchase**. No subscription.
Buy once on the App Store and it unlocks on your Mac, iPad and iPhone. On Android,
Pro is a separate one-time purchase through Google Play.

## Documentation

- **[Supported formats](docs/FORMATS.md)** — what every format renders and how
- **[PDF: add text, sign & save](docs/PDF.md)** — the full PDF workflow
- **[FAQ](docs/FAQ.md)** — privacy, AI keys, licensing, troubleshooting
- **[Changelog](CHANGELOG.md)** — what shipped when

## Support & feedback

Found a bug or want a format supported? **[Open an issue](https://github.com/hyya-dev/hyya-ink-docs/issues)** —
this repository is the public issue tracker. You can also reach us via
[hyya.com/#contact](https://hyya.com/#contact).

> This repository holds hYYa ink's public documentation and issue tracker.
> The app itself is a commercial product; its source is not published here.

---

© hYYa. hYYa ink is a product of hYYa — [hyya.com](https://hyya.com).
