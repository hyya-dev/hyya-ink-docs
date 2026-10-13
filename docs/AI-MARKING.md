# How hYYa ink marks AI-written text

In hYYa ink for Android, iPhone and iPad, the **Explain** and **Summarize** actions write new text with an AI
service you choose. That text carries an invisible mark saying it was written by AI, as the EU AI
Act asks of AI-generated text (Article 50(2)). It is shown on screen with the words
**"Written by AI"** and the model's name, and the mark goes with the text when you copy it.

**Reformat**, **Fix errors** and **Make diagram** are not marked: they tidy or correct your own
document, or write diagram code.

## What the mark is

Twenty-four invisible characters, standing for 24 bits, most significant bit first:

- `U+200B` (ZERO WIDTH SPACE) is a **0**, `U+200C` (ZERO WIDTH NON-JOINER) is a **1**;
- the bits spell three bytes: `0x01` (version 1), then `0x41 0x49` — "AI" in ASCII.

Both characters are invisible "format" characters that every text renderer is told to ignore, so the
text looks, reads aloud and searches exactly as before. One mark is placed in each line, right after
the line's first plain word that a space follows. Code, links, addresses and Markdown markup are
never touched.

## How to detect it

Look for the 24-character sequence anywhere in the text:

```python
ZERO, ONE = "\u200b", "\u200c"  # ZERO WIDTH SPACE, ZERO WIDTH NON-JOINER
MARK = "".join(ONE if (byte >> bit) & 1 else ZERO
               for byte in (0x01, 0x41, 0x49) for bit in range(7, -1, -1))

def written_by_ai(text: str) -> bool:
    return MARK in text

def without_the_mark(text: str) -> str:
    return text.replace(MARK, "")
```

Any part of a marked text that holds a whole line still carries that line's mark.

## What it cannot do

The mark travels with copied text, but it does not survive retyping, a screenshot read back by OCR,
translation, rewording, or a tool that removes invisible characters. A line without spaces — most
Chinese and Japanese text — carries no mark. Very short texts are exempt from marking under the
Commission's Code of Practice in any case.

Questions: [hyya.com/#contact](https://hyya.com/#contact).
