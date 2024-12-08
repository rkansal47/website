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

Follow [this](https://bootstrap.hugoblox.com/getting-started/install-hugo-extended/) for building locally. The command is

```bash
hugo server
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