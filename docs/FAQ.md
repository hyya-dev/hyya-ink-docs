# FAQ

**→ [Download hYYa ink](https://hyya.com/hyya-ink.html)**

## Pricing & licensing

### Is hYYa ink a subscription?
No. Reading and previewing every format — including exporting to PDF — is **free
forever**. Editing, PDF filling/signing and AI actions are unlocked with a **single
one-time purchase**.

### Do I have to buy it twice for Mac and iPhone?
No. The Mac App Store and iOS apps are a **Universal Purchase** — buy once with
your Apple Account and Pro unlocks on your Mac, iPad and iPhone.

### What's the difference between the App Store version and the direct download?
They're the same app through two storefronts. The **App Store** version unlocks via
in-app purchase. The **direct DMG** from hyya.com unlocks with a license key and
updates itself automatically. Because Apple and the direct store are separate
systems, a purchase in one does not carry to the other.

### Is there a trial?
Yes — a full-featured trial so you can try editing, signing and AI before deciding.
When it ends the app keeps working as a free viewer; nothing is locked away or
deleted.

## Privacy & AI

### Does hYYa ink send my documents anywhere?
No. All parsing, rendering, PDF handling and signing happen **on your device**.
There is no account, no server and no telemetry.

### What about the AI features?
AI is strictly **opt-in and bring-your-own-key (BYOK)**. Nothing is sent anywhere
unless you explicitly run an AI action. When you do, only the open document's text
goes to the provider *you* configured with *your* key. hYYa ink has no AI server of
its own and never proxies your content.

On devices with Apple Intelligence, some AI work can run **entirely on-device**
with no network at all.

### Where is my API key stored?
In the system keychain on your device. It is never transmitted to hYYa.

### Which AI providers work?
Any OpenAI-compatible endpoint — OpenRouter, OpenAI, Groq, Together AI, or a custom
endpoint. On macOS you can also point it at a local server such as Ollama or LM
Studio, which keeps everything on your machine.

## Using the app

### Why doesn't my AI key seem to work?
After entering your provider, key and model you must tap **Test & save**. Settings
are only stored once the connection test succeeds — this guarantees the app never
saves a configuration that doesn't work. The app will warn you if you try to leave
with unsaved changes.

### Can it preview files from Finder?
Yes — hYYa ink installs a **Quick Look extension**, so pressing the space bar on
any supported file previews it rendered, without opening the app.

### Will it take over as my default PDF app?
No. hYYa ink registers as an *alternate* handler, so it shows up under **Open
With** while Preview stays your default unless you change it yourself.

### Is the signature legally binding?
It's a **visual** signature — equivalent to signing a printed page by hand, and it
is flattened permanently into the document. It is not a cryptographic/PAdES digital
signature backed by a certificate authority.

## Platforms

### What are the system requirements?
macOS 14 or later; iPadOS/iOS 17 or later.

### Is there an Android or Windows version?
Not today. hYYa ink is a native Apple-platform app.

---

Still stuck? **[Open an issue](https://github.com/hyya-dev/hyya-ink-docs/issues)**
or contact us at [hyya.com/#contact](https://hyya.com/#contact).
