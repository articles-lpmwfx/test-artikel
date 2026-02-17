---
title: "Test Article"
author: "lpmwfx, Denmark, EU"
date: 17.02.2026
lang: en
description: "A test article verifying the full publish chain: Markdown, GitHub Pages, custom domain, and PDF generation."
---

![lpmwfx articles](../assets/badge.png)

# Test Article

This is a test article to verify the complete publishing pipeline from source to distribution.

## What We Are Testing

1. **Markdown to GitHub repo** — versioned article source, single source of truth
2. **GitHub Pages** — automatic web publishing via `docs/` directory
3. **Custom domain** — `test-artikel.lpmwfx.com` with DNS via Njal.la
4. **PDF generation** — pandoc with xelatex, distributed as tagged release
5. **Mistral Small proofreading** — automated spelling, grammar, and punctuation check
6. **Mermaid diagrams** — rendered client-side in HTML, pre-rendered PNG for PDF
7. **drawsvg graphics** — programmatic SVG generation with Python

## The Pipeline

The article flows through these stages:

![Publishing pipeline](../assets/pipeline.png)

- **Author** writes the draft (Danish or English)
- **Claude** formats and structures the Markdown
- **Mistral Small** handles translation and proofreading
- **Pandoc** generates HTML for the web and PDF for distribution
- **Local preview** confirms everything before publishing
- **Git push** and **GitHub release** make it public

## Character Support

European characters render correctly across all formats:

- Danish: æ ø å — Æ Ø Å
- German: ä ö ü ß
- French: é è ê ë ç

## Code Example

```python
def publish(article: str) -> str:
    """Publish an article to the web."""
    return f"Published: {article}"
```

## Conclusion

If you can read this at `test-artikel.lpmwfx.com` and download the PDF from the release page, the entire chain is working.
