[project_readme.md](https://github.com/user-attachments/files/33945825/project_readme.md)
# 🎃 Rolle Ghost Walk: Echoes of Lac Léman & Spectral Malay Lore

An interactive, bilingual web audio guide and horror soundscape designed for a self-guided nighttime ghost walk along the historic lakeside town of **Rolle, Switzerland (Canton of Vaud)**.

The experience fuses atmospheric Swiss Alpine legends with Southeast Asian / Malay spectral folklore across 6 physical waypoints, featuring spatial 3D audio, automated narration with background audio ducking, Google Maps turn-by-turn navigation, and station QR codes.

---

## 🗺️ The Haunted Trail & Stations

The walk spans approximately 1.1 km along the cobblestone streets and dark waters of Lac Léman:

| Stop | Title | Key Themes & Folklore Fusion | Location |
| :---: | :--- | :--- | :--- |
| **0** | **The Boundary Crossing** | Alpine *Arme Seelen* (Poor Souls) & Malay forest threshold invocation (*"Tok Nenek penjaga hutan, cucu tumpang lalu"*) | Chemin de Plein-Air |
| **1** | **The Linden Trees & Penunggu Pokok** | Medieval *Gerichtslinde* (Tribunal Linden) & *Orang Bunian* / *Puaka* tree guardians (*Disorok Hantu*) | Place des Tilleuls |
| **2** | **The Black Shoreline with the Serpents & the Hantu Air** | *Le Monstre du Léman* & the predatory *Hantu Air* lurking in the shallows | Quai de la Harpe |
| **3** | **Château de Rolle & Hantu Pocong** | Rampart gibbet cages, dragging chains & the shrouded, hopping *Pocong* spirit | Château de Rolle |
| **4** | **The Weeping Willow Tree** | Swiss *Weiße Frauen* (White Ladies) & the hanging boughs / piercing laugh (*mengilai*) of the *Pontianak* | Shoreline Willow Path |
| **5** | **The Penanggalan** | Phantom of Île de la Harpe & Southeast Asia's detached vampire head trailing dripping organs | Promenade facing Île de la Harpe |

---

## ✨ Features

- **Antique Manuscript & Blood Aesthetic:** Vintage weathered parchment styling, crinkled paper fiber textures, and organic arterial bleed visuals.
- **Bilingual Interface & Narration:** Instant one-tap toggle between **English** and **Bahasa Indonesia** across all UI elements, lore narratives, and spoken audio scripts.
- **Atmospheric Sequencing & Audio Ducking:** Ambient horror audio and procedural synthesizers introduce each scene before the web speech engine smoothly lowers background volume (audio ducking) to deliver the spoken script directly into the listener's headphones.
- **Spatial 3D Orbit (Binaural Panning):** Real-time stereo panning algorithm that slowly rotates entities around the listener's head in a 360-degree circle to simulate spirits circling the group in the dark.
- **Interactive Trail Mini-Map:** Built-in vector map with active station beacon pulsing and direct deep links to Google Maps for turn-by-turn walking directions.
- **Night-Vision Red Lantern Mode:** Preserves dark-adapted eyesight when navigating uneven cobblestones and tree roots along the unlit lake bank.
- **Station QR Code Generator:** Built-in client-side QR generator for printing station plaques or sharing waypoints instantly via deep link anchors (`#stop-0` through `#stop-5`).
- **Custom Audio Fallback:** Allows tour leads to upload custom field recordings or replacement MP3s directly from their device.

---

## 🚀 Getting Started & Local Setup

### 1. Clone or Download the Repository
```bash
git clone https://github.com/<your-username>/rolle-ghost-walk.git
cd rolle-ghost-walk
```

### 2. Directory Structure
Ensure the root directory contains `index.html` along with the corresponding station ambient audio files:
```text
rolle-ghost-walk/
├── index.html
├── freesound_community-ethnic-malay-music-16877.mp3
├── freesound_community-030822_leaves-rustling-in-wind-79518.mp3
├── freesound_community-witch-forest-atmo-24654.mp3
├── tanweraman-chain-rattling-prison-370007.mp3
├── worldlikeall-witch-noise-260363.mp3
└── README.md
```

### 3. Running Locally
Simply double-click `index.html` or open it with any modern web browser. For the best local testing experience (preventing local audio CORS restrictions), launch a lightweight server:
```bash
# Using Python 3
python -m http.server 8000
```
Then visit `http://localhost:8000` in your browser.

---

## 🌐 Deployment

This application is 100% serverless and client-side:
- **Netlify:** Connect the repository to Netlify with default settings (no build step required). Every `git push` to `main` automatically updates the live website.
- **GitHub Pages:** Enable GitHub Pages under **Settings > Pages > Source (Deploy from a branch > main > /root)**.

---

## 🛠️ Built With

- **HTML5 & Vanilla JavaScript** (Single-file architecture)
- **Web Audio API** (Procedural synthesis, oscillators, stereo panning & real-time oscilloscope canvas)
- **Web Speech API** (SpeechSynthesis with dynamic voice selection and audio ducking)
- **[Tailwind CSS](https://tailwindcss.com/)** (Utility styling via CDN)
- **[Lucide Icons](https://lucide.dev/)** (Vector icons)
- **[QRCode.js](https://davidshimjs.github.io/qrcodejs/)** (Dynamic client-side QR generation)
- **Google Fonts** (*Cinzel*, *Inter*, *Nosifer*)

---

## 🎧 Best Experience Recommendations

1. **Use Stereo Headphones or Earbuds:** Essential for the spatial 3D audio effect.
2. **Enable Night Vision Mode:** Tap the lantern button in the top header to preserve dark adaptation while walking.
3. **Keep Volume at Moderate Levels:** Spectral screeches and sudden atmospheric shifts occur at designated checkpoints.

---

## 📜 License & Credits

- Audio samples sourced under Creative Commons / Public Domain from [Freesound.org](https://freesound.org/).
- Project created for Halloween walking tours and folklore exploration along Lac Léman.
