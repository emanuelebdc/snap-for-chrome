# EmaF205 SNAP // Lightweight Viewport Capture & Framing Utility

<p align="center">
  <img src="assets/social-preview.jpg" alt="EmaF205 SNAP Social Banner" width="100%">
</p>

> **"Crisp viewport framing without bloated recording suites. Capture, frame, and export in 4 seconds."**  
> A high-precision, client-side viewport framing and screenshot composition tool engineered for developers, educators, and product designers. Frames web application captures into standardized aspect ratios with subtle translucent device bezels and zero cloud dependencies.

[![GitHub Repo](https://img.shields.io/badge/GitHub-emanuelebdc%2Fsnap--for--chrome-black?style=for-the-badge&logo=github&logoColor=white)](https://github.com/emanuelebdc/snap-for-chrome)
[![Chrome MV3](https://img.shields.io/badge/Chrome-Extension_MV3-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white)](https://github.com/emanuelebdc/snap-for-chrome)
[![Client-Side Privacy](https://img.shields.io/badge/Privacy-100%25_Local-10b981?style=for-the-badge)](https://github.com/emanuelebdc/snap-for-chrome)
[![Aspect Ratios](https://img.shields.io/badge/Presets-16%3A9_%7C_4%3A3_%7C_1%3A1_%7C_9%3A16-dfff00?style=for-the-badge&logoColor=000000)](https://github.com/emanuelebdc/snap-for-chrome)
[![License: MIT](https://img.shields.io/badge/License-MIT-black?style=for-the-badge)](LICENSE)

---

## ✦ The Genesis & Why This Exists

When documenting software architectures, writing educational case studies, or sharing project updates on GitHub and LinkedIn, presentation matters. Yet the daily workflow for capturing and presenting interfaces is broken:

1. **The Native Screenshot Trap**: Taking raw desktop screenshots leaves uneven window borders, distracting background clutter, or non-standard aspect ratios that get awkwardly cropped or letterboxed on social feeds.
2. **The Bloated Desktop App Trap**: Dedicated mockup tools and recording suites are frequently 500MB+ Electron applications that take seconds to launch, demand paid cloud subscriptions, or upload confidential screen captures to third-party servers.

I built **EmaF205 SNAP** in Milan to solve this routine friction once and for all: **a featherweight, zero-server capture and framing utility that runs entirely inside your browser sandbox.** 

Drop a screenshot, paste from clipboard, select your desired ratio (16:9, 4:3, 1:1, or mobile 9:16), apply clean typographic framing guides, and download crisp, publication-ready images in under four seconds.

---

## ✦ Visual Interface & Operational Overview

<p align="center">
  <img src="assets/emaf205-snap-overview.png" alt="EmaF205 SNAP Interface & Framing Overview" width="100%">
</p>

---

## ✦ Core Capabilities

- **Precision Aspect Ratio Engine**: Instant presets for **16:9** (YouTube / Slides / Case Studies), **4:3** (Technical Documentation), **1:1** (Social Feeds), and **9:16** (Mobile Viewports).
- **Subtle Glass Viewport Framing**: Translucent device bezel overlay with clean edge radii, eliminating visual noise while maintaining architectural focus.
- **Dual Runtime Architecture**: Can be installed as an unpacked **Google Chrome / Microsoft Edge Extension (Manifest V3)** or launched as a standalone static web app (`capture.html`).
- **High-DPI Canvas Rendering**: Computes pixel-perfect compositing on high-density Retina displays without fuzzy interpolation or subpixel blurring.
- **Instant Clipboard Pipeline**: Paste images directly with <kbd>Cmd</kbd> + <kbd>V</kbd> / <kbd>Ctrl</kbd> + <kbd>V</kbd> and copy results with one click.
- **100% Client-Side Privacy**: Zero data leaves your device. All image transformations and raster operations happen strictly inside browser RAM.

---

## ✦ Scheda Tecnica // Technical Specifications

| Parametro | Specifica Tecnica |
|:---|:---|
| **Ambiente di Esecuzione** | Google Chrome / Microsoft Edge / Safari / Firefox (Modern Evergreen Browsers) |
| **Architettura Software** | 100% Client-Side (HTML5 Canvas 2D + ES6+ JavaScript Vanilla) |
| **Dipendenze Esterne** | **0** (Nessun framework, nessuna libreria npm, zero build pipeline) |
| **Modalità Operative** | 1. Estensione Browser Chrome Manifest V3 (`manifest.json`)<br/>2. Web App Standalone offline (`capture.html`) |
| **Formati Input Supportati** | Incolla da appunti (`image/png`), Drag-and-Drop file PNG, JPEG, WebP |
| **Formati Output** | PNG ad alta risoluzione (Lossless Retina) / JPEG compresso ad alta fedeltà |
| **Privacy e Sicurezza** | Zero server backend, zero telemetria, zero cookie, conformità GDPR totale |
| **Rapporti d'Aspetto** | 16:9 (1920x1080), 4:3 (1600x1200), 1:1 (1200x1200), 9:16 (1080x1920) |
| **Accessibilità** | Focus ad alto contrasto, scorciatoie da tastiera, zero elementi microscopici |

---

## ✦ Struttura del Progetto

```text
snap-for-chrome/
├── manifest.json             # Configurazione Manifest V3 per estensione Chrome
├── capture.html              # Interfaccia grafica di framing standalone
├── capture.js                # Motore logico Canvas, gestione eventi e rendering
├── icons/                    # Set di icone ad alta risoluzione (16, 32, 48, 128px)
├── assets/                   # Copertine, social banner e documentazione visiva
│   ├── social-preview.jpg    # Banner 16:9 hero per GitHub e social
│   └── emaf205-snap-overview.png # Screenshot operativo completo
├── dist/                     # Pacchetti pronti per la distribuzione
├── docs/                     # Rapporti di test e verifiche
└── README.md                 # Documentazione ufficiale
```

---

## ✦ Quickstart & Istruzioni di Avvio

### Metodo 1: Web App Standalone (Immediato)
Non richiede installazione:
1. Clona la repository:
   ```bash
   git clone https://github.com/emanuelebdc/snap-for-chrome.git
   cd snap-for-chrome
   ```
2. Apri `capture.html` con un doppio clic in qualsiasi browser.
3. Incolla o trascina l'immagine da inquadrare ed esporta il risultato.

### Metodo 2: Estensione Chrome (Manifest V3)
1. Apri Google Chrome o Edge e naviga su `chrome://extensions/`.
2. Attiva la modalità sviluppatore (**Developer mode**) in alto a destra.
3. Clicca su **Carica estensione non pacchettizzata** (**Load unpacked**).
4. Seleziona la cartella del repository `snap-for-chrome`.
5. L'icona di SNAP apparirà nella barra degli strumenti per un accesso istantaneo.

---

## ✦ Autore & Filosofia del Progetto

Ideato, progettato e sviluppato da **[Emanuele BDC](https://emaf205.com)** a Milano.  
Parte dell'ecosistema di strumenti digitali ad alta efficienza e zero backend di **Emanuele BDC / EmaF205**.

Rilasciato sotto licenza open-source **[MIT License](LICENSE)**. Libero per utilizzi personali, accademici e commerciali.
