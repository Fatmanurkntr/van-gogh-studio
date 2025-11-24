# 🎨 Van Gogh Studio - Ultimate Edition

**Van Gogh Studio** is an interactive and generative art application inspired by Vincent van Gogh’s impasto technique, transforming static images into living particle simulations.

The project blends classic computer graphics algorithms (Flow Fields) with modern Generative AI (Google Gemini) to deliver a unique digital art experience.

🔗 **Live Demo:**  
https://Fatmanurkntr.github.io/van-gogh-studio/

---

## ✨ Key Features (What You Can Do)

### 1. 🖌️ Interactive Painting & Animation
- **Living Canvas:** The artwork isn’t static; it flows based on the underlying image data.  
- **Magic Brush:** Bring your canvas to life using mouse or touch gestures.  
- **Freeze & Flow:** Pause the simulation or let it move freely.

### 2. 🎵 Audio Reactive Art
- **Dance with Music:** Enable the microphone—your artwork will move in sync with the rhythm.  
- **Bass & Dynamics:** Strong bass speeds up particles; silence makes them settle.

### 3. 🧠 Hybrid AI Capabilities
- **Smart Filters (No API Required):**  
  Instantly change color palettes with simple words like “Fire”, “Ocean”, “Forest”, or “Matrix”.  
- **Gemini Art Critic:**  
  Get poetic AI-generated critiques of your artwork.  
- **Generative Art (Pro):**  
  Turn text prompts into new SVG visuals (example: *“A cyberpunk city in Van Gogh style”*).

### 4. ⏪ Time Travel (Robust Undo System)
- **Step-by-Step Undo:**  
  Reverse brush movements and filter changes smoothly.  
- **Snapshot Memory:**  
  Because every particle state is stored, rewinding looks natural and seamless.

### 5. 🛠️ Customization Studio
- Adjust particle density, flow speed (viscosity), and brush radius in real time.  
- **Shape Shifting:** Switch between Square, Circle, or Line particle types.  
- **Export:** Save high-resolution PNG images or record 5-second videos.

---

## 🔧 How It Works (The Engineering)

This project is built entirely with **Vanilla JavaScript** and the **HTML5 Canvas API**, with zero dependencies in the core engine.

### 1. Flow Field Algorithm
- **Luminance Calculation:**  
  Each pixel’s brightness is computed as:  
  `0.299R + 0.587G + 0.114B`
- **Vector Mapping:**  
  Brightness values map to directional flow vectors.  
- **Particle Physics:**  
  Thousands of particles follow these invisible vectors, creating a “wind-like brushstroke” effect.

### 2. "Tethered Flow" Physics
- **Liquid Motion:** Particles drift smoothly in the direction of brush movement.  
- **Form Retention:**  
  They never escape the artwork; they return to their origin points.  
- **Underpainting:**  
  Background layers prevent empty black areas.

### 3. Hybrid AI Integration
- **Local Logic (Free):**  
  A hashing-based system creates color palettes from simple text.  
- **Remote API (Google Gemini):**  
  - Image generation  
  - Art analysis  
  - SVG rendering  

---

## 🚀 Tech Stack
- **Frontend:** HTML5, CSS3 (Glassmorphism), JavaScript (ES6+)  
- **Graphics:** HTML5 Canvas API  
- **AI:** Google Gemini API  
- **Hosting:** GitHub Pages

---

## 📦 Installation & Usage

```bash
git clone https://github.com/Fatmanurkntr/van-gogh-studio.git
```

Open `index.html` in any modern browser to start the app.




