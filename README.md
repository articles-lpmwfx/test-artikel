# Test Artikel

En test-artikel for at verificere hele publish-kæden.

| Format | Rolle | Link |
|--------|-------|------|
| MD | Master (source of truth) | [article/test-artikel.md](article/test-artikel.md) |
| HTML | Public portal | [test-artikel.lpmwfx.com](https://test-artikel.lpmwfx.com) |
| PDF | Autoritativ version | [Releases](../../releases) |

## Build

```bash
# Generate PDF
pandoc article/test-artikel.md -o article/test-artikel.pdf \
  --pdf-engine=xelatex -V lang=da -V geometry:margin=2.5cm

# Preview locally
open article/test-artikel.pdf
```

## Structure

```
article/
  test-artikel.md    ← MASTER (source of truth)
assets/              ← images, diagrams
docs/                ← GitHub Pages (generated)
```
