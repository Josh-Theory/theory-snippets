## Theory Snippets

Liquid, CSS, and JS snippets for common patterns and features that are not included in the official extension. These will pull from the filename to generate classes, schema names, etc. DM me for requests.

## Liquid Snippets (37)

| Title | Prefixes | Description |
|---|---|---|
| Section Boilerplate Baseline | `sbpb` | Minimal Shopify section with schema and stylesheet link. |
| Section Boilerplate | `sbp` | Full Shopify section scaffold with color and padding settings and schema. |
| Swiper Boilerplate | `swp`, `swiper` | Liquid markup to render a Swiper slider with captured options and slides. |
| Javascript asset | `js`, `jsa` | Add a deferred `<script>` tag referencing the section JS asset. |
| Javascript module | `jm`, `jsm` | Add a `<script type="module">` tag referencing the component JS asset. |
| CSS asset | `css` | Add a `stylesheet_tag` linking the section CSS asset. |
| Style tag | `style` | Insert a Shopify `{% style %}` block. |
| Stylesheet tag | `ts`, `st`, `stylesheet tag` | Insert a `{% stylesheet %}` block. |
| Javascript tag | `js`, `jst`, `javascript tag` | Insert a `{% javascript %}` block. |
| Section style boilerplate | `sstyle`, `secstyle` | Standard section-scoped styles with color variables and responsive padding. |
| Badge | `badge` | Render a metafield-driven badge span with background and text colors. |
| Base Class | `bclass, bc` | Insert base BEM class attribute using the current filename. |
| Image Tag | `imgtag` | Render `image_tag` with width, alt, lazy loading, and section-scoped classes. |
| Block Content | `cb, contentblock` | Capture and render a `content_for 'block'` placeholder. |
| Blocks Content | `cbs`, `contentblocks` | Output `content_for 'blocks'` placeholder. |
| Product Block Content | `cbp, contentblockproduct` | Render a product-specific block via `content_for`. |
| Swiper Block Content | `cbsp, contentblockswiper` | Create `_td-slider` block for Swiper slides or fallback when empty. |
| Render TD Badge | `rbdg, rtdbadge, rabadge, rbdge` | Render `td-badge` snippet for an object with optional class. |
| If Title | `ifti, iti, iftitle` | Conditional heading if the title setting is present. |
| If Text | `ifte, ite, iftext` | Conditional text wrapper if the text setting is present. |
| If Image | `ifi, iimg, ifimage` | Conditional image output with sizing and lazy loading. |
| If Button | `ifb, ibtn, ifbutton` | Conditional link button combining URL and CTA settings. |
| Liquid tag | `liq` | Insert a `{% liquid %}` tag wrapper. |
| Attributes attribute | `attrs, attributes` | Add inline style attribute via `td-style-attributes` render. |
| Doc tag | `doctag` | Insert a `{% doc %}` block. |
| Duplicate comment | `dupe` | Add a comment noting a duplicate of the current file. |
| Duplicate text | `dupetext, dtext` | Add a comment string noting a duplicate (text variant). |
| Themecheck disable | `disable`, `themecheckdisable` | Disable Theme Check for following lines. |
| Theme check enable | `enable`, `themecheckenable` | Re-enable Theme Check. |
| Metaobject loop | `mloop, metaobjectloop` | Iterate over metaobjects of a given type. |
| Richtext metaoject loop | `rml, mlr, rmetaobjectloop` | Loop metaobjects and output a richtext metafield tag. |
| Link Option | `lopt, link option` | Wrap content in `<a>` when URL provided; `<div>` otherwise. |
| If Main Title | `mt, ifmt, imt, ifmain` | Conditional H1 for first section, otherwise H2. |
| Color Scheme Schema | `_scheme` | Schema fragment for a color scheme setting. |
| Color Background Schema | `_bgc` | Schema fragment for a color background setting. |
| Button Schema | `_button` | Schema fragment for URL and CTA fields. |
| Collection List Schema | `_cl`, `_clist` | Schema fragment for a `collection_list` setting. |

## JavaScript Snippets (1)

| Title | Prefixes | Description |
|---|---|---|
| Web Component Boilerplate | `wcb`, `web` | Vanilla custom element class with safe define and error handling. |

## CSS Snippets (18)

| Title | Prefixes | Description |
|---|---|---|
| Base Class | `bc`, `base` | Base selector scaffold using filename-derived block. |
| Card Class | `bcard`, `base card` | Card element selector scaffold. |
| Title Class | `btitle`, `base title` | Title element selector scaffold. |
| Text Class | `btext`, `base text` | Text element descendant reset scaffold. |
| Button Class | `bbtn`, `bbutton`, `base button` | Button element selector scaffold. |
| Grid center | `gce`, `gcenter` | Center content with CSS Grid and `place-items`. |
| Flex gallery | `gallery, gf` | Flexible gallery layout with gaps and wrapping. |
| Card width | `Card width`, `cw` | Equal-width cards per column count using `calc`. |
| A11y font size | `afs` | Rem-based font-size relative to a base variable. |
| A11y font size value | `afsv` | Value-only `calc` for font-size expressions. |
| Trim RTE margins | `trim`, `rte` | Remove first/last margins inside the text block. |
| Line clamp | `Line clamp`, `lc` | Multi-line truncation using `-webkit-line-clamp`. |
| MQ 375px | `M0`, `M375` | Media query scaffold for max-width 375px. |
| MQ 767px | `M1`, `M767` | Media query scaffold for min-width 767px. |
| MQ 1024px | `M2`, `M1024` | Media query scaffold for min-width 1024px. |
| MQ 1280px | `M3`, `M1280` | Media query scaffold for min-width 1280px. |
| MQ 1440px | `M4`, `M1440` | Media query scaffold for min-width 1440px. |
| MQ 1920px | `M5`, `M1920` | Media query scaffold for min-width 1920px. |

---

