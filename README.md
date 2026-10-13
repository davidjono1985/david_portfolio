# David Johnson — portfolio

Static site published with GitHub Pages: https://davidjono1985.github.io/david_portfolio/

Plain HTML and CSS, no build step. Edit `index.html` and `style.css` directly. All paths are relative so the site works under `/david_portfolio/`.

- `index.html` — the portfolio
- `projects/` — detail pages for early (bootcamp) work, kept at their original URLs
- `docs/VERIFICATION.md` — outstanding fact and link checks

## Rollback to the original portfolio

The site as published before the October 2026 redesign is preserved at commit
`6413c39d046004284ec785db0c24d34f14eecd18` (master, "updated tech stack", 2020-08-10) and on the remote branch
`portfolio-before-redesign-2026-10-13`, which points at exactly that commit. (An annotated tag could not be pushed from the
build environment, so a branch is used instead.) It is also viewable at `/archive/original/` on the live site.

To restore it, either revert the redesign merge on `master`:

    git revert -m 1 <redesign-merge-commit>

or restore the old files without touching history:

    git fetch origin portfolio-before-redesign-2026-10-13
    git checkout origin/portfolio-before-redesign-2026-10-13 -- .
    git rm -r -q archive docs photo/projects   # folders added by the redesign
    git commit -m "Restore original portfolio"

Do not delete the backup branch.
