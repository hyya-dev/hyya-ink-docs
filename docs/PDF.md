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

## Mark up by hand — Mac, iPhone & iPad

Handwritten annotation, the way you'd mark up a printed page. On **iPhone and iPad**
since 1.2.0; on the **Mac** since 1.2.1.

**On iPhone and iPad**

1. Open a PDF and tap **Markup**
2. Write with **Apple Pencil** — or just your finger, on any device
3. Choose pen, marker or highlighter from the system tool palette
4. Move between pages with the **‹ 1/3 ›** arrows — one session can mark up as
   many pages as you like
5. Tap **Done** to commit, or **Cancel** to discard everything

**On the Mac**

1. Open a PDF and click **Markup**
2. Draw with your **trackpad or mouse**
3. Pick pen, marker, pencil or eraser, one of five ink colours, and the thickness —
   from hYYa ink's own tool bar at the bottom of the page
4. Move between pages with the **‹ 1/3 ›** arrows, exactly as on iPad
5. Click **Done** to commit, **Cancel** (or **Esc**) to discard everything

The Mac has its own drawing surface because Apple's PencilKit provides the ink
itself but no ready-made canvas or tool palette on macOS. The strokes are the same
real PencilKit ink as on iPad, flattened into the page the same way — so a document
marked up on a Mac is indistinguishable from one marked up on an iPad. Since a mouse
reports no pressure, stroke width follows your **speed** instead: move quickly and
the line tapers, like a real pen.

Your handwriting is **written into the page content**, exactly like a signature.
That's what makes it survive saving, exporting, printing and opening in other PDF
apps — the ink is part of the document, not a floating annotation another viewer
can quietly drop.

**Why it works this way — and why that's the point:**

- **Nobody can strip your marks.** Most PDF apps store annotations as a separate
  layer, and most let a recipient select one and delete it — or "remove all
  comments" in a single click. Ink written into the page isn't a removable object,
  so it can't be quietly taken out.
- **No hidden author data travels with it.** PDF comment layers routinely embed the
  author's name and timestamps. There's no annotation object here, so there's
  nothing like that riding along inside the file you send.
- **It renders everywhere.** Export it, print it, email it, open it on Windows —
  the marks are simply part of the document.
- **It never leaves your device.** Markup is applied entirely on your Mac, iPhone
  or iPad; nothing is uploaded.

The flip side is the same property: because the ink becomes part of the page, you
can't reposition or rub out a stroke later. Undo works while you're marking up, and
the whole session can be undone right after you tap **Done** — after that the marks
are permanent, exactly as if you'd used a real pen on paper.

> **To be clear about what this is not:** handwritten markup is a *visual* mark. It
> is not encryption, and not a cryptographic (PAdES) digital signature.

> **Was iPhone and iPad only.** Before 1.2.1 the Mac app had no handwritten markup.
> It does now, with its own trackpad/mouse tool bar — update to 1.2.1 or later.

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
| Mark up by hand *(Mac, iPhone & iPad)* | | ✅ |
| AI actions | | ✅ |

Pro is a **one-time purchase**, not a subscription, and unlocks across your Mac,
iPad and iPhone.

## Privacy

PDFs are parsed and rendered entirely on-device. Nothing is transmitted anywhere.
The only time any document content leaves your device is if *you* explicitly run an
AI action with your own API key — see the [FAQ](FAQ.md).
