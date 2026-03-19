A single-file, zero-dependency web app for visualizing atoms and molecules in 3D — with a built-in science AI assistant.

> **No install. No server. Just open `atom3d.html` in a browser.**

---

## Features

### 🔭 Atom Viewer
- Animated 3D Bohr model for all 118 elements
- Search by element name, symbol, or atomic number
- Info panel: atomic number, protons, neutrons, atomic mass, electron shell configuration
- 3 fun facts per element
- **Download as STL** for 3D printing

### 🔗 Bond Builder
- Combine 2–3 elements to see their 3D molecule
- Number inputs beside each element to specify atom counts (e.g. H×2 + O×1)
- ~20 built-in compounds: water, ammonia, methane, salt, rust, sulfuric acid, and more
- CPK-colored ball-and-stick models with bond type, shape, and bond angle
- Includes a description with real-world context for each compound

### 🤖 Science AI Chat
- Ask anything about chemistry, physics, biology, elements, or molecules
- Pulls live data from multiple free APIs:
  - 📖 **Wikipedia** — reads up to 3 full articles and synthesizes the best sentences
  - 🧪 **PubChem** — molecular formulas, weights, and IUPAC names
  - 🦆 **DuckDuckGo** — instant answers
  - 🌐 **Wikidata** — structured entity descriptions
  - 🚀 **NASA Images API** — space and astronomy queries
  - 🔢 **Numbers API** — numeric facts
- Learns from your conversation (within the session)
- Built-in material composition lookup (~70 materials: water, steel, DNA, glass, and more)
- App navigation help built in ("how do I use the bond builder?", "suggest some bonds")
- Responses capped at 75 words for readability
- Filters out irrelevant Wikipedia articles (TV shows, films)

---

## How to Use

1. Download `atom3d.html`
2. Open it in any modern browser (Chrome, Firefox, Edge)
3. **Atom Viewer:** type an element name, symbol, or number → click Generate
4. **Bond Builder:** click "Bond Builder" (top right) → enter 2–3 elements with counts → click Combine
5. **AI Chat:** click the 🤖 button (bottom right) → ask any science question

### Controls
| Action | How |
|---|---|
| Rotate model | Click and drag |
| Zoom | Scroll wheel |
| Pan | Right-click drag |
| Download STL | Green button in info panel |
| Switch modes | Top-right toggle button |

---

## Tech Stack

| Technology | Use |
|---|---|
| [Three.js v0.160](https://threejs.org/) | 3D rendering (via importmap CDN) |
| OrbitControls | Mouse/touch camera control |
| STLExporter | 3D print export |
| BufferGeometryUtils | Geometry merging for STL |
| Vanilla JS / HTML / CSS | Everything else — no framework |

---

## Supported Compounds (Bond Builder)

| Elements | Compound |
|---|---|
| H + O | Water (H₂O) |
| Na + Cl | Sodium Chloride (NaCl) |
| C + O | Carbon Dioxide (CO₂) |
| H + N | Ammonia (NH₃) |
| C + H | Methane (CH₄) |
| H + Cl | Hydrochloric Acid (HCl) |
| Fe + O | Iron Oxide / Rust (Fe₂O₃) |
| H + O + S | Sulfuric Acid (H₂SO₄) |
| H + N + O | Nitric Acid (HNO₃) |
| C + H + O | Methanol (CH₃OH) |
| H + Na + O | Sodium Hydroxide (NaOH) |
| Ca + C + O | Calcium Carbonate (CaCO₃) |
| C + H + N | Hydrogen Cyanide (HCN) |
| … and more | |

---

## AI Chat Examples

```
"what is the difference between an element and a molecule?"
"what is graphene?"
"what elements make up hydrochloric acid?"
"how do I use the bond builder?"
"suggest some bonds to try"
"what are some key companies in copper mining?"
"remember that I'm studying for a chemistry exam"
```

---

## Notes

- No API keys required — all data sources are free and public
- Memory clears on each page reload (session only)
- STL files open in any 3D printing slicer (Cura, PrusaSlicer, etc.)
- Works fully offline except for the AI chat (which requires internet for API calls)

---

*Built with Three.js and free public APIs. Single file, runs anywhere.*

