# Veld-UI

**A quiet design system for thoughtful interfaces.**

Veld-UI is a framework-free CSS design system inspired by editorial layouts, cartographic details, warm paper, forest ink, and terracotta accents. It is built with CSS custom properties, responsive layouts, system fonts, and no runtime dependencies.

## Features

- CSS only — no JavaScript or build step required
- Responsive editorial layout primitives
- Ivory, forest green, terracotta, and mineral color palette
- Serif display typography paired with monospace labels
- Topographic contour-inspired visual details
- CSS custom properties for colors, type scales, spacing, and layout
- Visible keyboard focus styles
- `prefers-reduced-motion` support
- No third-party fonts, trackers, or external assets

## Preview

Open [`preview/index.html`](preview/index.html) locally, or enable GitHub Pages for the repository and publish from the root folder.

## Quick start

Copy `veld.css` into your project and include it in your HTML:

```html
<link rel="stylesheet" href="./veld.css">
```

Use Veld-UI's layout and type classes:

```html
<div class="veld-shell">
  <p class="veld-label">Field note · 01</p>
  <h1 class="veld-display">A quieter web.</h1>
  <p class="veld-lede">
    A considered visual language for thoughtful interfaces.
  </p>
  <a class="veld-link-arrow" href="#work">Explore work</a>
</div>
```

## Core tokens

| Token | Default |
| --- | --- |
| `--veld-paper` | `#F1EBDF` |
| `--veld-paper-raised` | `#E6DECE` |
| `--veld-ink` | `#17251F` |
| `--veld-ink-soft` | `#3A4A42` |
| `--veld-sage` | `#5C6E62` |
| `--veld-terracotta` | `#A8442A` |
| `--veld-mineral` | `#C09A2E` |

Override the custom properties in your own stylesheet to create a variation:

```css
:root {
  --veld-paper: #f5f1e8;
  --veld-ink: #202820;
  --veld-terracotta: #9d4932;
}
```

## Class naming

Veld-UI classes use the `veld-` prefix to reduce collisions with existing styles. The stylesheet provides the editorial layout and component classes used by the preview, including:

- `.veld-shell`
- `.veld-label`
- `.veld-header` and `.veld-nav`
- `.veld-hero` and `.veld-hero-grid`
- `.veld-display` and `.veld-lede`
- `.veld-plate` and `.veld-plate-data`
- `.veld-section` and `.veld-intro-grid`
- `.veld-list` and `.veld-work`
- `.veld-quote`
- `.veld-footer`
- `.veld-button`

These classes are design primitives rather than a complete component framework. Compose them with semantic HTML to suit your project.

## CDN

After you publish this repository under your GitHub account, you can load the stylesheet through jsDelivr:

```html
<link
  rel="stylesheet"
  href="https://cdn.jsdelivr.net/gh/USERNAME/veld-ui@main/veld.css"
>
```

Replace `USERNAME` with your GitHub username. The CDN URL will work after the repository and `veld.css` are publicly available.

## GitHub Pages

1. Push this project to a public repository named `veld-ui`.
2. Open **Settings → Pages** in the repository.
3. Under the build and deployment settings, choose **Deploy from a branch**.
4. Select `main` and the `/ (root)` folder, then save.
5. Wait for deployment. The preview can then be opened at `https://USERNAME.github.io/veld-ui/preview/`.

## License

This project is released under [The Unlicense](LICENSE), dedicating it to the public domain to the extent permitted by applicable law. See the license file for the complete text.
