# sensible.css

Set of sensible CSS defaults for any website. Use along with the [normalize.css](https://necolas.github.io/normalize.css/).

Based on modern ([unit value](http://caniuse.com/#feat=calc) and [custom properties](http://caniuse.com/#feat=css-variables)) APIs. Works on Chrome, Firefox, Safari and Opera without additional libraries. For IE and Edge support you can use [postcss-cssnext](http://cssnext.io).

## Installation

**npm**

`$ npm install --save sensible.css`

**Yarn**

`$ yarn add sensible.css`

**CDN**

`<link rel="stylesheet" href="//cdn.rawgit.com/bkzl/sensible.css/v1.0.2/sensible.css">`


## What does it do?

- Changes global (excluding images) box sizing to `border-box`
- Shows vertical scrollbar
- Removes top and/or bottom margin from text, table and form elements
- Removes bottom margin from nested ordered and unordered lists
- Sets font smoothing
- Sets basic font size of headings, body and small text using [modular scale](http://www.modularscale.com/); you can control the values by setting: `--font-base` (1em), `--font-ratio` (1.3333) and `--font-leading` (1.45)
- Defines `--spacing-unit` (1.3rem)
- Changes images vertical align to middle
- Sets tables border collapse and width (100%)
- Aligns `thead` cells text to left
- Sets `code` and `pre code` white space
- Positions `sup` and `sub`

## Custom properties

Override custom properties by setting new values in the `:root` element:

```css
:root {
  --font-base: 1em;
  --font-ratio: 1.333;
  --font-leading: 1.45;
  --heading-ascent: 1.414em;
  --heading-descent: 0.5em;
  --heading-leading: 1.2;
  --spacing-unit: 1.3rem;
}
```
