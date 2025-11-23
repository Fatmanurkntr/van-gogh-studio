# van-gogh-studio
An interactive generative art engine that brings Van Gogh's style to life using flow fields and particle simulations. Powered by Gemini AI
# 🎨 Van Gogh Studio - Interactive Generative Art

**Van Gogh Studio** is an interactive web application that transforms static images into living, breathing particle simulations inspired by the impasto technique of Vincent van Gogh. 

It uses **Flow Field algorithms** to simulate fluid movement and integrates **Google Gemini AI** to generate custom artistic assets on the fly.

🔗 **Live Demo:** [Buraya GitHub Pages Linkini Yapıştır]

![Project Screenshot](https://via.placeholder.com/800x450?text=App+Screenshot+Here)
*(Screenshots of the interface recommended here)*

## ✨ Key Features

* **🌊 Interactive Flow Fields:** The image is not static; it flows like a liquid. Users can use a "Brush" tool to manually direct the flow of particles, creating a personalized version of the artwork.
* **🧠 AI-Powered Generation:** Integrated with **Google Gemini 2.5 Flash API** to convert text prompts into SVG vector art, which is then particle-ized instantly.
* **🎨 Smart Style Filters:** A custom keyword detection engine that changes the color palette based on user input (e.g., "Fire", "Neon", "Ocean") without needing an API key.
* **⏪ Time Travel (Undo):** A robust undo system that snaps particles back to their previous states instantly.
* **📸 Snapshot:** Users can download their created masterpieces as high-quality PNG files.
* **⚡ High Performance:** Built with optimized Vanilla JavaScript and HTML5 Canvas API, capable of rendering thousands of particles at 60 FPS.

## 🛠️ Tech Stack

* **Core:** HTML5, CSS3 (Modern Glassmorphism UI)
* **Logic:** Vanilla JavaScript (ES6+)
* **Rendering:** HTML5 Canvas API (`2d context`)
* **AI Integration:** Google Gemini API (Flash Model)
* **No external libraries used.** (Zero dependencies)

## 🚀 How to Use

1.  **Enter the Studio:** Click start to load the default "Starry Night" simulation.
2.  **Interact:** * **View Mode:** Move your mouse to push particles gently.
    * **Brush Mode:** Click and drag to paint new flow directions.
3.  **Customize:** Use the sliders to adjust particle density, speed, and brush size.
4.  **AI & Filters:** Type "Fire" in the filter box for instant style changes, or use the AI panel to generate new images from text.

## 👨‍💻 Development

This project explores the intersection of **Computer Engineering** and **Digital Art**. It demonstrates proficiency in:
* Vector mathematics and physics simulations.
* Image processing (pixel manipulation).
* API integration and asynchronous programming.
* State management (Undo/Redo logic).

---
*Created by [Fatımanur Kantar]*
