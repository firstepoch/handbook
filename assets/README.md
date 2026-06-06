# Assets

Static assets for the handbook.

## Conventions

- **`logo-square.png`** — square site logo shown in the sidebar (and used as the
  favicon). Referenced from `_quarto.yml` under `book.sidebar.logo`. If it is
  ever missing, drop a square PNG here at that exact filename and the build
  picks it up automatically.
- **`images/`** — captioned figures and screenshots. Reference them from
  chapters and add a caption + cross-reference label, e.g.:

  ```markdown
  ![A descriptive caption.](assets/images/example.png){#fig-example}
  ```

  then cite with `@fig-example`.
