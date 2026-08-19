# abdelkbirnainiaa.me

Personal site for Abdelkbir Nainiaa, served by GitHub Pages at
<https://abdelkbirnainiaa.me>.

## What's here

| File | Purpose |
|---|---|
| `index.html` | The whole site — markup, styles and script in one file, no build step |
| `CNAME` | Binds `abdelkbirnainiaa.me` to this Pages site |

## Editing it

There is no toolchain. Edit `index.html` and push to `main`; Pages redeploys.

The content that changes most often is near the bottom of the file:

- **Assertions** — the `<li class="assert">` items in `#asserts`. The `data-ms`
  attribute is that row's timing; the summary totals them automatically.
- **Projects** — the `<a class="spec">` blocks under *Selected work*.
- **Stack** — the `<div class="row">` pairs under *Stack*.

## Design

The page is built as a passing test suite: the claims resolve from pending to
`✓` on load, with a run bar counting up and a summary line. The conceit is the
argument — the work is about shipping software with a suite and a pipeline, so
the page demonstrates that rather than asserting it.

| Token | Light | Dark | Role |
|---|---|---|---|
| `--paper` | `#F7F7F5` | `#10131A` | Page ground |
| `--raised` | `#FFFFFF` | `#161A23` | Cards |
| `--ink` | `#14181F` | `#E8EAED` | Body text |
| `--muted` | `#626B7A` | `#98A1B0` | Secondary text |
| `--pass` | `#12735A` | `#3FB58C` | Passing status |
| `--cobalt` | `#1E3FB8` | `#8AA0F7` | Accent, focus rings |

Type: **Archivo** for display, **IBM Plex Sans** for body, **IBM Plex Mono** for
assertions, timings and tags.

Every foreground/background pair meets WCAG AA in both themes (lowest ratio
5.02:1). The run animation is skipped entirely under `prefers-reduced-motion`,
which renders every assertion as already passed.

## Checks

```bash
# no horizontal overflow at any width, no mechanical layout violations
open index.html
```

Verified: AA contrast in both themes, visible keyboard focus, skip link, no
horizontal overflow from 500px to 1440px, reduced-motion path, `aria-live` on
the async run.
