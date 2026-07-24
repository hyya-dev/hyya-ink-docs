# PDF: view, fill, sign, mark up, export

hYYa ink treats PDFs as first-class documents on Mac, iPad and iPhone. Everything
happens **on your device** — no upload, no cloud conversion service, no account.

**→ [Download hYYa ink](https://hyya.com/hyya-ink.html)**

---

## View a PDF

Open any `.pdf` and it renders in a clean, paginated viewer. hYYa ink registers as
an *alternate* PDF handler, so it appears under **Open With** without taking over
Preview as your default.

Viewing is **free forever**.

## Fill in a form

Works on real form fields *and* on flat, scanned paperwork that has no form fields
at all — the common case that trips up other tools.

1. Tap **Fill Blanks** in the toolbar
2. Tap anywhere on the page where text should go
3. Type — the text appears exactly where you tapped
4. Drag to reposition, or re-edit any entry
5. Tap **Done** to commit

Typed text is placed **verbatim**. No AI is involved in placement, so nothing can
garble or delay what you typed. (An optional "Ask AI" affordance exists separately
if you want it — it can never block or alter normal typing.)

## Sign by hand

1. Tap **Sign**
2. Draw your signature — choose **black or blue ink**
3. Place it on the page: drag to position, pinch or use the on-screen buttons to
   resize and rotate
4. Tap **Done**

The signature is **flattened into the page content**, so it survives saving,
re-opening and sharing — it isn't a floating annotation that other viewers drop.

> **Note:** this is a *visual* signature — the handwritten-signature equivalent of
> signing a printed page. It is not a cryptographic/PAdES digital signature.

## Mark up by hand — iPhone & iPad

Handwritten annotation, the way you'd mark up a printed page.

1. Open a PDF and tap **Markup**
2. Write with **Apple Pencil** — or just your finger, on any device
3. Choose pen, marker or highlighter from the system tool palette
4. Move between pages with the **‹ 1/3 ›** arrows — one session can mark up as
   many pages as you like
5. Tap **Done** to commit, or **Cancel** to discard everything

Your handwriting is **written into the page content**, exactly like a signature.
That's what makes it survive saving, exporting, printing and opening in other PDF
apps — the ink is part of the document, not a floating annotation another viewer
can quietly drop.

> **The trade-off, stated plainly:** because the ink is flattened into the page, it
> is **not re-editable afterwards** — you can't select a stroke later to move or
> delete it. Undo works while you're still marking up, and the whole commit is a
> single undo step, so you can reverse it immediately after tapping Done. Beyond
> that, the marks are permanent.

> **iPhone and iPad only.** Handwritten markup is built on PencilKit and has no
> equivalent in the Mac app, so the Mac version does not have this feature.

## Undo and redo

Dedicated **undo and redo buttons** in the toolbar — no keyboard required, which
matters on iPhone and iPad.

## Export or print any document to PDF

Not just PDFs: **any** supported format can be exported to a clean, paginated PDF —
Markdown, JSON, CSV, Mermaid diagrams, LaTeX and the rest. Pagination is
typographic, so headings, paragraphs and fenced code blocks are never sliced across
a page break. Output uses A4 or US Letter automatically based on your region, on a
paper-light theme regardless of the app theme you use.

Exporting to PDF is **free**.

---

## What's free vs Pro

| Action | Free | Pro |
|---|:--:|:--:|
| View PDFs | ✅ | ✅ |
| Export / print any document to PDF | ✅ | ✅ |
| Fill in forms and flat paperwork | | ✅ |
| Sign by hand | | ✅ |
| Mark up by hand *(iPhone & iPad)* | | ✅ |
| AI actions | | ✅ |

Pro is a **one-time purchase**, not a subscription, and unlocks across your Mac,
iPad and iPhone.

## Privacy

PDFs are parsed and rendered entirely on-device. Nothing is transmitted anywhere.
The only time any document content leaves your device is if *you* explicitly run an
AI action with your own API key — see the [FAQ](FAQ.md).
