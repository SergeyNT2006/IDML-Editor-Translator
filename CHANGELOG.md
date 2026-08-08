# Changelog

All notable changes to IDML Editor-Translator are documented here.

## [0.1.0] — 2026-08-08

### Added

- Product identity: name, identifier `com.sergeynt.idmleditor`, data folder `IDMLEditor`, env prefix `IDMLEDITOR_*`
- **IDML** open / edit / save round-trip (Stories `Content` text); verified openable in InDesign
- Segment table: search, state filters, **column sort**, story banding (IDML)
- **File → Estimate…** — billable volume (chars with/without spaces; numeric-only skipped)
- **File → Export / Import Excel…** — Target exchange for external editors
- QA panel toggle; debounced QA; mergeDocument identity reuse; background cache learn
- **Network** kill-switch (cloud off; local LLM on localhost still allowed)
- Optional **LLM** presets: Ollama, LM Studio, OpenAI, OpenRouter, Custom
- Proprietary LICENSE; Windows portable packaging (`readme.txt` / `quickstart.txt`)
- Store: [Payhip $49](https://payhip.com/b/7Q3Cg); PayPal email delivery — [`docs/BUY.md`](docs/BUY.md)
- Bonus formats: Illustrator XLIFF/XML ([Export-Import text for Illustrator](https://payhip.com/b/pI8NY)), Markdown (markup hidden), plain text, generic XML

### Removed

- In-app **license key** stub (no activation)

### Notes

- Paid InDesign IDML product; buyers receive the portable build (no key).
