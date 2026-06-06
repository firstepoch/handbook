# FirstEpoch Handbook

The FirstEpoch Handbook is a [Quarto](https://quarto.org) book — a
sidebar-navigated, searchable web handbook for FirstEpoch. It is written as a
collection of `.qmd` chapters, themed with a light accent style, and published
automatically to GitHub Pages at
<https://firstepoch.github.io/handbook/> whenever changes merge to the default
branch. Chapters can carry citations, cross-references, math, code highlighting,
captioned figures, and embeds (Datawrapper iframes, YouTube videos).

## Local build

You'll need [Quarto](https://quarto.org/docs/get-started/) installed.

```bash
# Live preview with hot reload (opens in your browser):
quarto preview

# One-off full render into _book/:
quarto render
```

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for the branch / preview / PR workflow
and how to hide work-in-progress chapters with `draft: true`.
