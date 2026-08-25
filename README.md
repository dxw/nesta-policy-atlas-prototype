# Policy Atlas — design documentation

Static site. Every page is a single self-contained HTML file: no build step, no
dependencies, no network calls. Open any of them directly in a browser or serve
the folder as-is.

## Pages

| URL | Page |
| --- | --- |
| `index.html` | Overview |
| `principles.html` | Design principles |
| `patterns.html` | AI patterns |
| `habits.html` | Team habits |
| `prototype-notes.html` | Prototype notes |
| `brand.html` | Brand |
| `design-system.html` | Design system (branding, components, pages) |
| `roadmap.html` | Roadmap |
| `prototype.html` | Working prototype — new search |
| `completed-run.html` | Prototype — completed run |
| `sources.html` | Prototype — sources |
| `splash.html` | Marketing splash page |

`completed-run.html` and `sources.html` are reached from inside the prototype
rather than the documentation nav.

## Deploying to GitHub Pages

1. Push the contents of this folder to a repository.
2. Settings → Pages → Source: **Deploy from a branch**.
3. Branch `main`, folder `/` if this folder is the repository root, or `/docs`
   if you copied it to `docs/`.

`.nojekyll` is present so Jekyll leaves the files alone.

## Editing

Do not edit these files. They are compiled. The editable sources are the
`.dc.html` files in the design project; `stage/` holds the same sources with
the site's URLs substituted, and each page is recompiled from there.
