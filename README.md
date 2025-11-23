# 🎨 Van Gogh Studio - Ultimate Edition

**Van Gogh Studio** is an interactive, generative art application that transforms static images into living, breathing particle simulations inspired by the impasto technique of Vincent van Gogh.

It combines **classic computer graphics algorithms** (Flow Fields) with **modern Generative AI** (Google Gemini) to create a unique digital art experience.

🔗 **Live Demo:** [https://Fatmanurkntr.github.io/van-gogh-studio/](https://Fatmanurkntr.github.io/van-gogh-studio/)

![Project Screenshot](https://via.placeholder.com/800x450?text=Van+Gogh+Studio+Preview)

---

## ✨ Key Features (What You Can Do)

### 1. 🖌️ Interactive Painting & Animation
* **Living Canvas:** The artwork is not a static image; it flows like a liquid based on the visual data.
* **Magic Brush:** Use your mouse/touch to "paint" movement. Wherever you touch, the painting comes to life and flows in the direction of your stroke.
* **Freeze & Flow:** Control the simulation state. Freeze the painting to examine details, or let it flow endlessly.

### 2. 🧠 Hybrid AI Capabilities
* **Smart Filters (No API Required):** Type words like *"Fire"*, *"Ocean"*, *"Matrix"*, or *"Forest"* to instantly change the color palette using a local keyword detection algorithm.
* **Gemini AI Critic:** Ask the built-in AI to analyze your current artwork and write a poetic critique or description.
* **Generative Art (Pro):** Use Google's **Gemini 2.5 Flash** or **Imagen** models to generate brand new SVG-based base images from text prompts (e.g., *"A cyberpunk city in Van Gogh style"*).

### 3. ⏪ Time Travel (Robust Undo System)
* **Step-by-Step Undo:** Made a mistake with the brush? Or didn't like the last filter? The advanced Undo system lets you revert changes one by one.
* **Snapshot Memory:** The system remembers the exact position of every single particle, ensuring a smooth and glitch-free rewind experience.

### 4. 🛠️ Customization Studio
* **Fine-Tuning:** Adjust particle density (pixel size), flow speed, and brush radius in real-time.
* **Export:** Download your masterpiece as a high-resolution PNG file.

---

## 🔧 How It Works (The Engineering)

This project is built with **Vanilla JavaScript** and **HTML5 Canvas API**, with zero external dependencies for the core engine. Here is a breakdown of the technical implementation:

### 1. The Flow Field Algorithm
The core of the simulation is a "Flow Field." We analyze the source image's pixel data:
* **Luminance Calculation:** We calculate the brightness of every pixel using the formula `0.299*R + 0.587*G + 0.114*B`.
* **Vector Mapping:** Brighter pixels create flow vectors pointing in specific angles (0 to 360 degrees).
* **Particle Physics:** Thousands of particles (`Canvas 2D` entities) are spawned. They follow these invisible vectors, creating the illusion of brush strokes moving with the "wind" of the image.

### 2. The "Smart Undo" Architecture
Implementing `Undo` in a physics simulation is challenging because particles are constantly moving.
* **Snapshot Strategy:** We implemented a "Snapshot before Mutation" pattern. Before any user action (Brush stroke start, Filter apply), the system takes a deep snapshot of the state.
* **Data Stored:**
    * `FlowField[]`: The entire grid of wind directions.
    * `Particles[{x, y, vx, vy, color}]`: The exact position, velocity, and color of every single particle (up to 5,000 entities).
* **Teleportation:** When `Undo` is triggered, particles don't just reverse direction; they are instantly "teleported" back to their saved coordinates to ensure 100% accuracy.

### 3. Hybrid AI Integration
We use a dual approach for AI features:
* **Local Logic (Free):** For color filters, we use a local hashing algorithm that converts text input into consistent color palettes without needing an internet connection.
* **Remote API (Google Gemini):** For complex tasks (Image Generation & Analysis), we make asynchronous calls to the Google Gemini API. The response is parsed (e.g., extracting SVG code from text) and rendered onto the canvas dynamically.

---

## 🚀 Tech Stack

* **Frontend:** HTML5, CSS3 (Glassmorphism UI), JavaScript (ES6+)
* **Graphics:** HTML5 Canvas API (`CanvasRenderingContext2D`)
* **AI:** Google Gemini API (Flash 2.5 & Imagen Models)
* **Hosting:** GitHub Pages

---

## 📦 Installation & Setup

1.  Clone the repository:
    ```bash
    git clone [https://github.com/Fatmanurkntr/van-gogh-studio.git](https://github.com/Fatmanurkntr/van-gogh-studio.git)
    ```
2.  Open `index.html` in any modern web browser.
3.  (Optional) To use the **Pro AI Features**, click the `[API SETTINGS]` button in the UI and paste your Google Gemini API Key.

---

## 👨‍💻 Author

Created by **Fatımanur Kantar**.
*A blend of Computer Engineering & Digital Art.*
