# raghavkansal.com

Personal academic site, built on the
[HugoBlox Academic CV](https://github.com/HugoBlox/theme-academic-cv) template
(the actively-maintained successor to the wowchemy Academic theme this site
used through early 2026).

Deployed via [Netlify](https://www.netlify.com/) — see [`netlify.toml`](netlify.toml)
for the build pipeline (Hugo Extended 0.161 + pnpm + Pagefind).

## Build locally

Prerequisites (one-time):

```bash
brew install hugo go node pnpm
```

Then, from the repo root:

```bash
pnpm install
hugo mod get -u   # refresh HugoBlox/kit modules to latest tagged versions
hugo server       # http://localhost:1313/
```

Production build (matches what Netlify runs):

```bash
hugo --gc --minify
pnpm run pagefind   # builds the search index from public/
```

## Repo layout (HugoBlox conventions)

| Path | What lives there |
|------|------------------|
| `config/_default/hugo.yaml` | Site title, baseURL, permalinks (`/talk/:slug/`, `/publication/:slug/`), taxonomies. |
| `config/_default/params.yaml` | HugoBlox v2 schema — identity, theme palette (`#e76f51`), Google Analytics measurement ID, repository link, copyright. |
| `config/_default/menus.yaml` | Top nav (with nested Publications / Presentations / Notes submenus). |
| `config/_default/module.yaml` | Hugo module imports (`HugoBlox/kit/modules/{blox,slides,integrations/netlify}`). |
| `data/authors/admin.yaml` | The author profile that drives the home bio block, the awards list, the experience timeline, and `authors: [admin]` references in publications/talks. |
| `content/_index.md` | Home page (bio block + News markdown block). |
| `content/{publications,events,projects}/<slug>/index.md` | One folder per item, plus `featured.{jpg,png}` and `cite.bib`. |
| `content/{publications,talks,projects,select-pubs,select-talks,awards,experience,contact,notes}.md` | Top-level landing pages, each composed of HugoBlox blocks (`portfolio`, `collection`, `resume-awards`, `resume-experience`, `contact-info`). |
| `layouts/_shortcodes/related_items.html` | The one local override — appended to project bodies via `{{< related_items >}}` to list publications + talks that reference the project in their `projects:` front-matter array. |
| `static/uploads/CV.pdf` | Linked from the menu and the home bio block. |

## Adding content

A new publication, talk, or project is a single folder under
`content/{publications,events,projects}/<slug>/` with an `index.md` and
optional `featured.{jpg,png}` / `cite.bib`. See the existing entries for the
front-matter shape (`links: [{type: pdf, url: ...}]` etc.).
