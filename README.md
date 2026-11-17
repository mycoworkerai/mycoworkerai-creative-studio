# My Coworker AI — Creative Studio

> **Status: DRAFT**

A centralized workspace for developing, organizing, reviewing, and exporting the visual content and creative assets of **My Coworker AI**.

This repository is the source of truth for brand creative work. It is designed to support the character library, social campaigns, HTML-based layouts, motion graphics, and reusable visual assets without tying the project to a single production tool.

## Current focus

- Establish the official Myca character asset library (2D and 3D).
- Organize Instagram Stories and feed content.
- Store editable HTML source files and export-ready templates.
- Keep original assets separate from generated layouts and final exports.
- Preserve creative decisions and revisions through Git history.

## Production workflow

1. **Create** — develop copy, visual direction, and layouts in the appropriate tools.
2. **Import** — add source files and approved assets to this repository.
3. **Review** — inspect the work in the target environment (including Gemini when local asset access is needed).
4. **Export** — generate final PNG/video deliverables and store them in the relevant export directory.
5. **Archive** — retain source files and approved outputs with clear version/status labels.

Typical handoff:

`Claude (HTML/source authoring) → GitHub (versioned source of truth) → Gemini (local asset access and review) → Export`

## Repository structure

```text
.
├── assets/
│   └── myca/                 # Approved character artwork and visual assets
├── brand/
│   ├── guidelines/           # Brand identity, palette, typography, usage
│   └── references/           # Approved moodboards and visual references
├── campaigns/
│   └── instagram/
│       ├── stories/          # Story source files and briefs
│       └── posts/            # Feed/carousel source files and briefs
├── exports/
│   └── instagram/            # Final PNG exports, grouped by format
├── motion/
│   ├── projects/             # Motion design source projects
│   └── exports/              # Rendered motion deliverables
├── templates/
│   └── html/                 # Reusable HTML creative templates
└── docs/                     # Workflow, production notes, and decisions
```

## Status convention

All newly scaffolded materials begin as **DRAFT**. Use these labels consistently:

- **DRAFT** — initial structure or work in progress; not approved.
- **IN REVIEW** — ready for visual, copy, or technical review.
- **APPROVED** — approved for reuse or publication.
- **ARCHIVED** — retained for history; no longer active.

A file's status should describe the artifact itself, not imply that the entire repository is approved.

## Asset and file conventions

- Keep original character artwork in `assets/`; do not redraw approved character artwork in HTML or SVG.
- HTML files should reference assets using relative paths so the project remains portable.
- Keep editable source files alongside their briefs; store final exports separately.
- Prefer descriptive, lowercase, kebab-case filenames.
- Do not commit credentials, API keys, private user data, or unrelated application source code.
- Avoid duplicate copies of the same asset. Use a clear canonical filename and reference it.

## Initial scope

The repository is a creative production workspace, not the My Coworker AI application source repository. Product screenshots, social content, brand assets, and motion deliverables belong here only when they are intended as creative materials.

---

**Repository status: DRAFT**  
**Maintainer:** My Coworker AI  
