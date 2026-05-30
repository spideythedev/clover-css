# 🍀 Clover CSS

> *"If a dev can easily recreate it, it's too simple for Clover."*

**Clover CSS** is an intentionally overcomplicated CSS component library. **20 components.** One class each. 7,000+ lines of CSS. Zero JavaScript required. Beautiful, absurd results.

Every component takes 150-400 lines of meticulously engineered CSS — layered shadows, nested pseudo-elements, SVG filters, math-driven animations, blend modes, transform chains, and custom property cascades that would make any sane developer weep.

---

[![NPM Version](https://img.shields.io/npm/v/clover-css-lib)](https://www.npmjs.com/package/clover-css-lib)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Lines of CSS](https://img.shields.io/badge/Lines-7000%2B-6c5ce7)](clover.css)
[![Components](https://img.shields.io/badge/Components-20-00c853)](https://github.com/spideythedev/clover-css)
[![Zero JS](https://img.shields.io/badge/JavaScript-0%25-ff6b6b)](https://github.com/spideythedev/clover-css)

---

## 📑 Table of Contents

- [Philosophy](#-philosophy)
- [Installation](#-installation)
- [Quick Start](#-quick-start)
- [Components Overview](#-components-overview)
- [Component Details](#-component-details)
  - [1. Glass Card](#1-clover-glass-card)
  - [2. Clay Button](#2-clover-clay-button)
  - [3. Neubrutal Card](#3-clover-neubrutal-card)
  - [4. Cyber Panel](#4-clover-cyber-panel)
  - [5. Magnetic Container](#5-clover-magnetic-container)
  - [6. Liquid Blob](#6-clover-liquid-blob)
  - [7. Typewriter](#7-clover-typewriter)
  - [8. Kaleidoscope](#8-clover-kaleidoscope)
  - [9. Morphing Shape](#9-clover-morphing-shape)
  - [10. Rainbow Spinner](#10-clover-rainbow-spinner)
  - [11. Parallax Section](#11-clover-parallax-section)
  - [12. Flip Card 3D](#12-clover-flip-card-3d)
  - [13. Expand Search](#13-clover-expand-search)
  - [14. Notification Bell](#14-clover-notification-bell)
  - [15. Drag Ghost](#15-clover-drag-ghost)
  - [16. Spotlight Card](#16-clover-spotlight-card)
  - [17. Toggle Realm](#17-clover-toggle-realm)
  - [18. Tooltip Magic](#18-clover-tooltip-magic)
  - [19. Marquee Banner](#19-clover-marquee-banner)
  - [20. Progress Cosmic](#20-clover-progress-cosmic)
- [Theming](#-theming)
- [Dark Mode](#-dark-mode)
- [Accessibility](#-accessibility)
- [Browser Support](#-browser-support)
- [Performance](#-performance)
- [File Structure](#-file-structure)
- [Contributing](#-contributing)
- [FAQ](#-faq)
- [License](#-license)
- [Links](#-links)

---

## 🧠 Philosophy

Modern CSS is too easy. Utility classes? Sanity? Maintainability? Where's the *art*?

Clover CSS is the antidote. Every component is a masterclass in CSS excess:

- **150-400 lines per component** — Each class hides incredible complexity
- **Nested pseudo-elements** — `::before` and `::after` are always in use
- **Math-driven animations** — `calc()`, `steps()`, `cubic-bezier()` spring physics
- **SVG filters** — `feTurbulence`, `feDisplacementMap` for real-time distortion
- **Blend modes** — `overlay`, `multiply`, `screen`, `soft-light`
- **Transform chains** — `perspective` + `rotateY` + `scale` + `skew` combos
- **Custom properties** — Full theming via CSS variables

### The Clover Promise

> If a developer can easily recreate it, it's too simple for Clover.

---

## 📦 Installation

### NPM

```bash
npm install clover-css-lib
```
## 📦 Installation

### NPM

```bash
npm install clover-css-lib
```

### Import in your CSS:

```css
@import 'clover-css-lib/clover.css';
```

### Or link in HTML:

```html
<link rel="stylesheet" href="node_modules/clover-css-lib/clover.css">
```

### CDN

```html
<!-- UNPKG -->
<link rel="stylesheet" href="https://unpkg.com/clover-css-lib/clover.css">

<!-- jsDelivr (NPM) -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/clover-css-lib/clover.css">

<!-- jsDelivr (GitHub) -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/spideythedev/clover-css/clover.css">
```

---

## 🚀 Quick Start

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Clover CSS Demo</title>
    <link rel="stylesheet" href="https://unpkg.com/clover-css-lib/clover.css">
</head>
<body>

    <!-- Glass Card -->
    <div class="clover-glass-card">
        <h2>Hello Clover 🍀</h2>
        <p>7 layers of glassmorphism in one class.</p>
    </div>

    <!-- Clay Button -->
    <button class="clover-clay-button">Click Me</button>

    <!-- Neubrutal Card -->
    <div class="clover-neubrutal-card">
        <h3>BRUTAL.</h3>
        <p>Hard shadows. Bold colors.</p>
    </div>

    <!-- Cyber Panel -->
    <div class="clover-cyber-panel">
        <p>&gt; ACCESSING MAINFRAME...</p>
        <p>&gt; CONNECTION ESTABLISHED.</p>
    </div>

    <!-- Magnetic Container -->
    <div class="clover-magnetic-container" style="background:linear-gradient(135deg,#667eea,#764ba2);color:white;text-align:center;padding:2rem;">
        <h3>✨ Hover Me ✨</h3>
        <p>I tilt in 3D!</p>
    </div>

    <!-- Liquid Blob (needs SVG filter - see docs) -->
    <div class="clover-liquid-blob" style="--clover-liquid-size:150px;"></div>

    <!-- Typewriter -->
    <div class="clover-typewriter">
        <span data-typewriter-line style="--line-index:0;--line-chars:30;">Hello from Clover CSS CDN! 🍀</span>
        <span data-typewriter-line style="--line-index:1;--line-chars:42;">This is a CSS-only typewriter effect.</span>
        <span data-typewriter-line style="--line-index:2;--line-chars:35;">No JavaScript. Pure CSS magic.</span>
    </div>

    <!-- Kaleidoscope -->
    <div class="clover-kaleidoscope" style="--clover-kaleidoscope-size:150px;"></div>

    <!-- Morphing Shape -->
    <div class="clover-morphing-shape" style="--clover-morph-size:160px;"></div>

    <!-- Rainbow Spinner -->
    <div class="clover-rainbow-spinner" style="--clover-spinner-size:70px;"></div>

    <!-- Flip Card 3D -->
    <div class="clover-flip-card-3d" style="--clover-flip-width:260px;--clover-flip-height:200px;">
        <div class="clover-flip-inner">
            <div class="clover-flip-front"><h3>🎴 Front</h3><p>Hover to flip!</p></div>
            <div class="clover-flip-back"><h3>🔮 Back</h3><p>Surprise!</p></div>
        </div>
    </div>

    <!-- Expand Search -->
    <div class="clover-expand-search">
        <input type="text" placeholder="Search anything...">
    </div>

    <!-- Notification Bell -->
    <button class="clover-notification-bell has-notification">
        <span class="clover-bell-badge">3</span>
    </button>

    <!-- Drag Ghost -->
    <div class="clover-drag-ghost" style="--clover-drag-size:140px;display:flex;align-items:center;justify-content:center;color:white;font-weight:600;">
        Drag Me
    </div>

    <!-- Spotlight Card -->
    <div class="clover-spotlight-card">
        <h3>🔦 Spotlight</h3>
        <p>Move your cursor over me!</p>
    </div>

    <!-- Toggle Realm -->
    <label class="clover-toggle-realm">
        <input type="checkbox">
        <span class="clover-toggle-track"></span>
        <span class="clover-toggle-thumb"></span>
    </label>

    <!-- Tooltip Magic -->
    <span class="clover-tooltip-magic">
        Hover for tip
        <span class="clover-tooltip-body">I'm a magical tooltip! ✨</span>
    </span>

    <!-- Marquee Banner -->
    <div class="clover-marquee-banner">
        <div class="clover-marquee-track">
            <span>🚀 New: Clover CSS v1.0.0 is live!</span>
            <span>🍀 20 components. Zero JS.</span>
            <span>⭐ Star us on GitHub!</span>
            <span>🚀 New: Clover CSS v1.0.0 is live!</span>
            <span>🍀 20 components. Zero JS.</span>
            <span>⭐ Star us on GitHub!</span>
        </div>
    </div>

    <!-- Progress Cosmic -->
    <div class="clover-progress-cosmic" style="--clover-progress:70%;">
        <div class="clover-progress-fill"></div>
        <div class="clover-progress-head"></div>
    </div>

</body>
</html>
```

---

## 🧩 All 20 Components

| # | Component | Type | Lines | Layers |
|---|---|---|---|---|
| 1 | `.clover-glass-card` | Card | ~280 | 7 |
| 2 | `.clover-clay-button` | Button | ~300 | 12 |
| 3 | `.clover-neubrutal-card` | Card | ~250 | 5 |
| 4 | `.clover-cyber-panel` | Panel | ~270 | 5 |
| 5 | `.clover-magnetic-container` | Container | ~240 | 3 |
| 6 | `.clover-liquid-blob` | Decorative | ~180 | 4 |
| 7 | `.clover-typewriter` | Text | ~190 | 5 |
| 8 | `.clover-kaleidoscope` | Decorative | ~170 | 4 |
| 9 | `.clover-morphing-shape` | Decorative | ~200 | 4 |
| 10 | `.clover-rainbow-spinner` | Loader | ~210 | 5 |
| 11 | `.clover-parallax-section` | Section | ~250 | 4 |
| 12 | `.clover-flip-card-3d` | Card | ~240 | 5 |
| 13 | `.clover-expand-search` | Input | ~260 | 5 |
| 14 | `.clover-notification-bell` | Button | ~270 | 6 |
| 15 | `.clover-drag-ghost` | Draggable | ~250 | 4 |
| 16 | `.clover-spotlight-card` | Card | ~380 | 6 |
| 17 | `.clover-toggle-realm` | Toggle | ~390 | 7 |
| 18 | `.clover-tooltip-magic` | Tooltip | ~340 | 5 |
| 19 | `.clover-marquee-banner` | Banner | ~280 | 4 |
| 20 | `.clover-progress-cosmic` | Progress | ~410 | 6 |

---

## 📖 Detailed Usage

### 1. .clover-glass-card

```html
<div class="clover-glass-card">
  <h3>Glass Card</h3>
  <p>Content here...</p>
</div>
```

Property Default Description
--clover-glass-blur 18px Backdrop blur intensity
--clover-glass-saturation 1.8 Color saturation
--clover-glass-opacity 0.35 Base transparency
--clover-glass-pulse-duration 6s Border pulse speed
--clover-glass-noise-opacity 0.04 Texture grain

### 2. .clover-clay-button

```html
<button class="clover-clay-button">Click Me</button>
```

Property Default Description
--clover-clay-bg #f0f0f0 Button background
--clover-clay-text #5a4e4e Text color
--clover-clay-border-radius 22px Corner roundness
--clover-clay-hover-lift -4px Lift on hover
--clover-clay-active-squish 0.92 Press scale

### Variants:

```html
<button class="clover-clay-button" style="padding:1.25rem 3rem;font-size:1.3rem;">Large</button>
<button class="clover-clay-button" style="--clover-clay-bg:#dff9fb;--clover-clay-text:#0a3d62;">Themed</button>
```

### 3. .clover-neubrutal-card

```html
<div class="clover-neubrutal-card">
  <h3>BRUTAL.</h3>
  <p>Content here...</p>
</div>
```

Property Default Description
--clover-neubrutal-bg #ffeb3b Card background
--clover-neubrutal-shadow-offset-x 8px Shadow X offset
--clover-neubrutal-shadow-hover-split 18px Split distance
--clover-neubrutal-slash-color #ff5252 Slash color

### 4. .clover-cyber-panel

```html
<div class="clover-cyber-panel">
  <p>&gt; ACCESSING MAINFRAME...</p>
</div>
```

Property Default Description
--clover-cyber-bg #0a0a0a Terminal background
--clover-cyber-border-color-1 #00ffff Primary neon
--clover-cyber-border-color-2 #ff00ff Secondary neon
--clover-cyber-glitch-shift 4px Glitch displacement

### 5. .clover-magnetic-container

```html
<div class="clover-magnetic-container" style="background:linear-gradient(135deg,#667eea,#764ba2);">
  <h3>✨ Hover Me ✨</h3>
</div>
```

Property Default Description
--clover-magnetic-perspective 800px 3D depth
--clover-magnetic-rotate-factor 0.05 Tilt intensity
--clover-magnetic-scale-hover 1.04 Scale on hover

### Optional JS for cursor tracking:

```javascript
document.querySelectorAll('.clover-magnetic-container').forEach(el => {
  el.addEventListener('mousemove', (e) => {
    const rect = el.getBoundingClientRect();
    el.style.setProperty('--_mouse-x', (e.clientX - rect.left) / rect.width);
    el.style.setProperty('--_mouse-y', (e.clientY - rect.top) / rect.height);
  });
  el.addEventListener('mouseleave', () => {
    el.style.setProperty('--_mouse-x', 0.5);
    el.style.setProperty('--_mouse-y', 0.5);
  });
});
```

### 6. .clover-liquid-blob

Requires SVG filter in HTML:

```html
<svg style="position:absolute;width:0;height:0;">
  <filter id="clover-goo-filter">
    <feTurbulence type="fractalNoise" baseFrequency="0.015" numOctaves="3" seed="2" result="noise">
      <animate attributeName="baseFrequency" values="0.015;0.025;0.015" dur="8s" repeatCount="indefinite"/>
    </feTurbulence>
    <feDisplacementMap in="SourceGraphic" in2="noise" scale="25" xChannelSelector="R" yChannelSelector="G"/>
  </filter>
</svg>

<div class="clover-liquid-blob"></div>
```

Property Default Description
--clover-liquid-bg #6c5ce7 Primary color
--clover-liquid-bg2 #a29bfe Secondary color
--clover-liquid-size 200px Blob size
--clover-liquid-speed 8s Morph speed

### 7. .clover-typewriter

```html
<div class="clover-typewriter">
  <span data-typewriter-line style="--line-index:0;--line-chars:30;">Hello from Clover CSS CDN! 🍀</span>
  <span data-typewriter-line style="--line-index:1;--line-chars:42;">This is a CSS-only typewriter effect.</span>
  <span data-typewriter-line style="--line-index:2;--line-chars:35;">No JavaScript. Pure CSS magic.</span>
</div>
```

Property Default Description
--clover-typewriter-speed 0.07s Per-character speed
--clover-typewriter-line-delay 2s Delay between lines
--line-chars 40 Characters in line (set per line)
--line-index 0 Line number (0, 1, 2...)

### 8. .clover-kaleidoscope

```html
<div class="clover-kaleidoscope"></div>
```

Property Default Description
--clover-kaleidoscope-size 180px Dimensions
--clover-kaleidoscope-speed 12s Rotation speed

### 9. .clover-morphing-shape

```html
<div class="clover-morphing-shape"></div>
```

Property Default Description
--clover-morph-size 200px Dimensions
--clover-morph-speed 10s Morph speed
--clover-morph-bg1 #6c5ce7 Gradient start
--clover-morph-bg2 #fd79a8 Gradient end

### 10. .clover-rainbow-spinner

```html
<div class="clover-rainbow-spinner"></div>
```

Property Default Description
--clover-spinner-size 80px Dimensions
--clover-spinner-speed 1.5s Rotation speed
--clover-spinner-thickness 6px Ring thickness

### 11. .clover-parallax-section

```html
<div class="clover-parallax-section" style="--clover-parallax-height:400px;">
  <div>
    <h2>🚀 Deep Space</h2>
    <p>Scroll to see parallax layers shift.</p>
  </div>
</div>
```

Property Default Description
--clover-parallax-height 100vh Section height
--clover-parallax-bg1 #0a0a2e Deep space color
--clover-parallax-accent #6c5ce7 Accent glow

### 12. .clover-flip-card-3d

```html
<div class="clover-flip-card-3d">
  <div class="clover-flip-inner">
    <div class="clover-flip-front">
      <h3>🎴 Front</h3>
      <p>Hover to flip!</p>
    </div>
    <div class="clover-flip-back">
      <h3>🔮 Back</h3>
      <p>Surprise content!</p>
    </div>
  </div>
</div>
```

Property Default Description
--clover-flip-width 300px Card width
--clover-flip-height 400px Card height
--clover-flip-duration 0.8s Flip speed
--clover-flip-front-bg gradient Front face background
--clover-flip-back-bg gradient Back face background

### 13. .clover-expand-search

```html
<div class="clover-expand-search">
  <input type="text" placeholder="Search anything...">
</div>
```

Property Default Description
--clover-search-size 48px Collapsed size
--clover-search-expand-width 320px Expanded width
--clover-search-glow purple Focus glow color

### 14. .clover-notification-bell

```html
<button class="clover-notification-bell has-notification">
  <span class="clover-bell-badge">3</span>
</button>
```

Property Default Description
--clover-bell-size 44px Bell size
--clover-bell-badge-bg #ff4757 Badge color
--clover-bell-color #5a4e4e Bell color

### With dropdown tray:

```html
<button class="clover-notification-bell has-notification">
  <span class="clover-bell-badge">5</span>
  <div class="clover-bell-tray open">
    <div class="clover-tray-item unread">🔔 New message from Alex</div>
    <div class="clover-tray-item">⭐ Your PR was merged</div>
    <div class="clover-tray-item">📦 Package shipped</div>
  </div>
</button>
```

### 15. .clover-drag-ghost

```html
<div class="clover-drag-ghost" style="display:flex;align-items:center;justify-content:center;color:white;">
  Drag Me
</div>
```

Property Default Description
--clover-drag-size 160px Card size
--clover-drag-bg gradient Card background
--clover-drag-ghost-opacity 0.3 Ghost trail opacity

### 16. .clover-spotlight-card

```html
<div class="clover-spotlight-card">
  <h3>🔦 Spotlight</h3>
  <p>Move your cursor over me!</p>
</div>
```

Property Default Description
--clover-spotlight-bg #1a1a2e Card background
--clover-spotlight-color purple Spotlight color
--clover-spotlight-size 300px Spotlight radius

### Optional JS for cursor tracking (same pattern as magnetic container):

```javascript
document.querySelectorAll('.clover-spotlight-card').forEach(card => {
  card.addEventListener('mousemove', e => {
    const rect = card.getBoundingClientRect();
    card.style.setProperty('--_mouse-x', (e.clientX - rect.left) / rect.width);
    card.style.setProperty('--_mouse-y', (e.clientY - rect.top) / rect.height);
  });
  card.addEventListener('mouseleave', () => {
    card.style.setProperty('--_mouse-x', 0.5);
    card.style.setProperty('--_mouse-y', 0.5);
  });
});
```

### 17. .clover-toggle-realm

```html
<label class="clover-toggle-realm">
  <input type="checkbox">
  <span class="clover-toggle-track"></span>
  <span class="clover-toggle-thumb"></span>
</label>
```

Property Default Description
--clover-toggle-on #feca57 Sun color (on)
--clover-toggle-off #dfe6e9 Moon color (off)
--clover-toggle-width 64px Track width
--clover-toggle-height 32px Track height

### 18. .clover-tooltip-magic

```html
<span class="clover-tooltip-magic">
  Hover for tip
  <span class="clover-tooltip-body">I'm a magical tooltip! ✨</span>
</span>
```

### Directions:

```html
<span class="clover-tooltip-body" data-tooltip-dir="top">Top tooltip</span>
<span class="clover-tooltip-body" data-tooltip-dir="bottom">Bottom tooltip</span>
<span class="clover-tooltip-body" data-tooltip-dir="left">Left tooltip</span>
<span class="clover-tooltip-body" data-tooltip-dir="right">Right tooltip</span>
```

Property Default Description
--clover-tooltip-bg dark glass Tooltip background
--clover-tooltip-accent purple Accent color
--clover-tooltip-speed 0.4s Animation speed

### 19. .clover-marquee-banner

```html
<div class="clover-marquee-banner">
  <div class="clover-marquee-track">
    <span>🚀 Announcement 1</span>
    <span>🍀 Announcement 2</span>
    <span>⭐ Announcement 3</span>
    <span>🚀 Announcement 1</span>
    <span>🍀 Announcement 2</span>
    <span>⭐ Announcement 3</span>
  </div>
</div>
```

Property Default Description
--clover-marquee-speed 20s Scroll speed
--clover-marquee-bg #1a1a2e Background
--clover-marquee-fade 60px Edge fade width

### 20. .clover-progress-cosmic

```html
<div class="clover-progress-cosmic" style="--clover-progress:70%;">
  <div class="clover-progress-fill"></div>
  <div class="clover-progress-head"></div>
</div>
```

Property Default Description
--clover-progress 60% Progress percentage
--clover-progress-fill gradient Fill gradient
--clover-progress-glow purple Head glow color
--clover-progress-speed 0.6s Animation speed

---

## 🎨 Theming

### Every component exposes custom properties. Theme globally:

```css
:root {
  --clover-glass-blur: 24px;
  --clover-clay-bg: #e8e0f0;
  --clover-neubrutal-bg: #00ff88;
  --clover-cyber-border-color-1: #ff4444;
  --clover-spotlight-color: rgba(0, 200, 83, 0.3);
}
```

### Or per-instance:

```html
<div class="clover-glass-card" style="--clover-glass-pulse-duration: 2s;">
  Faster pulse!
</div>
```

---

## 🌓 Dark Mode

Dark mode is automatic via prefers-color-scheme: dark. Every component has built-in dark variants with adjusted shadows, colors, and glow intensities.

No extra classes needed. It just works.

---

## ♿ Accessibility

· All components respect prefers-reduced-motion: reduce
· :focus-visible states on every interactive component
· Sufficient contrast ratios in both light and dark modes
· Keyboard navigable where applicable
· No pointer-events: none on interactive elements

---

## 🌐 Browser Support

| Feature | Chrome | Firefox | Safari | Edge |
|---|---|---|---|---|
| `backdrop-filter` | 76+ | 103+ | 18+ | 79+ |
| `conic-gradient` | 69+ | 83+ | 12.1+ | 79+ |
| `mix-blend-mode` | 41+ | 32+ | 8+ | 79+ |
| `clip-path` | 55+ | 54+ | 9.1+ | 79+ |
| `mask-image` | 1+ | 53+ | 15.4+ | 79+ |
| `color-mix()` | 111+ | 113+ | 16.2+ | 111+ |
| CSS `@property` | 85+ | 128+ | 16.4+ | 85+ |
| SVG `feTurbulence` | 1+ | 1+ | 1+ | 79+ |
| `perspective` / 3D | 36+ | 16+ | 9+ | 12+ |
| `steps()` timing | 8+ | 4+ | 5+ | 12+ |
| `prefers-reduced-motion` | 74+ | 63+ | 10.1+ | 79+ |
| `prefers-color-scheme` | 76+ | 67+ | 12.1+ | 79+ |
---

## ⚡ Performance

Despite the complexity, Clover CSS is performant:

· GPU-accelerated backdrop-filter, box-shadow, and transform
· SVG filters are GPU-accelerated in modern browsers
· prefers-reduced-motion eliminates all animations for accessibility
· Zero JavaScript means zero runtime overhead
· Full library: ~91 KB uncompressed, ~15 KB gzipped

---

## 📂 File Structure

```
clover-css/
├── clover.css          # Full source (7,000+ lines of madness)
├── index.html          # 20-component showcase demo
├── docs.html           # Complete documentation
├── license.html        # MIT License page
├── LICENSE             # Plain text MIT license
├── README.md           # You are here
└── package.json        # NPM configuration
```

---

## 🤝 Contributing

We need more insane components! Can you make:

· .clover-weather-widget — 47 keyframe weather animations?
· .clover-audio-visualizer — Pure CSS bar animations?
· .clover-particle-field — 100+ box-shadow particles?

### How to Contribute

1. Fork the repo
2. Create a branch: git checkout -b my-insane-component
3. Write your component (minimum 150 lines!)
4. Submit a PR

See **CONTRIBUTING.md** for full guidelines.

---

## ❓ FAQ

**Q: Is this a joke?**
A: **Yes and no**. Every component is production-capable. The implementation is deliberately overengineered. It's functional art.

**Q: Why 12 box-shadows on one button?**
A: B**ecause 11 wasn't enough, and 13 would be excessive**. Each shadow serves a specific role in the clay/neumorphic illusion.

**Q: Does this impact performance?**
A: **No.** Modern GPUs handle these effects efficiently. The prefers-reduced-motion fallback ensures accessibility.

**Q: Can I use this in production?**
A: **Absolutely**. It's MIT licensed. Go wild.

**Q: Why no JavaScript?**
A: Because **real CSS wizards don't need it.**

---

## 📄 License

MIT © 2026 Clover CSS Contributors

Free to use, modify, and distribute. See LICENSE for full text.

---

## 🔗 Links

· NPM: npmjs.com/package/clover-css-lib
· GitHub: github.com/spideythedev/clover-css
· Live Demo: spideythedev.github.io/clover-css
· Documentation: docs.html
· License: license.html

---

## 🍀 The Clover Promise

No utility classes. No .p-4 .m-2 .bg-blue-500. One class. Absolute CSS chaos. Beautiful results.

Clover CSS — Because you hate yourself, and we respect that.

---

*Made with 🍀 and questionable life choices.*
