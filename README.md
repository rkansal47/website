# Source Code for https://raghavkansal.com

- [Source Code for https://raghavkansal.com](#source-code-for-httpsraghavkansalcom)
  - [Customizations for future reference](#customizations-for-future-reference)
    - [SafeHTML for author block](#safehtml-for-author-block)


## Customizations for future reference

### SafeHTML for author block

To render page breaks and italics, had to:

1. Copy the source [about.biography.html](https://github.com/wowchemy/wowchemy-hugo-themes/blob/98c928a7671543a44cc86dcdc5308ea3f23dd79a/modules/wowchemy/layouts/partials/blocks/about.biography.html#L124) file to [layouts/partials/blocks/about.biography.html](layouts/partials/blocks/about.biography.html)
2. Modify this [line](https://github.com/wowchemy/wowchemy-hugo-themes/blob/98c928a7671543a44cc86dcdc5308ea3f23dd79a/modules/wowchemy/layouts/partials/blocks/about.biography.html#L124), changing `{{ .institution }}` --> `{{ .institution | SafeHTML }}`

Downloading the source file locally overwrites the source. Changing the line allows it to use HTML commands (by default, it escapes them.)