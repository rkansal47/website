# Website

Source Code for https://raghavkansal.com.

- [Website](#website)
  - [Building](#building)
  - [Customizations for future reference](#customizations-for-future-reference)
    - [SafeHTML for author block](#safehtml-for-author-block)
    - [SCSS](#scss)
    - [Layouts](#layouts)
      - [Event / Talk Page](#event--talk-page)
      - [Project Page](#project-page)
      - [Page Links (buttons)](#page-links-buttons)
      - [Views](#views)


## Building

Install the toolchain (Hugo Extended is required for SCSS; Go is required because the theme is loaded as a Hugo Module):

```bash
brew install hugo go
```

Fetch theme modules and run the dev server:

```bash
hugo mod get -u
hugo mod tidy
hugo server
```

The site is then served at <http://localhost:1313>.

To reproduce the production build that Netlify generates into `public/`:

```bash
hugo --gc --minify
```

### Modern Hugo compatibility shims

The wowchemy theme (now defunct, succeeded by HugoBlox) was last released against Hugo ~0.111. Several local overrides keep it building on current Hugo (≥ 0.123 removed `getCSV`, ≥ 0.145 removed `_build`, etc.):

- [`layouts/shortcodes/table.html`](layouts/shortcodes/table.html) — replaces removed `getCSV` with `os.ReadFile` + `transform.Unmarshal`.
- [`layouts/partials/analytics/google_analytics.html`](layouts/partials/analytics/google_analytics.html) and [`layouts/partials/components/feedback.html`](layouts/partials/components/feedback.html) — replace removed `site.GoogleAnalytics` with `site.Config.Services.GoogleAnalytics.ID`.
- [`layouts/_default/baseof.html`](layouts/_default/baseof.html) — fixes a bug in the theme's `{{with .File}}` block (it dereferenced `.File.UniqueID` instead of `.UniqueID`, which the new `*source.File` type rejects).
- [`layouts/partials/functions/get_featured_image.html`](layouts/partials/functions/get_featured_image.html) — shim that forwards to the new namespaced `wowchemy-core/functions/get_featured_image.html` (a few v5.9.0 call sites still use the old un-namespaced path).
- [`layouts/landing/list.html`](layouts/landing/list.html) — wowchemy ships `landing/single.html` but no `landing/list.html`, so a section's `_index.md` with `type: landing` falls back to `_default/list.html` and ignores the `sections:` block builder. This shim mirrors the single template so landing pages also work as section indexes (e.g. `content/publications/_index.md` → `/publications/`).
- `content/{event,publications}/_index.md` use string view names (`card`, `citation`) instead of numeric ones (`3`, `4`); modern Hugo decodes integers as `uint64` which the theme's view dispatcher doesn't handle.
- `config/_default/languages.yaml` uses `locale:` instead of the deprecated `languageCode:`.
- `config/_default/config.yaml` uses `pagination.pagerSize` instead of the deprecated top-level `paginate:`.

### Publications URL

The publications section lives under `content/publications/` (plural) so individual papers render at `/publications/<slug>/` and the section landing at `/publications/`. The older `/publication/*` URLs (used through May 2026) are 301-redirected via [`static/_redirects`](static/_redirects) on Netlify.

To configure Google Analytics, set the GA tag in `config/_default/config.yaml`:

```yaml
services:
  googleAnalytics:
    ID: G-XXXXXXXXXX
```


## Customizations for future reference

### SafeHTML for author block

To render page breaks and italics, had to:

1. Copy the source [about.biography.html](https://github.com/wowchemy/wowchemy-hugo-themes/blob/98c928a7671543a44cc86dcdc5308ea3f23dd79a/modules/wowchemy/layouts/partials/blocks/about.biography.html#L124) file to [layouts/partials/blocks/about.biography.html](layouts/partials/blocks/about.biography.html)
2. Modify this [line](https://github.com/wowchemy/wowchemy-hugo-themes/blob/98c928a7671543a44cc86dcdc5308ea3f23dd79a/modules/wowchemy/layouts/partials/blocks/about.biography.html#L124), changing `{{ .institution }}` --> `{{ .institution | SafeHTML }}`

Downloading the source file locally overwrites the source. Changing the line allows it to use HTML commands (by default, it escapes them.)


### SCSS

See changes in [assets/scss/custom.scss](assets/scss/custom.scss)


### Layouts

#### Event / Talk Page

Added location link [here](https://github.com/rkansal47/website/blob/b91fb48fbbfb65b73894ab4e392bf00ed3c352f3/layouts/event/single.html#L54).

#### Project Page

 - Removed footer
 - Added functionality to show only featured papers or talks [here](https://github.com/rkansal47/website/blob/b91fb48fbbfb65b73894ab4e392bf00ed3c352f3/layouts/project/single.html#L29-L31) but didn't end up using it

#### Page Links (buttons)

Added arXiv button [here](https://github.com/rkansal47/website/blob/b91fb48fbbfb65b73894ab4e392bf00ed3c352f3/layouts/partials/page_links.html#L32-L36).

#### Views

Bunch of custom views, including:

 - "Card" backgrounds with different opacities e.g. [here](https://github.com/rkansal47/website/blob/b91fb48fbbfb65b73894ab4e392bf00ed3c352f3/layouts/partials/views/community/event_card.html#L33)
 - Adding URLs for locations and events
 - Modifying metadata format e.g. [here](https://github.com/rkansal47/website/blob/b91fb48fbbfb65b73894ab4e392bf00ed3c352f3/layouts/partials/views/community/event_card.html#L62-L73)
 - Remove time from dates e.g. [here](https://github.com/rkansal47/website/blob/b91fb48fbbfb65b73894ab4e392bf00ed3c352f3/layouts/partials/views/community/event_card.html#L60)
