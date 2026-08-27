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

## Add text to a PDF

hYYa ink detects no form fields and never hunts for boxes — you place every piece of
text yourself, at the exact spot you tap. That is what lets it work on flat, scanned
paperwork with no form fields at all, the common case that trips up other tools.

1. Tap **Add Text** in the toolbar
2. Tap anywhere on the page where text should go
3. Type — the text appears exactly where you tapped
4. Drag to reposition, or re-edit any entry
5. Tap **Done** when you have finished adding text

Nothing is written to a file yet — see [Saving](#saving-writes-a-new-file) below.

Typed text is placed **verbatim**. No AI is involved anywhere in this flow — there is
no "interpret this" button, no suggestion, and no network call. You click or tap a spot
and you type.

## Sign by hand

1. Tap **Sign**
2. Draw your signature — choose **black or blue ink**
3. Place it on the page: drag to position, pinch or use the on-screen buttons to
   resize and rotate
4. Tap **Done**

Your signature stays **adjustable for as long as the document is open** — reposition,
resize or remove it. When you save, it is **flattened into the page content of a new
file**, so in the copy you send it survives re-opening and sharing and isn't a floating
annotation that other viewers can drop.

> **Note:** this is a *visual* signature — the handwritten-signature equivalent of
> signing a printed page. It is not a cryptographic/PAdES digital signature.

## Mark up by hand — Mac, iPhone & iPad

Handwritten annotation, the way you'd mark up a printed page. On **iPhone and iPad**
since 1.2.0; on the **Mac** since 1.2.1.

**On iPhone and iPad**

1. Open a PDF and tap **Markup**
2. On **iPad**, write with **Apple Pencil** or a finger; on **iPhone**, with a finger
   (Apple Pencil is iPad-only)
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

When you save, your handwriting is **written into the page content of the new file**,
exactly like a signature. That's what makes it survive exporting, printing and opening
in other PDF apps — in the saved copy the ink is part of the document, not a floating
annotation another viewer can quietly drop.

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

The flip side applies to the **saved copy**, not to your session: once the ink is part
of that new file's page content, it cannot be repositioned or rubbed out there. While
the document is still open, everything stays adjustable — and the original file you
opened is never modified either way.

> **To be clear about what this is not:** handwritten markup is a *visual* mark. It
> is not encryption, and not a cryptographic (PAdES) digital signature.

> **Was iPhone and iPad only.** Before 1.2.1 the Mac app had no handwritten markup.
> It does now, with its own trackpad/mouse tool bar — update to 1.2.1 or later.

## Undo

A dedicated **undo button** in the toolbar — no keyboard required, which matters on
iPhone and iPad. It steps back one entry at a time: an added text entry, a signature,
a markup stroke.

There is **no redo button** in the PDF tools, deliberately. Undo here removes one
pending entry rather than rewinding a whole document, so there is nothing to restore,
and a permanently greyed-out control reads as broken. (Redo does exist on the Mac for
ordinary text editing, at **Edit ▸ Redo**, and inside the signature pad.)

## Saving writes a NEW file

Every tool here — Add Text, Sign, Markup, and each of the document tools below —
leaves the PDF you opened **untouched**. Your edits stay live and adjustable while the
document is open, and **Save copy…** writes them into a **new** file. hYYa ink never
overwrites your original.

Saving a copy requires Pro.

## Find, read and navigate

- **Find in document** — every match highlighted at once, with a live count and
  next/previous. ⌘F on the Mac.
- **Pages and contents** — page thumbnails, plus the PDF's own table of contents when
  it has one. A sidebar on the Mac; a sheet on iPhone and iPad.
- **Password-protected PDFs** open normally — hYYa ink asks for the password.

All three are **free**, on Mac, iPhone and iPad. On the Mac, Find and the page sidebar
are icon buttons; their names appear as tooltips rather than printed captions.

## Document tools

Seven more tools, all Pro, all on Mac, iPhone and iPad. On iPhone they live in the
**•••** Tools menu; on the Mac they are in the **•••** menu in the toolbar.

| Tool | What it does |
|---|---|
| **Make Searchable** | On-device text recognition adds a searchable, selectable text layer to a scanned page — so a photographed document can be searched, selected, and read by the AI actions. Around thirty languages, detected automatically. Nothing is uploaded. |
| **Organise Pages** | Reorder, rotate and remove pages, and insert pages from another PDF. |
| **Protect** | Set an open password, and choose whether printing and copying are allowed. |
| **Compress** | The exact before-and-after size is shown before you save. |
| **Watermark** | Live preview as you set the wording and strength. |
| **Compare** | See which pages differ between two versions of a document. |
| **Mark Up Text** | Highlight, underline or strike through selected text. |

> **Make Searchable is not AI.** It is Apple's on-device Vision text recognition. It
> runs entirely on your device and sends nothing anywhere.

Every one of these writes a **new** file. The PDF you opened is never modified.

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
| Find in document | ✅ | ✅ |
| Pages and contents | ✅ | ✅ |
| Open a password-protected PDF | ✅ | ✅ |
| Add text to a PDF | | ✅ |
| Sign by hand | | ✅ |
| Mark up by hand *(Mac, iPhone & iPad)* | | ✅ |
| Save a copy with your edits | | ✅ |
| Mark Up Text, Make Searchable, Organise Pages, Protect, Compress, Watermark, Compare | | ✅ |
| AI actions | | ✅ |

Pro is a **one-time purchase**, not a subscription, and unlocks across your Mac,
iPad and iPhone.

## Privacy

PDFs are parsed and rendered entirely on-device. Nothing is transmitted anywhere.
The only time any document content leaves your device is if *you* explicitly run an
AI action with your own API key — see the [FAQ](FAQ.md).
