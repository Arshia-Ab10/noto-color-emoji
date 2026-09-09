<div align="center">
  <p align="center">
    <img src="https://raw.githubusercontent.com/Arshia-Ab10/noto-emoji/main/third_party/region-flags/waved-svg/emoji_u1f1ee_1f1f7.svg" alt="Iran (Lion and Sun)" height="44" style="vertical-align: middle; margin: 0 4px;">
    <img src="https://raw.githubusercontent.com/Arshia-Ab10/noto-emoji/main/third_party/region-flags/waved-svg/emoji_u1f1fa_1f1f8.svg" alt="United States" height="44" style="vertical-align: middle; margin: 0 4px;">
    <img src="https://raw.githubusercontent.com/Arshia-Ab10/noto-emoji/main/third_party/region-flags/waved-svg/emoji_u1f1e9_1f1ea.svg" alt="Germany" height="44" style="vertical-align: middle; margin: 0 4px;">
    <img src="https://raw.githubusercontent.com/Arshia-Ab10/noto-emoji/main/third_party/region-flags/waved-svg/emoji_u1f1ee_1f1f1.svg" alt="Israel" height="44" style="vertical-align: middle; margin: 0 4px;">
    <img src="https://raw.githubusercontent.com/Arshia-Ab10/noto-emoji/main/third_party/region-flags/waved-svg/emoji_u1f1ec_1f1e7.svg" alt="United Kingdom" height="44" style="vertical-align: middle; margin: 0 4px;">
    <img src="https://raw.githubusercontent.com/Arshia-Ab10/noto-emoji/main/third_party/region-flags/waved-svg/emoji_u1f1ef_1f1f5.svg" alt="Japan" height="44" style="vertical-align: middle; margin: 0 4px;">
  </p>

  # Noto Color Emoji (COLRv1)

  **High-Performance Modular Webfont Subsets & Desktop Font**

  [![jsDelivr](https://data.jsdelivr.com/v1/package/gh/Arshia-Ab10/noto-emoji/badge)](https://www.jsdelivr.com/package/gh/Arshia-Ab10/noto-emoji)
  [![License: OFL-1.1](https://img.shields.io/badge/License-OFL--1.1-blue.svg)](LICENSE)
  [![Format: COLRv1 / WOFF2](https://img.shields.io/badge/Format-COLRv1%20%2F%20WOFF2-success.svg)](#)
  [![Desktop: TTF](https://img.shields.io/badge/Desktop-TTF%20Included-orange.svg)](fonts/)

  <p>An optimized, production-grade distribution of Google's <b>Noto Color Emoji</b> (COLRv1 vector standard). Delivers 10 ultra-lightweight, on-demand WOFF2 subsets via CDN alongside a standalone desktop font, featuring the restored <b>Iranian Lion and Sun national flag</b>.</p>
</div>

---

## 📖 Overview

Google's official color emoji font is rich and expressive, but full builds can exceed 20 MB, making them impractical for standard web use. 

This repository solves that by providing **10 modular WOFF2 subsets** partitioned with precise `unicode-range` definitions. Browsers load only the exact categories requested by the page on demand. Additionally, it integrates the restored historical 1964 Iranian national emblem (**Lion and Sun** / شیر و خورشید) directly into the regional indicator sequence (`🇮🇷`), rendered with official Google waving geometry.

---

## ✨ Features

- **Blazing-Fast Web Delivery:** Divided into 10 semantic WOFF2 subsets. Sites only download what they use (e.g., just flags or smileys), providing instant rendering without large payloads.
- **Restored Iranian Lion & Sun Flag:** The national flag sequence (`u1F1EE_u1F1F7`) is replaced with the authentic 1964 emblem, processed via Google's `naive_warp.py` pipeline to preserve mathematical wave ripples, standard borders, and 3D lighting.
- **Full GSUB Ligature Integrity:** Preserves all OpenType substitution tables, multi-codepoint ZWJ sequences, gender combinations, and skin-tone modifiers across all world flags and symbols.
- **Cross-Platform Compatibility:** Easily imported into any web app via the jsDelivr CDN or installed locally (`.ttf`) on Windows, macOS, and Linux for design suites, text editors, and apps.

---

## 🚀 Quick Start

### 1. Web Integration (CDN)

Add the stylesheet to the `<head>` of your website:

```html
<!-- Always latest -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/Arshia-Ab10/noto-emoji@main/dist/font.css">
```

*(Recommended for production: pin to a specific release tag)*

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/Arshia-Ab10/noto-emoji@v1.0.0/dist/font.css">
```

### 2. Apply in CSS

Include `'Noto Color Emoji'` in your font stack:

```css
body {
  font-family: 'Noto Color Emoji', system-ui, -apple-system, sans-serif;
}
```

### 3. Desktop Installation (Windows, macOS, Linux)

1. Download **[`NotoColorEmoji-Regular.ttf`](fonts/NotoColorEmoji-Regular.ttf)** from the [`fonts/`](fonts/) directory or the latest [Release](../../releases).
2. Open the file and click **Install**.
3. Select **Noto Color Emoji** in Telegram, Photoshop, Illustrator, Office, or terminal emulators.

---

## 📦 Modular Subsets

| Subset File | Category | Content Summary |
| :--- | :--- | :--- |
| **`noto-emoji-flags.woff2`** | **National Flags** | All country flags, including restored Lion & Sun Iran flag <img src="https://raw.githubusercontent.com/Arshia-Ab10/noto-emoji/refs/heads/main/src/flags/IR.svg" alt="Iran Flag" height="18" valign="middle"> |
| **`noto-emoji-flags-special.woff2`** | **Special Flags** | Rainbow, pirate, transgender, and regional subdivision flags |
| **`noto-emoji-symbols.woff2`** | **Symbols & Signs** | Arrows, colored hearts, geometric figures, zodiac, math & status icons |
| **`noto-emoji-objects.woff2`** | **Objects & Tools** | Tech, tools, books, office equipment, clothing, household items |
| **`noto-emoji-activities.woff2`** | **Sports & Games** | Sports gear, musical instruments, medals, awards, hobbies |
| **`noto-emoji-travel.woff2`** | **Travel & Places** | Vehicles, aviation, architecture, landmarks, transit |
| **`noto-emoji-food.woff2`** | **Food & Drink** | Fruits, vegetables, meals, drinks, utensils, desserts |
| **`noto-emoji-nature.woff2`** | **Animals & Nature** | Animals, plants, weather phenomena, astronomy, nature |
| **`noto-emoji-people.woff2`** | **People & Body** | Professions, families, body parts, gestures, skin tones |
| **`noto-emoji-smileys.woff2`** | **Smileys & Emotions** | Standard facial expressions, hand signs, emotions |

---

## 📁 Repository Structure

```text
noto-emoji/
├── fonts/
│   └── NotoColorEmoji-Regular.ttf    # Standalone desktop font (COLRv1)
├── dist/
│   ├── font.css                      # Unified CDN stylesheet with unicode-range
│   ├── noto-emoji-flags.woff2        # National flags chunk
│   └── ...                           # 9 additional modular WOFF2 chunks
├── src/
│   └── flags/
│       └── IR.svg                    # Waved Lion & Sun flag vector
├── demo/
│   └── demo.html                     # Multi-country interactive demo
├── README.md
└── LICENSE                           # SIL Open Font License 1.1
```

---

## 🧪 Live Demo

To inspect rendering, test ligature substitution across countries, and preview light and dark contrast, open [`demo/demo.html`](demo/demo.html) in any modern browser.

---

## 📄 License & Attribution

- **Base Font:** Copyright © 2022 The Noto Project Authors ([googlefonts/noto-emoji](https://github.com/googlefonts/noto-emoji)).
- **Modifications & Subsetting:** Copyright © 2026 Arshia-Ab10.
- **License:** Distributed under the **[SIL Open Font License, Version 1.1](LICENSE)** (OFL-1.1).
