## Theory Snippets

Liquid, CSS, and JS snippets for common patterns and features that are not included in the official extension. These will pull from the filename to generate classes, schema names, etc. DM Josh for requests.

## Table of contents

- [Liquid Workflow Snippets (36)](#liquid-workflow-snippets-36)
- [JavaScript Snippets (1)](#javascript-snippets-1)
- [CSS Snippets (24)](#css-snippets-24)
- [Liquid Language Snippets](#liquid-language-snippets)
  - [Comment Tag](#comment-tag)
  - [Control Flow Tag](#control-flow-tag)
  - [Iteration Tag](#iteration-tag)
  - [Variable Tag](#variable-tag)
  - [Theme Tag](#theme-tag)
  - [Schema Tag](#schema-tag)

## Liquid Workflow Snippets (36)

| Title | Prefixes | Description |
|---|---|---|
| Block Boilerplate | `bbp` | Boilerplate for a block file with example `content_for` and schema/preset. |
| Section Boilerplate | `sbp` | Modern section scaffold with attribute-based styles, color/padding settings, and schema. |
| Project Section Boilerplate | `psbp` | Project section scaffold with color scheme, width, desktop/mobile padding controls, and presets. |
| Legacy Section Boilerplate Baseline | `lsbpb` | Minimal Shopify section with schema and stylesheet link. |
| Legacy Section Boilerplate | `lsbp` | Full Shopify section scaffold with color and padding settings and schema. |
| Legacy Swiper Boilerplate | `lswp`, `lswiper` | Liquid markup to render a Swiper slider with captured options and slides. |
| Javascript asset | `js`, `jsa` | Add a deferred `<script>` tag referencing the section JS asset. |
| Javascript module | `jm`, `jsm` | Add a `<script type="module">` tag referencing the component JS asset. |
| CSS asset | `css` | Add a `stylesheet_tag` linking the section CSS asset. |
| Style tag | `style` | Insert a Shopify `{% style %}` block. |
| Stylesheet tag | `ts`, `st`, `stylesheet tag` | Insert a `{% stylesheet %}` block. |
| Javascript tag | `js`, `jst`, `javascript tag` | Insert a `{% javascript %}` block. |
| Legacy Section style boilerplate | `lsstyle`, `lsecstyle` | Standard section-scoped styles with color variables and responsive padding. |
| Badge | `badge` | Render a metafield-driven badge span with background and text colors. |
| Base Class | `bclass`, `bc` | Insert base BEM class attribute using the current filename. |
| Image Tag | `imgtag` | Render `image_tag` with width, alt, lazy loading, and section-scoped classes. |
| Block Content | `cb`, `contentblock` | Capture and render a `content_for 'block'` placeholder. |
| Blocks Content | `cbs`, `contentblocks` | Output `content_for 'blocks'` placeholder. |
| Product Block Content | `cbp`, `contentblockproduct` | Render a product-specific block via `content_for`. |
| Swiper Block Content | `cbsp, contentblockswiper` | Create `_td-slider` block for Swiper slides or fallback when empty. |
| Render TD Badge | `rbdg`, `rtdbadge`, `rabadge`, `rbdge` | Render `td-badge` snippet for an object with optional class. |
| If Title | `ifti`, `iti`, `iftitle` | Conditional heading if the title setting is present. |
| If Text | `ifte`, `ite`, `iftext` | Conditional text wrapper if the text setting is present. |
| If Image | `ifi`, `iimg`, `ifimage` | Conditional image output with sizing and lazy loading. |
| If Button | `ifb`, `ibtn`, `ifbutton` | Conditional link button combining URL and CTA settings. |
| Attributes attribute | `attrs`, `attributes` | Add inline style attribute via `td-style-attributes` render. |
| Duplicate comment | `dupe` | Add a comment noting a duplicate of the current file. |
| Duplicate text | `dupetext`, `dtext` | Add a comment string noting a duplicate (text variant). |
| Themecheck disable | `disable`, `themecheckdisable` | Disable Theme Check for following lines. |
| Theme check enable | `enable`, `themecheckenable` | Re-enable Theme Check. |
| Metaobject loop | `mloop`, `metaobjectloop` | Iterate over metaobjects of a given type. |
| Richtext metaoject loop | `rml`, `mlr`, `rmetaobjectloop` | Loop metaobjects and output a richtext metafield tag. |
| Link Option | `lopt`, `link option` | Wrap content in `<a>` when URL provided; `<div>` otherwise. |
| If Main Title | `mt`, `ifmt`, `imt`, `ifmain` | Conditional H1 for first section, otherwise H2. |
| Button Schema | `_button` | Schema fragment for URL and CTA fields. |
| Collection List Schema | `_cl`, `_clist` | Schema fragment for a `collection_list` setting. |

## JavaScript Snippets (1)

| Title | Prefixes | Description |
|---|---|---|
| Web Component Boilerplate | `wcb`, `web` | Vanilla custom element class with safe define and error handling. |

## CSS Snippets (24)

| Title | Prefixes | Description |
|---|---|---|
| Base Class | `bc`, `base` | Base selector scaffold using filename-derived block. |
| Card Class | `bcard`, `base card` | Card element selector scaffold. |
| Title Class | `btitle`, `base title` | Title element selector scaffold. |
| Text Class | `btext`, `base text` | Text element descendant reset scaffold. |
| Button Class | `bbtn`, `bbutton`, `base button` | Button element selector scaffold. |
| Grid center | `gce`, `gcenter` | Center content with CSS Grid and `place-items`. |
| Flex gallery | `gallery`, `gf` | Flexible gallery layout with gaps and wrapping. |
| Card width | `Card width`, `cw` | Equal-width cards per column count using `calc`. |
| A11y font size | `afs` | Rem-based font-size relative to a base variable. |
| A11y font size value | `afsv` | Value-only `calc` for font-size expressions. |
| Trim RTE margins | `trim`, `rte` | Remove first/last margins inside the text block. |
| Pause animation | `pause animation` | Set `animation-play-state` to `paused`. |
| Line clamp | `Line clamp`, `lc` | Multi-line truncation using `-webkit-line-clamp`. |
| MQ 375px | `M0`, `M375` | Media query scaffold for max-width 375px. |
| MQ 767px | `M1`, `M767` | Media query scaffold for min-width 767px. |
| MQ 1024px | `M2`, `M1024` | Media query scaffold for min-width 1024px. |
| MQ 1280px | `M3`, `M1280` | Media query scaffold for min-width 1280px. |
| MQ 1440px | `M4`, `M1440` | Media query scaffold for min-width 1440px. |
| MQ 1920px | `M5`, `M1920` | Media query scaffold for min-width 1920px. |
| MXQ 767px | `MXQ1`, `MXQ767` | Media query scaffold for max-width 767px. |
| MXQ 1024px | `MXQ2`, `MXQ1024` | Media query scaffold for max-width 1024px. |
| MXQ 1280px | `MXQ3`, `MXQ1280` | Media query scaffold for max-width 1280px. |
| MXQ 1440px | `MXQ4`, `MXQ1440` | Media query scaffold for max-width 1440px. |
| MXQ 1920px | `MXQ5`, `MXQ1920` | Media query scaffold for max-width 1920px. |

---

## Liquid Language Snippets

Actively maintained fork of the original [Shopify Liquid Template Snippets](https://marketplace.visualstudio.com/items?itemName=killalau.vscode-liquid-snippets)

### Comment Tag

```
comment- // whitespace stripped
doc- // whitespace stripped
```

### Control Flow Tag

```
if
else
elsif
ifelse
unless
case
when
if-     // whitespace stripped
else-   // whitespace stripped
elsif-  // whitespace stripped
ifelse- // whitespace stripped
unless- // whitespace stripped
case-   // whitespace stripped
when-   // whitespace stripped
```

### Iteration Tag

```
cycle
cyclegroup
for
limit       // For loops option
offset      // For loops option
reversed    // For loops option
break
continue
tablerow
cycle-      // whitespace stripped
cyclegroup- // whitespace stripped
for-        // whitespace stripped
continue-   // whitespace stripped
tablerow-   // whitespace stripped
```

### Variable Tag

```
assign
increment
decrement
capture
assign-  // whitespace stripped
capture- // whitespace stripped
```

### Theme Tag

```
content_for
render
renderwith // Theme tag {% render %} with parameters
section
raw
layout
layoutnone
liquid
liquid-   // whitespace stripped
paginate
schema
stylesheet

```

### Schema Tag

```
_schema
_text
_textarea
_image_picker
_radio
_select
_checkbox
_range
_color
_font
_collection
_product
_blog
_page
_link_list
_url
_video
_richtext
_html
_article
_header
_paragraph
_blocks
_number
_collection_list
_product_list
_color_background
_color_scheme
_color_scheme_group
_inline_richtext
_liquid
_metaobject
_metaobject_list
_text_alignment
_video_file
```
