# Project: Strength Log

A single-page static workout tracker (`index.html` + `svgs/`) deployed to GitHub Pages on push to `main`.

## Workflow preferences

- **Always auto-merge feature PRs to `main`** without asking. Use squash merges. The user has explicitly opted into this — do not pause to confirm.
- After merging, the GitHub Pages workflow (`.github/workflows/pages.yml`) deploys automatically. The `github-pages` environment is gated to the default branch (`main`), so feature-branch PR runs will fail their deploy step — that's expected; the post-merge run on `main` is what matters.
- Delete merged feature branches when GitHub doesn't auto-clean them.

## Deploy gotcha

If a deploy fails on `main`, the most likely cause is **Settings → Pages → Source** not being set to **GitHub Actions**. That's a manual UI setting; flag it to the user rather than trying to fix from code.

## Site

Live URL: https://rnbhome.github.io/workout/
