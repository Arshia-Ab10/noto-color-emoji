<div align="center">
  <img src="https://raw.githubusercontent.com/Arshia-Ab10/noto-color-emoji/refs/heads/main/src/flags/IR.svg" alt="Iranian Lion and Sun Flag" width="160">
  
  # Noto Color Emoji with Iranian Lion & Sun Flag

  [![jsDelivr](https://data.jsdelivr.com/v1/package/gh/Arshia-Ab10/noto-color-emoji/badge)](https://www.jsdelivr.com/package/gh/Arshia-Ab10/noto-color-emoji)
  [![License: OFL-1.1](https://img.shields.io/badge/License-OFL--1.1-blue.svg)](LICENSE)
  [![Format: COLRv1 / WOFF2](https://img.shields.io/badge/Format-COLRv1%20%2F%20WOFF2-success.svg)](#)
  [![Desktop: TTF](https://img.shields.io/badge/Desktop-TTF%20Included-orange.svg)](fonts/)

  <p>An optimized, modular webfont release of Google's <b>Noto Color Emoji</b> (COLRv1 vector standard), featuring the restored historic national <b>Lion and Sun flag of Iran</b> (1964 standard).</p>
</div>

---

## 📖 Overview

This repository provides **10 modular, on-demand WOFF2 subsets** designed for blazing-fast web performance via the **jsDelivr CDN**, alongside a standalone **desktop font (`.ttf`)** for local installation on Windows, macOS, and Linux.

---

## ✨ Features

- **Accurate Vector National Flag:** Replaced the Iranian flag glyph (`u1F1EE_u1F1F7`) with the 1964 national emblem, processed through Google's official flag-waving pipeline (`naive_warp.py`) to retain mathematical wave curves, 3D perspective lighting, and standard Noto borders.
- **High-Performance Modular Delivery:** Split into 10 semantic WOFF2 sub-chunks configured with precise `unicode-range` rules. Browsers download only the chunk requested by the content (e.g., only the flags subset), resulting in near-instant load times.
- **Intact OpenType GSUB Ligatures:** Preserves all binary substitution tables, skin tone modifiers, and multi-character ZWJ sequences. Regional indicator pairs (`U+1F1EE` + `U+1F1F7`) substitute cleanly without falling back to individual letters.
- **Cross-Platform Support:** Ready for instant web integration via CDN or local desktop installation across operating systems and creative applications.

---

## 🚀 Quick Start

### 1. Web Integration (CDN)

Add the following stylesheet inside the `<head>` of your HTML document:

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/Arshia-Ab10/noto-color-emoji@main/dist/font.css">
```

*(Recommended for production: pin to a specific release tag, e.g., `@v1.0.0`)*

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/Arshia-Ab10/noto-color-emoji@v1.0.0/dist/font.css">
```

### 2. Apply in CSS

Add `'Noto Color Emoji'` to your font stack:

```css
body {
  font-family: 'Noto Color Emoji', system-ui, -apple-system, sans-serif;
}
```

### 3. Desktop Installation (Windows, macOS, Linux)

If you want to use the font on your local system (e.g., in Telegram Desktop, Microsoft Word, Adobe Photoshop, Illustrator, or system-wide):

1. Download **[`NotoColorEmoji-Regular.ttf`](fonts/NotoColorEmoji-Regular.ttf)** from the [`fonts/`](fonts/) directory (or from the latest [Release](../../releases)).
2. Double-click the downloaded file and click **Install**.
3. Select **Noto Color Emoji** as your active font in any supported software.

---

## 📦 Webfont Subsets Overview

The webfont subsets in [`dist/`](dist/) are categorized into 10 modular chunks:

| File | Category | Description |
| :--- | :--- | :--- |
| **`noto-emoji-flags.woff2`** | **Flags (National)** | All country flags featuring the restored Lion & Sun Iran flag <img src="https://raw.githubusercontent.com/Arshia-Ab10/noto-color-emoji/refs/heads/main/src/flags/IR.svg" alt="Iran Flag" height="20" valign="middle"> |
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

## 📁 Repository Structure

```text
noto-color-emoji/
├── fonts/
│   └── NotoColorEmoji-Regular.ttf    # Full desktop font (COLRv1 vector standard)
├── dist/
│   ├── font.css                      # Unified stylesheet with unicode-range
│   ├── noto-emoji-flags.woff2        # National flags subset
│   └── ...                           # Other 9 modular WOFF2 subsets
├── src/
│   └── flags/
│       └── IR.svg                    # Waved Lion & Sun vector source
├── demo/
│   └── demo.html                     # Live preview and test page
├── README.md
└── LICENSE                           # SIL Open Font License 1.1
```

---

## 🧪 Live Demo

To test font loading, ligature substitutions, and rendering across dark and light backgrounds, open [`demo/demo.html`](demo/demo.html) in any modern browser.

---

## 📄 License & Attribution

- **Base Font:** Copyright © 2022 The Noto Project Authors ([googlefonts/noto-emoji](https://github.com/googlefonts/noto-emoji)).
- **Modifications & Assembly:** Copyright © 2026 Arshia-Ab10.
- **License:** Distributed under the **[SIL Open Font License, Version 1.1](LICENSE)** (OFL-1.1).
