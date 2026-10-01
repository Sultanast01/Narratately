# 📖 Narrately

**Any document, read aloud — free, right in your browser.**

Narrately turns PDFs, Word docs, and text files into something you can listen to instead of read. No installs, no sign-up required to try it, no payment. Open the link, upload a file, hit play.

🔗 **Live app:** [your-live-link-here](https://your-username.github.io/narratately/)

⭐ **If you find this useful, a star on this repo goes a long way** — it's the easiest way to show support and helps others discover it too.

---

## Features

- 📄 Reads **PDF, DOCX, and TXT** files aloud
- 🎙️ Voice picker, sorted to favor clearer British/natural-sounding voices over robotic defaults
- ⏱️ Adjustable reading speed, skip forward/back, drag-to-seek scrubber
- 📚 Personal library — add multiple books, each remembers where you left off
- 🌗 Light, dark, and system theme
- 📱 Installable like an app (Add to Home Screen on iPhone/Android) — opens full-screen, no browser bars
- 🔒 Everything stays on your own device — no account, no server storing your books
- 💬 Built-in feedback box
- 100% free, no catch

## How it works

Everything runs client-side in the browser:
- **pdf.js** extracts text from PDFs
- **mammoth.js** extracts text from Word docs
- The browser's own built-in text-to-speech engine (Web Speech API) reads it aloud — no external API calls, no cost per use
- Your library is saved in your browser's local storage, private to your device

## Running it yourself

This is a single self-contained HTML file — no build step, no dependencies to install.

1. Download `reader.html`
2. Open it directly in a browser, or deploy it anywhere static files are served:
   - **GitHub Pages** — upload it, rename to `index.html`, enable Pages in repo Settings
   - Any static host (Netlify, Vercel, your own server, etc.)

### Optional setup

A few features are off by default and need your own free third-party accounts to activate — the app tells you exactly where to look in the code (search for these names):

| Feature | Service | Code variable |
|---|---|---|
| Waitlist signup gate | [Formspree](https://formspree.io) (free) | `FORMSPREE_ENDPOINT`, `GATE_ENABLED` |
| In-app feedback box | [Formspree](https://formspree.io) (free) | `FEEDBACK_FORMSPREE_ENDPOINT` |
| Visitor analytics | [GoatCounter](https://goatcounter.com) (free) | the `data-goatcounter` script tag |

None of these are required to use the app — it works fully free and open with all of them left as placeholders.

## Built in public

This was built as part of the **Emergence Challenge** — a 21-day build-and-learn-in-public challenge. Feedback, issues, and ideas welcome.

---

If Narrately saved you a trip to the gym without your headphones, or got a book read that was gathering dust — that's what this was built for. Enjoy, and feel free to star ⭐ or share with anyone who'd find it useful.
