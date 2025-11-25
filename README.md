# 🎨 Van Gogh Studio | Interactive Digital Art

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Technology](https://img.shields.io/badge/HTML5_Canvas-JavaScript-yellow)
![AI](https://img.shields.io/badge/Powered_by-Gemini_AI-purple)

**Van Gogh Studio** is an immersive, browser-based interactive art application. It deconstructs static masterpieces into thousands of living particles, allowing users to interact with the artwork using physics simulations, audio reactivity, and generative AI tools.

This project combines advanced **HTML5 Canvas** manipulation, **Flow Field** algorithms, and the **Google Gemini API** to create a unique blend of classic art and modern technology.

---

## ✨ Key Features

### 🖌️ Interactive Particle System
* **Fluid Simulation:** The artwork comes alive with a custom physics engine. Particles react to mouse movements, creating fluid-like ripples and swirls.
* **Deep Zoom:** A multi-layer canvas system (`Deep`, `Mid`, `Foreground`) provides a parallax effect and depth.
* **Dynamic Density:** Users can adjust particle density in real-time, ranging from "Ultra High" detail to performance-optimized modes.

### 🤖 AI Integration (Gemini)
* **Art Critic Analysis:** Uses Gemini Vision to analyze the current canvas state and provide a poetic, artistic critique.
* **Generative AI Painting:** Describe a scene, and the AI generates a raw SVG representation which is then particle-ized instantly.
* **Prompt Magic:** Enhances simple user prompts into detailed artistic descriptions.

### 🎵 Audio Reactivity
* **Visualizer:** Activates the microphone to make the particles dance to music.
* **Frequency Analysis:** Bass frequencies trigger particle size expansion, while treble frequencies affect movement intensity.

### 🛠️ Creative Tools
* **Neon Mode:** Adds a glow filter and saturation boost for a cyberpunk aesthetic.
* **Shape Shifting:** Switch particle shapes between **Squares**, **Circles**, and **Lines**.
* **Color Studio:** Apply custom HSL color palettes or "Smart Filters" (e.g., typing "Fire" automatically applies a red/orange palette).
* **Auto Pilot:** A "Van Gogh Mode" that automatically applies swirling forces to mimic the *Starry Night* flow.

### 💾 Export & Share
* **Video Recording:** Native support to record high-quality (VP9/WebM) 5-second video clips of the animation.
* **Snapshot:** High-resolution PNG export of the current frame.
* **Undo/Redo System:** Full state management to revert accidental changes.

---

## 🚀 How to Run

### Prerequisites
* A modern web browser (Chrome, Edge, Firefox).
* **Recommended:** A local development server (e.g., VS Code "Live Server" extension) to avoid CORS issues with image loading.

### Installation
1.  Clone or download the repository.
2.  Open the project folder.
3.  Launch `index.html` via a local server.
    * *Note: Opening the file directly (`file://`) may block the canvas from reading image data due to browser security policies.*

### Setting up AI Features
To use the AI features (Analysis & Generation):
1.  Get a free API Key from [Google AI Studio](https://aistudio.google.com/app/apikey).
2.  Open the **AI Tools** section in the sidebar.
3.  Paste your key into the "Paste Gemini API Key Here" field.
4.  The key is saved locally in your browser (`localStorage`).

---

## 🎮 Controls

| Control | Action |
| :--- | :--- |
| **Left Click + Drag** | Repel particles or Paint flow (depending on tool) |
| **Sidebar Toggle** | Click the header to collapse/expand the UI |
| **Eye Icon (View)** | Interactive Physics Mode (Repel particles) |
| **Brush Icon** | Flow Paint Mode (Draw wind directions) |
| **Spacebar** | Not mapped (Reserved for future shortcuts) |
| **Enter** | Apply typed filter in Color Studio |

---

## 🛠️ Tech Stack

* **Frontend:** HTML5, CSS3 (Glassmorphism UI), Vanilla JavaScript (ES6+).
* **Rendering:** HTML5 `<canvas>` API (2D Context).
* **Physics:** Custom verlet-integration inspired physics loop.
* **AI:** Google Generative Language API (Gemini 2.5 Flash).
* **Fonts:** Google Fonts (Playfair Display, Inter, Courgette).

---

## 📂 Project Structure

```text
/
├── index.html        # Main application file (CSS/JS included)
└── README.md         # Documentation
