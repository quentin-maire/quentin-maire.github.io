# Quarto academic website — starter

A draft Quarto version of a personal academic site, with pages: About me, Selected publications, Teaching, CV.

## 1. Adding files to folder

CV to be included as `CV.pdf` in this same top-level folder (where this file is).

## 2. Preview locally (optional)

Quarto to be installed from <https://quarto.org/docs/get-started/>, then from this folder run:

```
quarto preview
```

This will opens a live preview in the browser that updates as edits are made. This step saves a round-trip through GitHub Actions for
every small tweak.

## 3. Deploy

1. Create/rename a GitHub repo to `user-name.github.io`.
2. Push this folder's contents via GitHub Desktop (Add local repository → Publish/Push).
3. The included workflow (`.github/workflows/publish.yml`) builds the site
   and pushes it to a `gh-pages` branch itself. So in **Settings → Pages →
   Build and deployment → Source**, choose **"Deploy from a branch"** and
   select the `gh-pages` branch — not "GitHub Actions".
4. The `gh-pages` branch won't exist until the workflow runs once — push to
   `main`, let the Action finish, then the branch (and the option to select
   it) will appear.
