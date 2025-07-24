# 🚀 Definitive Music Visualizer & Player

![Definitive Music Visualizer & Player](https://placehold.co/1200x600/0c0a09/4f46e5?text=Live+Music+Visualizer+in+Action&font=inter)

**A feature-rich, interactive audio visualizer and music player built with modern web technologies. This application transforms sound from any source—microphone, local files, or drag-and-drop—into stunning, customizable animations in real-time.**

### **[➡️ View Live Demo Here](https://your-github-username.github.io/your-repo-name/)** *Replace this link with your live project URL after deploying on GitHub Pages.*

---

## ✨ Key Features

This isn't just a visualizer; it's a complete audio experience.

* **🎧 Multiple Audio Sources**:
    * **Microphone Input**: Visualize your voice or any sound in your environment.
    * **File Upload**: Select one or more audio files from your device.
    * **Drag & Drop**: Simply drag your audio files onto the window to instantly create a playlist.

* **🎹 Full-Featured Music Player**:
    * **Complete Playback Controls**: Play, pause, seek, next, and previous track controls.
    * **Dynamic Playlist**: Automatically generated from your uploaded files.
    * **Volume & Progress Bars**: Fine-tune your listening experience.

* **🎨 12+ Advanced Visualizers**:
    * A massive library of both **2D and 3D** visual themes, from flowing auroras to pulsing cityscapes.
    * **Interactive Previews**: A custom-built dropdown menu shows animated previews of each style.

* **🎥 Interactive 3D Mode**:
    * **WEBGL Rendering**: Switch to a powerful 3D rendering engine for immersive visuals.
    * **Full Camera Control**: Use your mouse to **orbit, pan, and zoom** within the 3D scenes.

* **🔧 Deep Customization**:
    * **Curated Color Palettes**: Choose from multiple aesthetic color themes like "Neon Nights" or "Ocean Deep".
    * **Effects Control**: Adjust audio sensitivity and toggle dynamic backgrounds.
    * **Settings Persistence**: Your preferred theme, palette, and volume are automatically saved in your browser for your next visit.

* **🔴 GIF Recording & Sharing**:
    * Capture a 10-second GIF of your unique visual creation and share it anywhere.

* **🖥️ Modern UI/UX**:
    * **Sleek, Collapsible Interface**: A modern, blur-effect control panel that can be hidden for a fully immersive view.
    * **"Now Playing" Toasts**: Get notified when a new track begins.
    * **Fullscreen Mode**: Go completely borderless for maximum impact.

---

## 🔮 Visualizer Showcase

Here's a small preview of the diverse visual themes available:

| Aurora | Particle Sphere (3D) | Metropolis (3D) | Sunburst |
| :---: | :---: | :---: | :---: |
| <img src="https://i.imgur.com/8i1eJgC.gif" width="150"> | <img src="https://i.imgur.com/5bLz3jW.gif" width="150"> | <img src="https://i.imgur.com/k6t8v8x.gif" width="150"> | <img src="https://i.imgur.com/s4f3z2Y.gif" width="150"> |

---

## 🛠️ Tech Stack

This project is built from the ground up using a modern, frontend-focused tech stack.

* **Core Logic & Animation**: **p5.js** for 2D/3D drawing and animations.
* **Audio Processing**: **p5.sound** library, which acts as a friendly interface for the **Web Audio API** (used for FFT, amplitude analysis, etc.).
* **Styling**: **Tailwind CSS** for a responsive, utility-first design system.
* **GIF Generation**: **gif.js** for client-side GIF encoding.
* **Base**: HTML5, modern JavaScript (ES6+).

---

## 🚀 How to Run Locally

This project is completely self-contained and requires no build steps.

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git)
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd YOUR_REPOSITORY_NAME
    ```
3.  **Open the `index.html` file** in any modern web browser (Chrome, Firefox, Edge, Safari).

And you're ready to go!

---

## 💡 How It Works

* **Audio Analysis**: The application uses a **Fast Fourier Transform (FFT)** object to analyze the audio's frequency spectrum in real-time. This data (bass, mid, treble levels) and the overall amplitude are fed directly into the visualizer drawing functions.
* **Rendering Engine**: p5.js handles all the rendering. A toggle allows the user to switch the p5.js canvas between the default **2D renderer** and the more powerful **WEBGL renderer** for 3D scenes.
* **3D Interaction**: When in WEBGL mode, the `orbitControl()` function from p5.js is enabled, which automatically maps mouse movements to camera transformations (orbit, pan, zoom).
* **State Management**: All user settings and application states (current track, volume, selected theme, etc.) are managed in a central `state` object within the p5.js instance. Settings are persisted to `localStorage`.
