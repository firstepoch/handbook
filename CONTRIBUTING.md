# Contributing

Our workflow keeps the published handbook clean while letting chapters be
drafted in the open.

## Workflow

1. **Branch.** Start each chapter on its own feature branch off the default
   branch (`main`):

   ```bash
   git checkout main && git pull
   git checkout -b draft/<chapter-name>
   ```

2. **Write & preview.** Author your chapter `.qmd` and preview locally with hot
   reload:

   ```bash
   quarto preview
   ```

   Add the chapter file to the `chapters:` list in `_quarto.yml`. Put figures in
   `assets/images/` and cite sources via `references.bib`.

3. **Open a PR.** Push the branch and open a pull request against `main` for
   review. Opening a PR does **not** publish anything — only merges to `main`
   trigger a deploy.

4. **Merge to publish.** Once approved and merged to `main`, the
   `.github/workflows/publish.yml` GitHub Action renders the book and deploys it
   to GitHub Pages.

## Drafts (merged but not ready)

To merge a chapter to `main` without publishing it yet, add `draft: true` to its
front matter:

```yaml
---
title: "My Chapter"
draft: true
---
```

With `draft-mode: gone` (set in `_quarto.yml`), draft chapters are excluded from
the published build entirely — no page, no sidebar link, no search entry.
Remove the flag when the chapter is ready to go live.
