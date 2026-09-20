# CV

Static personal site hosted on GitHub Pages from the `main` branch.

Live at https://oliviavoster.github.io/CV/

## Files

| Path | Purpose |
|---|---|
| `index.html` | The site |
| `styles.css` | All styling, shared by every page |
| `assets/` | Images |
| `.nojekyll` | Tells Pages to serve files as-is instead of running Jekyll |

## Editing

Edit, commit, push to `main`. Pages rebuilds automatically and the change is live in under a minute.

To preview locally, open `index.html` in a browser — there is no build step.

## A tailored version for one employer

Copy `index.html` into a new directory named after the company, then fix the two
relative paths so they point one level up:

    mkdir acme-corp
    cp index.html acme-corp/index.html

In `acme-corp/index.html`, change `styles.css` to `../styles.css` and
`assets/olivis.png` to `../assets/olivis.png`.

That version is then live at `/CV/acme-corp/` while the main one stays at `/CV/`.
Every version is reachable at the same time, and editing `styles.css` restyles
all of them.

Directories are not listed anywhere on the site, so a version is only findable by
someone you gave the link to — though anyone can read this public repo.
