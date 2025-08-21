# MDI Webfont (`mdi`)

[![npm version](https://img.shields.io/npm/v/@pteamx/mdi.svg?color=blue)](https://www.npmjs.com/package/@pteamx/mdi)
[![npm downloads](https://img.shields.io/npm/dm/@pteamx/mdi.svg?color=green)](https://www.npmjs.com/package/@pteamx/mdi)
[![license](https://img.shields.io/npm/l/@pteamx/mdi.svg?color=yellow)](https://github.com/pteamx/material-design-icons/blob/main/LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/pteamx/material-design-icons?style=social)](https://github.com/pteamx/material-design-icons/stargazers)


Webfont package based on **Google Material Symbols (v4.0.0, official)**.  
This package provides ready-to-use **CSS + webfonts** for baseline, rounded and sharp variants.  
All classes are prefixed with `mdi`.

---

## Variants

- **baseline** → `mdi`  
- **rounded** → `mdi-rounded`  
- **sharp** → `mdi-sharp`

Example:

```html
<i class="mdi mdi-home"></i>
<i class="mdi-rounded mdi-favorite"></i>
<i class="mdi-sharp mdi-settings"></i>
```

---

## Installation

```bash
npm i @pteamx/mdi
# or
yarn add @pteamx/mdi
# or
pnpm add @pteamx/mdi
```

---

## Usage

### Option A — HTML (`<link>` tags)

Connect the styles you need:

```html
<!-- Baseline -->
<link rel="stylesheet" href="/node_modules/@pteamx/mdi/css/mdi.css">

<!-- Rounded (optional) -->
<link rel="stylesheet" href="/node_modules/@pteamx/mdi/css/mdi-rounded.css">

<!-- Sharp (optional) -->
<link rel="stylesheet" href="/node_modules/@pteamx/mdi/css/mdi-sharp.css">
```

Use icons:

```html
<i class="mdi mdi-home"></i>             <!-- baseline -->
<i class="mdi-rounded mdi-favorite"></i> <!-- rounded -->
<i class="mdi-sharp mdi-settings"></i>   <!-- sharp -->
```

### Option B — SCSS

```scss
@use "@pteamx/mdi/css/mdi.css";          // baseline
@use "@pteamx/mdi/css/mdi-rounded.css";  // rounded (optional)
@use "@pteamx/mdi/css/mdi-sharp.css";    // sharp (optional)
```

---

## Class naming

```html
<i class="mdi mdi-<icon-name>"></i>
<i class="mdi-rounded mdi-<icon-name>"></i>
<i class="mdi-sharp mdi-<icon-name>"></i>
```

The `<icon-name>` matches the **Material Symbols** icon name (e.g. `home`, `favorite`, `settings`, …).

---

## Files

```
mdi/
 └─ css/
    ├─ mdi.css
    ├─ mdi-rounded.css
    └─ mdi-sharp.css
 └─ fonts/
    ├─ mdi.woff2 / .woff / .ttf / .eot / .svg
    ├─ mdi-rounded.*   (rounded variant)
    └─ mdi-sharp.*     (sharp variant)
```

👉 Use `.woff2` when possible — it’s the most compact modern format.  
Other formats are provided for compatibility.

---

## Tips

- You can include one variant (baseline/rounded/sharp) or several at once.  
- If you bundle assets, copy `mdi/fonts/*` to your public assets directory and adjust the `url()` paths in CSS if needed.  
- Tree-shaking doesn’t apply to webfonts — include only the variants you actually use.

---

## License

- **Icons:** [Google Material Symbols](https://fonts.google.com/icons), licensed under the [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0).  
- **This package:** redistributes the compiled webfonts/CSS for easier consumption.

---

## Repository & Issues

- Source & build scripts: <https://github.com/pteamx/material-design-icons>  
- Issues: <https://github.com/pteamx/material-design-icons/issues>

---

## Acknowledgements

Crafted by **pteamx**.  
Based on **Google Material Symbols (official)**.