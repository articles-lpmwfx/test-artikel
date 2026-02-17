---
title: "Test Artikel"
author: "lpmwfx"
date: 2026-02-17
lang: da
description: "En test-artikel for at verificere hele publish-kæden: Markdown → GitHub Pages → PDF"
---

# Test Artikel

Dette er en test-artikel til at verificere den fulde publish-pipeline.

## Hvad tester vi?

1. **Markdown til GitHub repo** — versioneret artikelkilde
2. **GitHub Pages** — automatisk web-publicering
3. **Custom domæne** — `test-artikel.lpmwfx.com` via Njal.la DNS
4. **PDF-generering** — pandoc med xelatex

## Danske tegn

Æble, ørred, ålborg — æøå ÆØÅ virker korrekt.

## Kodeeksempel

```python
def publish(article: str) -> str:
    """Publish an article to the web."""
    return f"Published: {article}"
```

## Konklusion

Hvis du kan læse dette på `test-artikel.lpmwfx.com`, virker hele kæden.
