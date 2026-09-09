# Noto Color Emoji with Iranian Lion & Sun Flag 🦁☀️

[![jsDelivr](https://data.jsdelivr.com/v1/package/gh/Arshia-Ab10/noto-color-emoji/badge)](https://www.jsdelivr.com/package/gh/Arshia-Ab10/noto-color-emoji)
[![License: OFL-1.1](https://img.shields.io/badge/License-OFL--1.1-blue.svg)](LICENSE)
[![Format: COLRv1 / WOFF2](https://img.shields.io/badge/Format-COLRv1%20%2F%20WOFF2-success.svg)](#)

A modernized, modular webfont release of Google's **Noto Color Emoji** (COLRv1 vector format), featuring the restored historic and national **Lion and Sun flag of Iran** (پرچم شیر و خورشید ایران, 1964 standard).

This repository provides **10 lightweight, on-demand WOFF2 subsets** designed for maximum web performance, accessible globally via the fast **jsDelivr CDN** without requiring users to download the full, heavy font.

---

## ✨ Features

- **Accurate Mathematical Vector Flag:** Designed based on the official 1964 Iranian national flag standard and processed through Google's official flag-waving toolchain (`naive_warp.py`) to preserve authentic sinusoidal curves, 3D lighting, perspective warping, and Noto border overlays.
- **Modular `unicode-range` Delivery:** The font is split into 10 semantic subsets. Browsers only fetch the specific chunk required by the page (e.g., only the flags subset), resulting in near-instant load times and zero network bloat.
- **Intact OpenType GSUB & Ligatures:** Full support for ZWJ sequences, skin tone modifiers, multi-character expressions, and flag ligatures. Regional indicator characters (`U+1F1EE` + `U+1F1F7`) cleanly substitute without splitting into separate letters.
- **Zero-Config CDN Integration:** Can be added to any web project with a single CSS `<link>` tag.

---

## 🚀 Quick Start

### 1. Include via CDN

Add the following `<link>` inside the `<head>` of your HTML document:

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/Arshia-Ab10/noto-color-emoji@main/dist/font.css">
```

*(Recommended for production: lock to a specific release tag, e.g., `@v1.0.0` instead of `@main`)*

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/Arshia-Ab10/noto-color-emoji@v1.0.0/dist/font.css">
```

### 2. Apply in CSS

Add `'Noto Color Emoji'` to your CSS font stack:

```css
body {
  font-family: 'Noto Color Emoji', system-ui, -apple-system, sans-serif;
}
```

---

## 📦 Webfont Subsets Overview

The font files located in [`dist/`](dist/) are structured as follows:

| File | Content Category | Description |
| :--- | :--- | :--- |
| **`noto-emoji-flags.woff2`** | **Flags (National)** | All country flags featuring the restored Lion & Sun Iran flag (`🇮🇷`) |
| **`noto-emoji-flags-special.woff2`** | **Flags (Special / Regional)** | Rainbow, pirate, transgender, and subdivision tags (Scotland, Wales, etc.) |
| **`noto-emoji-symbols.woff2`** | **Symbols & Signs** | Arrows, colored hearts, geometric shapes, zodiac, and punctuation |
| **`noto-emoji-objects.woff2`** | **Objects & Tools** | Tech, office supplies, clothing, tools, books, and household items |
| **`noto-emoji-activities.woff2`** | **Sports & Activities** | Sports gear, musical instruments, games, medals, and celebrations |
| **`noto-emoji-travel.woff2`** | **Travel & Places** | Vehicles, aircraft, ships, architecture, buildings, and maps |
| **`noto-emoji-food.woff2`** | **Food & Drink** | Fruits, vegetables, meals, snacks, sweets, and beverages |
| **`noto-emoji-nature.woff2`** | **Animals & Nature** | Mammals, birds, insects, plants, weather, moon phases, and space |
| **`noto-emoji-people.woff2`** | **People & Body** | Professions, couples, families, body gestures, and skin tones |
| **`noto-emoji-smileys.woff2`** | **Smileys & Emotions** | Classic facial expressions, hands, gestures, and emotions |

---

## 🧪 Live Demo

You can view and test the webfont rendering in both light and dark themes using [`demo/demo.html`](demo/demo.html), or preview it live through the repository's GitHub Pages.

---

## 📄 License & Attribution

- **Base Font:** Copyright © 2022 The Noto Project Authors ([googlefonts/noto-emoji](https://github.com/googlefonts/noto-emoji)).
- **Modifications & Distribution:** Copyright © 2026 Arshia-Ab10.
- **License:** Distributed under the **[SIL Open Font License, Version 1.1](LICENSE)** (OFL-1.1).
