# AGENTS.md

## Standard

This book follows the [QuadriviumPress MyST baseline](https://github.com/QuadriviumPress/bindery/blob/main/doc/myst-baseline.md) and the [presentation skill](https://github.com/QuadriviumPress/bindery/blob/main/skills/quadrivium-myst-presentation/SKILL.md).

## Commands

```bash
npm run start
npm run build
npm run verify
npm run check
npm run extract
```

`npm run check` is the production-equivalent verification and HTML build.

## Intentional differences

- `verify` runs `python3 scripts/verify_book.py`.
- `extract` (`python3 scripts/convert_pdf.py`) rebuilds Markdown from the source PDF. It is not part of `check`.
- Front matter, chapters, and back matter are split across `front/`, `chapters/`, `back/`, and `appendices/`.

## Presentation gap

Learning objectives, definitions, sample problems, and practice problems are `{admonition}` blocks. Solutions live in an appendix rather than `{solution}` dropdowns, and there is no `{exercise}` directive. That active-learning layout is kept until a later presentation pass.
