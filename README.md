# ORRERY - SOLAR SYSTEM EXPLORER

An interactive, responsive HTML5 Canvas visualization and field guide for our Solar System. Built using pure JS, CSS3 and HTML5 without any external framework dependencies, this application provides an educational 2D orbital model paired with live data fetched directly from NASA's public API.

---

## Key Features

* **Dynamic Orbital Simulation:** Real-time top-down animation of the 8 planets orbiting the Sun with configurable animation speed ('1x', '44x', '12x') and pause /resime controls.
* **Interactive Planet Field Guide:** Click on any planet in the canvas to open a detailed mission briefing panel featuring planet stats, physical composition, unique facts, and moon counts.
* **Live NASA Image Gallery:** Dynamically queries the `images-api.nasa.gov` REST API to fetch real surface and mission imagery for the selected planet.
* **Event Watch (Conjunction Detection):** Calculates angular proximity between planet orbits relative to the Sun and alerts the user to close apparent alignments.
* **Responsive HUD & Custom Styling:** Built with a modern dark-space UI theme that adapts seamlessly to desktop, tablet, and mobile screens.

---

## 📁 Project Structure

This project is authored as a single, self-contained single-file application (`orrery_solar_system.html`) for quick deployment and zero-configuration execution:

```
├── orrery_solar_system.html    # Contains HTML structures, CSS variables/styles, and JS engine
└── README.md                   # Project documentation
```

---

## 🚀 Getting Started

### Prerequisites

No build tools, package managers (`npm`/`yarn`), or backend servers are required. The only requirement for full functionality (including NASA image fetching) is an active internet connection and any modern web browser.

### Running the Application

1. Download or clone the `orrery_solar_system.html` file.
2. Open `orrery_solar_system.html` in your web browser of choice:
   - **Chrome / Firefox / Edge / Safari:** Double-click the file, or drag and drop it into an open browser tab.

---

## 🎮 How to Use

| Control | Action | Description |
| :--- | :--- | :--- |
| **Canvas Click** | Left-click any planet | Opens the detailed field guide panel and loads NASA imagery for that world. |
| **Pause / Resume** | Click `Ⅱ Pause` / `▶ Resume` | Freezes or unfreezes planetary motion. |
| **Speed Toggle** | Click `1× Speed` | Cycles playback speed between `1×`, `4×`, and `12×`. |
| **Reset** | Click `↺ Reset` | Resets elapsed simulation time back to 0. |
| **Planet Labels** | Toggle `Planet labels` | Shows or hides planet name tags on the canvas. |
| **Orbit Paths** | Toggle `Orbit paths` | Toggles rendering of elliptical orbital lines. |
| **Event Watch** | Toggle `Event watch` | Enables or disables top-down alignment banners. |
| **Show All** | Click `Show all` | Clears current planet selection and reverts the sidebar to system overview. |

---

## 🛠️ Technical Overview

* **Rendering Engine:** HTML5 2D Canvas context rendering gradients, atmospheric halos, procedural solar surface granules, planetary textures, moon orbits, and rings (Saturn & Uranus).
* **Scale Note:** Planet diameters are rendered on a scaled linear proportion relative to the Sun for visual distinction. Target hitboxes for clicks are enlarged to maintain usability across all screen sizes.
* **Data Sources:** 
  * Satellite & Planetary counts derived from NASA Goddard Planetary Fact Sheet and JPL Solar System Dynamics data.
  * Image Archive: [NASA Image and Video Library API](https://images.nasa.gov/docs/images.nasa.gov_api_docs.pdf).

---

## 📜 License

Distributed under the MIT License. Feel free to modify and adapt for educational or personal projects!
