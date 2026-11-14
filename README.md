# 🌍 Earth Detective: View of the Climate

> *“A spy-satellite console for the climate. Every warming city is a contact. Follow the evidence.”*

**Earth Detective** is an interactive, zero-dependency client-side web application built for climate intelligence and urban heat surveillance. It combines real-time NASA Earth observation data with rigorous statistical trend auditing to analyze warming dynamics across 100 global megacities from 1985 to 2024.

Developed as a submission for the **NASA Space Apps Challenge**.

---

## ✨ Key Features

- **🌐 Immersive 3D WebGL Globe:** Built with **Three.js**, featuring smooth orbital controls, starfields, dynamic lighting, and a spy-satellite console aesthetic complete with custom sensor simulation filters (*Normal, CRT, NVG, FLIR, Noir*).
- **📡 Real-Time NASA Telemetry:** Automatically fetches 40-year monthly point data (2m air temperature, daily maximums, and night-time minimums) from the **NASA POWER API (MERRA-2 reanalysis)**.
- **🛰️ Satellite Verification Layers:** Integrates **NASA GIBS WMS** overlays for **MODIS Land Surface Temperature (LST)** and **VIIRS Black Marble night lights**.
- **📊 Rigorous Statistical Engine:** Implements **Mann-Kendall trend tests**, **Sen’s slope calculations**, **lag-1 autocorrelation (AR1) variance corrections**, and **Benjamini-Hochberg False Discovery Rate (FDR)** adjustments to separate true warming signals from interannual noise.
- **🏙️ 100 Global Megacity Case Files:** Instant search, sorting by warming velocity, automated guided tours, and exportable CSV reports with full provenance data.

---

## 🚀 Quick Start

Because **Earth Detective** is engineered as a zero-backend, self-contained single-file application, running it requires no complex server configuration or package installation.

1. Clone or download this repository.
2. Open `NASA SPACE APPS CHALLENGE 2026.HTML` directly in any modern web browser (Chrome, Firefox, Safari, Edge).
3. Click **INITIALISE** to load the console. *(Note: Requires an active internet connection on first load to fetch live NASA POWER time-series data, which is then cached locally).*

---

## 🛠️ Tech Stack

* **Frontend & Rendering:** HTML5, CSS3, JavaScript (ES6+), **Three.js** (WebGL).
* **Data Sources:** 
  * [NASA POWER Project](https://power.larc.nasa.gov/) (MERRA-2 reanalysis meteorology).
  * [NASA GIBS WMS](https://earthdata.nasa.gov/eosdis/science-system-description/eosdis-components/gibs) (MODIS & VIIRS imagery).
* **Statistical Analysis:** Pure client-side non-parametric time-series processing.

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).
