<p align="center">
  <strong>OFFIXA</strong>
</p>

<p align="center">Deterministic document engines for developers.</p>

<p align="center">
  <a href="https://offixa.dev">Website</a> · <a href="https://docs.offixa.dev">Docs</a> · <a href="https://github.com/offixa-projects">GitHub</a>
</p>

---

## What is OFFIXA?

OFFIXA provides a suite of open-source engines for building, transforming, and rendering documents with **deterministic, reproducible output** — every time, on every platform.

No layout drift. No rendering surprises. Pixel-perfect documents from code.

## Products

| | Product | Description |
|---|---|---|
| **📄** | [**PDFixa Core**](https://github.com/offixa/pdfixa-core) | The foundational engine — parse, build, and render PDFs programmatically. |
| **📦** | [**PDFixa Examples**](https://github.com/offixa/pdfixa-examples) | Ready-to-run templates and recipes: invoices, reports, contracts, and more. |
| **⚡** | [**PDFixa Pro**](https://github.com/offixa-projects/pdfixa-pro) | Advanced features — digital signatures, form filling, batch processing, and enterprise tooling. |

## Start here

**New to OFFIXA?** Follow these steps:

1. **Explore** — Browse [PDFixa Examples](https://github.com/offixa-projects/pdfixa-examples) for real-world use cases.
2. **Install** — Add PDFixa Core to your project and generate your first document.
3. **Go further** — Unlock advanced workflows with PDFixa Pro.

## Quick example

```java
PdfDocument doc = PdfDocument.builder()
    .page(Page.a4()
        .add(Text.of("Hello from OFFIXA")
            .fontSize(24)
            .bold())
        .add(Text.of("Deterministic. Reproducible. Every time.")
            .fontSize(12)
            .color("#6B7280")))
    .build();

doc.save("hello.pdf");
```

## Links

- 🌐 [offixa.dev](https://offixa.dev) — Official website
- 📖 [docs.offixa.dev](https://docs.offixa.dev) — Documentation
- 💬 [Discussions](https://github.com/orgs/offixa-projects/discussions) — Ask questions and share ideas

---

<p align="center"><sub>Built with precision by the OFFIXA team.</sub></p>
