# Clover CSS

A complete visual foundation for ambitious websites. Clover combines a design-token system, responsive layout primitives, reusable interface components and expressive visual effects in a framework that stays close to native CSS.

## Install

~~~bash
npm install @spideythedev/clover-css
~~~

~~~html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/spideythedev/clover-css@main/clover.css">
~~~

The core stylesheet is **clover.css**. The original expressive effects library is preserved separately as **clover-effects.css**.

## Quick start

~~~html
<div class="clover-container clover-stack">
  <section class="clover-card" data-variant="raised">
    <span class="clover-badge" data-variant="success">Ready</span>
    <h1>Make the web feel considered.</h1>
    <p>Build interfaces with a coherent visual foundation.</p>
    <div class="clover-cluster">
      <button class="clover-button">Get started</button>
      <button class="clover-button" data-variant="outline">Explore</button>
    </div>
  </section>
</div>
~~~

## Design system

Override a few tokens to reshape the entire interface.

~~~css
:root {
  --clover-primary: #3159c9;
  --clover-primary-hover: #2447aa;
  --clover-radius-md: 1rem;
  --clover-radius-lg: 1.5rem;
  --clover-font-sans: "Manrope", system-ui, sans-serif;
  --clover-content-width: 82rem;
}
~~~

## Themes

Automatic mode follows the operating system. Set an explicit theme on any ancestor to override it.

~~~html
<html data-clover-theme="dark">
~~~

Supported values are **light** and **dark**. Remove the attribute to use automatic mode.

## Global shape and density

~~~html
<div data-clover-radius="soft" data-clover-density="comfortable">
  ...
</div>
~~~

Radius options: **sharp**, default, **soft**. Density options: **compact**, default, **comfortable**.

## Components

| Component | Class |
| --- | --- |
| Card | clover-card |
| Button | clover-button |
| Badge | clover-badge |
| Input | clover-input |
| Select | clover-select |
| Textarea | clover-textarea |
| Field | clover-field |
| Label | clover-label |
| Alert | clover-alert |
| Avatar | clover-avatar |
| Progress | clover-progress |
| Skeleton | clover-skeleton |
| Table | clover-table |
| Navigation | clover-nav |
| Panel | clover-panel |
| Divider | clover-divider |

Variants use data attributes instead of a growing collection of class names.

~~~html
<button class="clover-button" data-variant="secondary" data-size="sm">Cancel</button>
<div class="clover-card" data-variant="soft">...</div>
<span class="clover-badge" data-variant="warning">Pending</span>
~~~

## Layout

~~~html
<div class="clover-container">
  <div class="clover-grid-auto" style="--clover-grid-min: 18rem">
    <article class="clover-card">One</article>
    <article class="clover-card">Two</article>
    <article class="clover-card">Three</article>
  </div>
</div>
~~~

Available primitives: **clover-container**, **clover-stack**, **clover-cluster**, **clover-grid**, **clover-grid-auto**, **clover-split**, **clover-center** and **clover-flow**.

## Original effects

The original Clover visual experiments remain available in **clover-effects.css**. Load it after the core stylesheet when you want the original glass, clay, cyber, magnetic, liquid, typewriter, kaleidoscope and motion effects.

~~~html
<link rel="stylesheet" href="clover.css">
<link rel="stylesheet" href="clover-effects.css">
~~~

## Accessibility

Clover includes visible keyboard focus, native control semantics, reduced-motion handling, responsive layouts and system-aware color schemes. Components provide styling only; interactive behavior, labels, validation and ARIA semantics remain the responsibility of the application.

## Browser support

The core uses modern CSS features including custom properties, cascade layers, color-mix and grid. Use current versions of Chromium, Firefox and Safari.

## License

MIT. See [LICENSE](LICENSE).
