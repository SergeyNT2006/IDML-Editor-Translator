# IDML Editor-Translator

[![Version](https://img.shields.io/badge/version-0.1.0-green)](CHANGELOG.md)
[![License: Proprietary](https://img.shields.io/badge/License-Proprietary-red.svg)](LICENSE)
[![Buy on Payhip](https://img.shields.io/badge/Buy-$49-blue)](https://payhip.com/b/7Q3Cg)

**Paid, portable Windows companion** focused on Adobe InDesign **IDML** — open a package, edit or translate story text (manually or with a local/cloud LLM), check light QA, estimate volume for quoting, optionally exchange Targets via Excel, and save a package that opens cleanly back in InDesign.

The same workflow also works on **bonus formats**: Illustrator XLIFF/XML, Markdown, plain text, and generic XML (see [Supported formats](#supported-formats)).

> **Not a CAT tool.** This is not Trados, memoQ, or SmartCAT. It is a focused text-segment editor with optional LLM assist — primarily for IDML, with useful extras for Illustrator and everyday text files.

**No in-app license key.** You receive a portable ZIP after purchase.

### Buy

| Channel | Delivery |
|---|---|
| **[Product page](https://sergeynt2006.github.io/IDML-Editor-Translator/#buy)** | Payhip (instant) or PayPal button (email link within 2–3 hours) |
| **[Payhip — $49](https://payhip.com/b/7Q3Cg)** | Instant download after payment |

Details: [`docs/BUY.md`](docs/BUY.md) · site source: `docs/index.html`

---

## Privacy & network

- Documents are processed **on your PC**. The app does **not** upload files to vendor servers; no mandatory account; no vendor telemetry.
- **Network** toolbar switch:
  - **On** — cloud LLM and opening external links are allowed.
  - **Off** — **all** app cloud/internet traffic is blocked (including external links). Manual edit, Autofill, Estimate, Excel, Save keep working. **Local** LLM on `localhost` (Ollama / LM Studio) still works.
- For confidential work: leave **Network Off**, translate manually, or use a **local** LLM so source text never leaves the machine. Cloud APIs receive only segment text you explicitly send via **Translate**.

---

## Who it is for

| Audience | Why it helps |
|---|---|
| **Freelance translators** | IDML without a full CAT stack; optional local/cloud LLM + cache; Excel round-trip; **Illustrator XLIFF/XML** from Export-Import text for Illustrator |
| **Privacy-conscious users** | **Network Off** blocks the cloud; local LLM (Ollama / LM Studio) or fully manual workflow |
| **Correctors / editors** | Fast Source/Target table, QA, undo, Mark Translated — for InDesign **and** Illustrator exports |
| **Prepress / DTP (InDesign)** | Keep styles and package structure; only story `<Content>` text changes; save opens in InDesign |
| **Illustrator users** | Translate **XLIFF or XML** from **[Export-Import text for Illustrator](https://payhip.com/b/pI8NY)**, then import back with that plugin |
| **Markdown / docs workers** | Edit **`.md`** while **markup stays hidden** from editing |
| **Anyone with plain `.txt`** | Quick **volume estimate**, short translate, stats |
| **Agencies / PMs** | **File → Estimate…**; Excel for freelancers without this app |
| **Teams on locked PCs** | Portable mode (`portable.txt` → `.\data`) |

---

## Supported formats

### Primary — Adobe InDesign IDML

- Open / edit / save **`.idml`**
- Translates story text in `Stories` (`<Content>`); styles and package structure are preserved
- Round-trip verified: saved packages open in InDesign

### Bonus — Adobe Illustrator (recommended workflow)

Use with the author’s Illustrator plugin **[Export-Import text for Illustrator](https://payhip.com/b/pI8NY)**:

1. Export text from Illustrator → **XLIFF** or **XML** (single or batch).
2. Open that file here, translate Targets (manual / LLM / Autofill).
3. Save, then **import** the file back into Illustrator with the same plugin.

### Bonus — Markdown

- Open **`.md` / `.markdown`**
- Segments show **readable text**; **markup is not edited in the table** (Fmt chips show structure; raw markup reinjected on save)

### Bonus — Plain text

- Open **`.txt`** (paragraph-oriented)
- Ideal for **quick jobs**: character estimate, short translations, smoke tests

### Bonus — Generic XML

- Open arbitrary XML, pick leaf tags with text, edit Targets, save reinject

---

## What you get (v0.1)

- Segment table: search, state filters, view sort (ID / Source / Target / State), undo
- Story banding (IDML), Autofill, Mark Translated (**Ctrl+A**)
- **Optional LLM** (see below) + **local** translation cache
- QA panel (on/off), **Network** kill-switch for privacy
- **File → Estimate…** — volume for quoting
- **File → Export / Import Excel…** — Target hand-off for external editors
- Portable packaging for Windows

---

## Optional LLM translation

Manual editing always works with **no** AI and **Network Off**.

**Setup:** Settings → Preferences → **LLM connection…**

| Preset | Typical use |
|---|---|
| **Ollama (local)** | Private on-PC models (`http://localhost:11434/v1`) — works with Network Off |
| **LM Studio (local)** | Private local server (often `http://localhost:1234/v1`) — Network Off OK |
| **OpenAI** / **OpenRouter** / **Custom** | Cloud OpenAI-compatible `/v1` APIs — need Network On, internet, API key |

**Run:** toolbar **Translate empty…** or **Translate selection…** → confirm → **Start**. Local **translation cache** can fill repeats without a new API call.

---

## How to use (IDML)

1. In InDesign, export or package as **IDML**.
2. Open the `.idml` in **IDML Editor-Translator**.
3. Answer **Copy source to target?** — Yes to prefill Targets.
4. Edit **Target**, optional LLM, Mark Translated (**Ctrl+A**).
5. Optional: **Estimate…**, or **Export Excel…** → **Import Excel…** when done.
6. Check **QA**, then **File → Save** (`.bak` when overwriting).
7. Open the saved IDML in InDesign.

A sample IDML is included in the portable ZIP (`samples\`).

---

## Purchase & support

- **Buy page:** [sergeynt2006.github.io/IDML-Editor-Translator/#buy](https://sergeynt2006.github.io/IDML-Editor-Translator/#buy) — **$49**
- **Payhip (instant):** [payhip.com/b/7Q3Cg](https://payhip.com/b/7Q3Cg)
- Companion Illustrator plugin: **[Export-Import text for Illustrator](https://payhip.com/b/pI8NY)**
- Author: Sergey Inozemtsev · `sinozemez@gmail.com`

Proprietary terms: [LICENSE](LICENSE).
