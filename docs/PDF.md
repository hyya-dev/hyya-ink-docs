# PDF: view, add text, sign, mark up, save

hYYa ink treats PDFs as first-class documents on Mac, iPad, iPhone and Android. Everything
happens **on your device** — no upload, no cloud conversion service, no account.

**→ [Download hYYa ink](https://hyya.com/hyya-ink.html)**

---

## View a PDF

Open any `.pdf` and it renders in a clean, paginated viewer. On the Mac, hYYa ink
registers as an *alternate* PDF handler, so it appears under **Open With** without
taking over Preview as your default. On Android, hYYa ink appears in the list of apps that can open a PDF, without
becoming your default.

Viewing is **free forever**.

## Add text to a PDF

hYYa ink detects no form fields and never hunts for boxes — you place every piece of
text yourself, at the exact spot you tap. That is what lets it work on flat, scanned
paperwork with no form fields at all, the common case that trips up other tools.

1. Tap **Add Text** in the toolbar (on iPhone, it's in the **•••** Tools menu)
2. Tap anywhere on the page where text should go
3. Type — the text appears exactly where you tapped
4. Drag to reposition, or re-edit any entry
5. Tap **Done** when you have finished adding text

Nothing is written to a file yet — see [Saving](#saving-writes-a-new-file) below.

Typed text is placed **verbatim**. No AI is involved anywhere in this flow — there is
no "interpret this" button, no suggestion, and no network call. You click or tap a spot
and you type.

## Sign by hand

1. Tap **Sign** (on iPhone, in the **•••** Tools menu)
2. Draw your signature — choose **black or blue ink** — and tap **Add signature**
3. Place it on the page: drag to position, pinch or use the on-screen buttons to
   resize and rotate
4. Tap **Place signature** (on Android, **Done**)

Until you save, the undo button can take a placed signature off again; on Android you
can also tap it to move, resize or turn it. When you save, it is **flattened into the
page content of a new file**, so in the copy you send it survives re-opening and sharing
and isn't a floating annotation that other viewers can drop.

> **Note:** this is a *visual* signature — the handwritten-signature equivalent of
> signing a printed page. It is not a cryptographic/PAdES digital signature.

## Mark up by hand

Handwritten annotation, the way you'd mark up a printed page. On **iPhone and iPad**
since 1.2.0; on the **Mac** since 1.2.1; and on **Android**.

**On iPhone and iPad**

1. Open a PDF and tap **Markup** (on iPhone, in the **•••** Tools menu)
2. On **iPad**, write with **Apple Pencil** or a finger; on **iPhone**, with a finger
   (Apple Pencil is iPad-only)
3. Choose pen, marker, pencil or eraser from the system tool palette
4. Move between pages with the **‹ 1/3 ›** arrows — one session can mark up as
   many pages as you like
5. Tap the ✓ (**Done marking up**) to commit, or the ✕ (**Cancel markup**) to discard
   everything

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

**On Android**

1. Open a PDF and tap **Markup**
2. Draw on the pad in one of five ink colours — with a stylus, pressure sets each
   stroke's weight
3. Tap **Done**: the drawing is placed on the page, where you can drag it into position
   and resize it

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
- **It never leaves your device.** Markup is applied entirely on your Mac, iPhone,
  iPad or Android device; nothing is uploaded.

The flip side applies to the **saved copy**, not to your session: once the ink is part
of that new file's page content, it cannot be repositioned or rubbed out there. While
the document is still open, the undo button can take your handwriting off again — and
the original file you opened is never modified either way.

> **To be clear about what this is not:** handwritten markup is a *visual* mark. It
> is not encryption, and not a cryptographic (PAdES) digital signature.

> **Was iPhone and iPad only.** Before 1.2.1 the Mac app had no handwritten markup.
> It does now, with its own trackpad/mouse tool bar — update to 1.2.1 or later.

## Undo

A dedicated **undo button** in the toolbar — no keyboard required, which matters on
iPhone and iPad. On Android, **Undo** is in the **⋮** Tools menu. It steps back one
entry at a time: an added text entry, a signature, or a page's handwriting.

There is **no redo button** in the PDF tools, deliberately. Undo here removes one
pending entry rather than rewinding a whole document, so there is nothing to restore,
and a permanently greyed-out control reads as broken. (Redo does exist on the Mac for
ordinary text editing, at **Edit ▸ Redo**, and inside the signature pad.)

## Saving writes a NEW file

Every tool here — Add Text, Sign, Markup, and each of the document tools below —
leaves the PDF you opened **untouched**. Your edits stay live while the document is
open, and saving — **Save copy…** on the Mac, the save button on iPhone, iPad and
Android — writes them into a **new** file. hYYa ink never overwrites your original.

Saving a copy requires Pro.

## Find, read and navigate

- **Find in document** — every match highlighted at once, with a live count and
  next/previous. ⌘F on the Mac.
- **Pages and contents** — page thumbnails, plus the PDF's own table of contents when
  it has one. Beside the page on the Mac and
  iPad; a sheet on iPhone.
- **Password-protected PDFs** open normally — hYYa ink asks for the password.

All three are **free**, on every platform. On the Mac, Find and the page sidebar are
icon buttons; their names appear as tooltips rather than printed captions. On Android
they are the **Find** and **Pages** buttons.

## Document tools

The document tools — all Pro, on every platform. On iPhone they live in the **•••**
Tools menu; on the Mac and iPad they are in the **•••** menu in the toolbar; on Android,
in the **⋮** Tools menu.

| Tool | What it does |
|---|---|
| **Make Searchable** | On-device text recognition adds a searchable, selectable text layer to a scanned page — so a photographed document can be searched, and its text selected and copied. On Mac, iPad and iPhone it reads many languages and picks the language itself (how many depends on your system version); on Android you choose Latin-alphabet languages or Arabic. Your pages are never uploaded. |
| **Organise Pages** | Reorder, rotate and remove pages, and add the pages of another PDF. |
| **Protect** | Set a password to open the file, and ask PDF apps not to allow printing or copying. |
| **Compress** | The exact before-and-after size is shown before you save. |
| **Watermark** | Live preview as you set the wording and strength. |
| **Compare** | See which pages differ from another PDF. On Mac, iPad and iPhone it compares the words on each page; on Android it compares how each page looks. |
| **Mark Up Text** | Highlight, underline or strike through selected text (on Android, drag across the words). |
| **Redact & Replace** | **Redact** removes selected text permanently (on Android, drag across the words): the page is saved as a picture, so the words leave the file — they cannot be selected, copied or searched in the saved copy. Only the pages you redact become pictures; the other pages keep their text. Text recognition then runs over those pages so the text you kept stays searchable. **Replace** swaps selected text for new text; the original is removed the same way, so the saved file cannot display one value and extract another. |

> **What happens to the rest of a redacted page.** That page becomes an image,
> so hYYa ink immediately re-runs on-device text recognition over it —
> the text you kept stays selectable and searchable. It is *recognised* text rather than
> the original, so on an unusual font it can be imperfect. The redacted words cannot come
> back: the bars are burned in **before** the page is photographed, so the recogniser
> never sees them.

> **What Redact promises, precisely.** It removes the text you select, on the pages you
> redact. It is not a tool for removing a document's metadata, attachments or embedded
> files — it cleans the page, not the whole file. **Replace** removes the original too, so
> never think of it as hiding a value underneath a new one.

> **Make Searchable is not one of the AI actions.** It needs no key and no provider, and
> your pages are never uploaded. On Mac, iPad and iPhone it uses Apple's on-device text
> recognition; on Android, Google's ML Kit (and Tesseract for Arabic), where Google's
> library sends Google its own diagnostics — never your pages.

Every one of these except Compare writes a **new** file; Compare only shows you the
result. The PDF you opened is never modified.

## Export or print any document to PDF

Not just PDFs: **any** supported format can be exported or printed as a PDF. Markdown
comes out as the formatted document. On Mac, iPad and iPhone, Mermaid diagrams,
Graphviz, LaTeX and AsciiDoc come out rendered. Everything else — and those four on
Android — comes out as its text.

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
| Mark up by hand | | ✅ |
| Save a copy with your edits | | ✅ |
| Mark Up Text, Redact & Replace, Make Searchable, Organise Pages, Protect, Compress, Watermark, Compare | | ✅ |
| AI actions *(other formats — not available for PDFs)* | | ✅ |

Pro is a **one-time purchase**, not a subscription, and unlocks across your Mac,
iPad and iPhone. On Android, Pro is a separate one-time purchase through Google Play.

## Privacy

PDFs are parsed and rendered entirely on-device, and their content is never uploaded:
the AI actions aren't available for PDFs. For everything else, see the [FAQ](FAQ.md).
