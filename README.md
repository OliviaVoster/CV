# CV

Static personal site hosted on GitHub Pages from the `main` branch.

Live at https://oliviavoster.github.io/CV/

## Layout

Pages serves the repo root, so whatever sits at the root **is** the site. Each
version of the site gets its own directory, and the root holds whichever one is
currently the front door.

| Path | Serves at | Purpose |
|---|---|---|
| `index.html` | `/CV/` | Placeholder front page, to be replaced by the new site |
| `v1/` | `/CV/v1/` | The first CV — self-contained, its own HTML, CSS and images |
| `.nojekyll` | — | Tells Pages to serve files as-is instead of running Jekyll |

Every version directory is self-contained, so its internal links stay relative
and nothing breaks when a directory is renamed or moved.

## Adding the new site

Build it in its own directory first, for example `v2/`. It is live at `/CV/v2/`
the moment it is pushed, and the front page is untouched while you work.

When it is ready, promote it by replacing the root `index.html` with the new
site's files — or by pointing the root page at it.

## Editing

Edit, commit, push to `main`. Pages rebuilds automatically and the change is live
in under a minute.

To preview locally, open the `index.html` you care about in a browser — there is
no build step.
