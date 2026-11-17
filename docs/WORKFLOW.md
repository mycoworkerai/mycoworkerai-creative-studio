# Creative Workflow

**Status: DRAFT**

## Roles in the current toolchain

- **Claude:** assists with copy, art direction, and HTML/CSS source authoring.
- **GitHub:** versioned source of truth for briefs, HTML, assets, and approved deliverables.
- **Gemini:** can access local files when the workflow requires importing the repository or assets into a local environment, and can support review/export steps.

These are workflow responsibilities, not hard technical dependencies. Tools may change while the repository structure remains stable.

## Standard handoff

1. Prepare the brief and visual requirements.
2. Create or update the editable source.
3. Import the source and required assets into this repository.
4. Review the result in the intended environment.
5. Export final deliverables to the matching `exports/` directory.
6. Update the artifact status and commit the approved result.

## Artifact status

- **DRAFT** — work in progress; not approved.
- **IN REVIEW** — ready for review.
- **APPROVED** — approved for reuse or publication.
- **ARCHIVED** — retained for history.

## HTML Story checklist

- [ ] Canvas is 1080 × 1920 px (9:16).
- [ ] Original Myca image asset is linked; character is not recreated as SVG/CSS.
- [ ] All assets use relative paths.
- [ ] Fonts and images load before PNG export.
- [ ] Exported PNG is exactly 1080 × 1920 px.
- [ ] Export UI is excluded from the final image.
- [ ] Final visual and copy review completed.
