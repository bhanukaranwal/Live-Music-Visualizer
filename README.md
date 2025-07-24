# Live Music Visualizer

![Live Music Visualizer](https://placehold.co/800x400/10172a/ffffff?text=Add+a+Screenshot+or+GIF+of+your+Visualizer!)

A real-time, interactive music visualizer built with p5.js and the Web Audio API. This web application creates dynamic visuals that react to audio from a microphone, uploaded files, or even live MIDI instrument input.

**[Live Demo Link Here]** &lt;-- *Replace this with your GitHub Pages link after deploying!*

---

## ✨ Key Features

* **Multiple Audio Sources**: Visualize audio from your computer's **microphone** or by **uploading an audio file** (MP3, WAV, etc.).
* **Dynamic Visualizer Styles**: Switch between several unique visual modes on the fly:
    * **Particle Fountain**: Erupting particles that pulse with the music's volume.
    * **Waveform**: A classic oscilloscope-style representation of the audio wave.
    * **Frequency Bars**: A spectrum analyzer showing the intensity of different frequencies.
    * **Circular Ripples**: Expanding circles that react to the beat and bass.
* **Live MIDI Input**: Connect a MIDI keyboard or instrument to trigger colorful particle bursts with every note you play, mapping note pitch to position and color.
* **Interactive Controls**: A sleek, modern UI allows for real-time customization of the visualizer style, color, and audio sensitivity.
* **Responsive Design**: The visualizer and controls adapt to any screen size, from mobile to desktop.

---

## 🛠️ Tech Stack

* **Frontend**: HTML5, Tailwind CSS
* **Core Logic & Animation**: JavaScript (ES6+)
* **Graphics & Audio Processing**: [p5.js](https://p5js.org/) library with the p5.sound addon.
* **APIs**: Web Audio API, Web MIDI API

---

## 🚀 How to Run

This project is completely self-contained in a single `index.html` file.

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git)
    ```
2.  **Navigate to the directory:**
    ```bash
    cd YOUR_REPOSITORY_NAME
    ```
3.  **Open the `index.html` file** in any modern web browser (like Chrome, Firefox, or Edge).

That's it! No complex build steps or dependencies are required.

---

## 💡 How It Works

The application uses the **p5.js** library to create and manage the graphics on an HTML canvas. The **p5.sound** addon provides easy access to the **Web Audio API**, which is used to analyze the audio source in real-time.

* An **FFT (Fast Fourier Transform)** object analyzes the audio's frequency spectrum (for the bars and ripples).
* An **Amplitude** object measures the overall volume (for the particle fountain).
* The **Web MIDI API** listens for connected MIDI devices and triggers visual events when a "note on" message is received.

The UI is built with **Tailwind CSS** for rapid, responsive styling. All the logic is encapsulated within the `<script>` tag in the `index.html` file.
