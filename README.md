# Clover CSS

**ChloroPhilix · Version 3.0**

A single visual language for the whole interface. ChloroPhilix brings a violet-led color family, consistent geometry, responsive layout primitives and customizable components into a CSS-native design system.

## Install

~~~bash
npm install @spideythedev/clover-css
~~~

~~~html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/spideythedev/clover-css@v3.0.0/clover.css">
~~~

The core framework is **clover.css**. The original expressive experiments remain available in **clover-effects.css** as an optional companion.

## Quick start

~~~html
<main class="clover-container clover-stack">
  <section class="clover-card" data-variant="raised">
    <span class="clover-badge" data-variant="primary">ChloroPhilix</span>
    <h1>One visual language. Every detail in sync.</h1>
    <p>Compose interfaces with a considered system of color, shape and rhythm.</p>
    <div class="clover-cluster">
      <button class="clover-button">Get started</button>
      <button class="clover-button" data-variant="outline">Explore</button>
    </div>
  </section>
</main>
~~~

## The ChloroPhilix system

ChloroPhilix is built around one violet-indigo family. Surfaces, borders, accents, focus states, badges and controls share the same tonal language. Neutral ink and porcelain surfaces provide contrast without introducing competing accent families.

The default theme is light. Dark mode uses the same color family with deeper surfaces and brighter violet tones.

## Customize the system

Override tokens at the root or on a component scope.

~~~css
:root {
  --clover-primary: #6252dc;
  --clover-primary-hover: #5142bd;
  --clover-accent: #ebe8ff;
  --clover-radius-md: 1rem;
  --clover-radius-lg: 1.4rem;
  --clover-font-sans: "Manrope", system-ui, sans-serif;
  --clover-content-width: 84rem;
}
~~~

The full violet scale is available as **--clover-violet-50** through **--clover-violet-950**.

## Themes

~~~html
<html data-clover-theme="dark">
~~~

Use **light** or **dark**. Remove the attribute to follow the operating system preference.

## Shape and density

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
| Field and label | clover-field, clover-label |
| Alert | clover-alert |
| Avatar | clover-avatar |
| Progress | clover-progress |
| Skeleton | clover-skeleton |
| Table | clover-table |
| Navigation | clover-nav |
| Panel | clover-panel |
| Divider | clover-divider |
| Checkbox and radio | clover-checkbox, clover-radio |
| Switch | clover-switch |
| Tabs | clover-tabs, clover-tab |
| Accordion | clover-accordion |
| Breadcrumb | clover-breadcrumb |
| Tooltip | clover-tooltip |
| Stat | clover-stat |
| Pagination | clover-pagination |
| Empty state | clover-empty |

Variants use data attributes.

~~~html
<button class="clover-button" data-variant="outline">Cancel</button>
<div class="clover-card" data-variant="soft">...</div>
<span class="clover-badge" data-variant="primary">Featured</span>
~~~

## Interactive playground

Open [`playground.html`](./playground.html) for live previews of all 50 components. Search by component name, filter the five categories, switch light/dark themes, adjust radius and density, inspect the HTML and copy snippets.

## 50 hyper-classified components

The component library is organized into five groups:

### Navigation & wayfinding

- **Application top bar** — `.clover-topbar`
- **Application sidebar** — `.clover-sidebar`
- **Menu bar** — `.clover-menubar`
- **Command bar** — `.clover-commandbar`
- **Step indicator** — `.clover-stepper`
- **Segmented control** — `.clover-segmented`
- **Navigation rail** — `.clover-rail`
- **Navigation card** — `.clover-linkcard`
- **Tree navigation** — `.clover-tree`
- **Timeline** — `.clover-timeline`

### Data & visualization

- **Metric tile** — `.clover-metric`
- **Sparkline** — `.clover-sparkline`
- **Chart frame** — `.clover-chartframe`
- **Data grid** — `.clover-datagrid`
- **Data row** — `.clover-listrow`
- **Kanban board** — `.clover-kanban`
- **Activity feed** — `.clover-activity`
- **Rating display** — `.clover-rating`
- **Meter** — `.clover-meter`
- **Comparison panel** — `.clover-comparison`

### Inputs & form controls

- **Search field** — `.clover-search`
- **Combobox** — `.clover-combobox`
- **Date field** — `.clover-datefield`
- **Range control** — `.clover-range`
- **Number field** — `.clover-number`
- **PIN input** — `.clover-pin`
- **File drop zone** — `.clover-filedrop`
- **Upload item** — `.clover-upload`
- **Toggle group** — `.clover-togglegroup`
- **Form step** — `.clover-formstep`

### Feedback & states

- **Toast message** — `.clover-toast`
- **Announcement banner** — `.clover-banner`
- **Callout** — `.clover-callout`
- **Status indicator** — `.clover-status`
- **Notification item** — `.clover-notification`
- **Progress ring** — `.clover-progressring`
- **Skeleton block** — `.clover-skeletonblock`
- **Empty panel** — `.clover-emptypanel`
- **Error panel** — `.clover-errorpanel`
- **Success panel** — `.clover-successpanel`

### Overlays, actions & media

- **Modal surface** — `.clover-modal`
- **Side drawer** — `.clover-drawer`
- **Popover surface** — `.clover-popover`
- **Dropdown menu** — `.clover-dropdown`
- **Context menu** — `.clover-contextmenu`
- **Command palette** — `.clover-commandpalette`
- **Media card** — `.clover-media`
- **Image frame** — `.clover-image`
- **Video frame** — `.clover-video`
- **Code block** — `.clover-codeblock`

These classes provide visual structure only. Use semantic HTML and add the required JavaScript, ARIA state, focus management and keyboard behavior in your application.

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

The original visual experiments remain in **clover-effects.css**. Load it after the core stylesheet when you want the legacy glass, clay, cyber, magnetic, liquid, typewriter, kaleidoscope and motion effects.

~~~html
<link rel="stylesheet" href="clover.css">
<link rel="stylesheet" href="clover-effects.css">
~~~

## Accessibility

Clover includes visible keyboard focus, native control semantics, reduced-motion handling, responsive layouts and system-aware color schemes. Components provide styling only; application behavior, labels, validation and ARIA semantics remain the responsibility of the consuming application.

## Browser support

The core uses custom properties, cascade layers, grid, color-mix and modern selectors. Target current versions of Chromium, Firefox and Safari.

## License

MIT. See [LICENSE](LICENSE).
