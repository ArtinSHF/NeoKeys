# NeoKeys 🎹

NeoKeys is a web-based MIDI piano trainer and interactive musical workstation featuring falling notes, an inverted arcade Freeplay mode, full session recording, hardware MIDI output pass-through, and a responsive, mobile-friendly interface.

The project is inspired by desktop piano learning applications, built as a personal experiment to learn advanced frontend engineering, browser-based hardware communication, audio synthesis, dynamic canvas rendering, and complex game-state architecture.

## 🌐 Live Website

NeoKeys runs online using Vercel.

**Live site:** https://neo-keys.vercel.app

## 🎮 About the Project

NeoKeys renders a responsive 88-key piano at the bottom of the screen with a high-performance cyber-neon visualizer grid.

The application is a full duplex audio tool: it captures incoming physical or wireless MIDI keyboard inputs via the Web MIDI API and can route auto-play data back out into a physical piano's sound engine.

It supports local MIDI file loading, a built-in track library, real-time note name translation, standalone session recording, and downloadable MIDI exports.

---

## 🚀 Features

### Core Visualizer & Rendering Engine

* **88-Key Cyber Piano Bed:** High-fidelity virtual piano with real-time key highlighting.
* **Bi-Directional Waterfall Animations:**

  * **Standard Mode:** Notes cascade downward toward the hitline.
  * **Freeplay Mode:** Notes shoot upwards from the piano bed and stop on key release.
* **Responsive Font Scaling:** Note labels automatically resize to remain readable on mobile landscape screens.
* **Timeline Scrubbing:** A styled neon range slider lets users jump to any part of a song instantly.

### Advanced Audio & Hardware Systems

* **Multi-Instrument Sound Selector:** Swap between 4 custom Tone.js audio engines:

  * Grand Piano
  * Cyber Synth
  * 8-Bit Arcade
  * Ambient Strings
* **Hardware MIDI Output Pass-Through:** Sends MIDI Note On/Off commands back to a digital keyboard, allowing auto-playing tracks to play through the keyboard's physical speakers.
* **Hardware Synth Muter:** A toggle to silence browser audio when using a real piano's internal sound engine.

### Gamified Practice & Learning Tools

* **Built-In Tracks Menu:** Includes a built-in selection menu with pre-loaded classical pieces such as:

  * Beethoven's Moonlight Sonata
  * Für Elise
  * Clair de Lune
* **Intelligent Practice Mode:** The waterfall pauses automatically until the correct key is pressed.
* **Fast-Playing Patch:** Uses active key scanning to prevent lock-ups during rapid runs, trills, and arpeggios.
* **Smart Hand-Splitting Heuristics:** Detects left/right hand tracks from MIDI channels or calculates a median pitch split.
* **Internationalization Toggle:** Switches note names between English notation and French solfège.
* **Gamified Scoring Engine:** Tracks player accuracy with timing-based scoring and penalties for wrong notes.
* **Dynamic Performance Review:** Shows an end-of-song review with score, wrong notes, and feedback.

### Custom Session Recording & Exporting

* **Freeplay Studio Recording:** Captures live MIDI input while in Freeplay mode, including note values, velocities, timestamps, and durations.
* **Instant Sandbox Playback:** Converts recordings into playable in-app tracks for instant review.
* **MIDI File Downloader:** Generates a downloadable `.mid` file from custom recordings using MidiWriterJS.

---

## 🛠 Tools & Technologies Used

* **HTML5:** Structure and Canvas API
* **CSS3:** Custom properties and neon cyber styling
* **JavaScript:** ES6+, async Web MIDI, and state machines
* **Web MIDI API:** MIDI input/output hardware routing
* **Tone.js:** Audio synthesis, polyphonic mapping, and samplers
* **MidiWriterJS:** MIDI file compiling and encoding
* **VS Code:** Development environment
* **Vercel:** Deployment
* **AI Assistance:** Planning, debugging, and optimization

---

## ▶️ How to Run Locally

This project runs completely inside a single file and can be opened using any local server environment.

Recommended method:

1. Open the project folder in VS Code.
2. Install the **Live Server** extension.
3. Right-click `index.html`.
4. Select **Open with Live Server**.

The site should open in your browser at:

```text
http://127.0.0.1:5500/index.html
```

---

## 🎹 MIDI Keyboard Support

NeoKeys uses the browser's native Web MIDI API.

For the interactive MIDI features to work properly:

* Use a Web MIDI compatible browser such as Google Chrome, Opera, or Microsoft Edge.
* Connect your digital piano using USB-MIDI or a wireless MIDI/Bluetooth adapter before launching the page.
* Grant MIDI permissions when prompted by your browser.
* To hear playback through your piano, make sure your keyboard's MIDI receive channels are active.
* Use the **Mute Web Audio Synth** toggle when you want audio to come from your physical keyboard instead of the browser.

---

## 📁 Project Structure

```text
neokeys/
│
├── index.html        # Main single-file app
├── README.md         # Repository documentation
└── screenshots/      # UI layout and feature screenshots
```

---

## 📌 Status

This is an actively maintained experimental portfolio project.

Updates are focused on expanding practice mechanics, improving audio latency, refining MIDI hardware support, and optimizing canvas performance across different devices.

---

## ⚠️ Note

NeoKeys is a standalone, independent web application.

It is a personal development and game-design music training experiment made for educational purposes and to showcase frontend, hardware API, and canvas-rendered audio programming skills.

NeoKeys is not affiliated with Synthesia or any other piano learning software.

---

## 🧠 What I Learned

While building NeoKeys, I gained hands-on experience with:

* **Monolithic State Management:** Managing audio, rendering loops, recording, and hardware states inside a single-file app.
* **Duplex Hardware I/O:** Using browser APIs to receive and send low-level MIDI messages.
* **Canvas Coordinate Mapping:** Building and adjusting real-time visual math for different note directions and screen sizes.
* **Asynchronous Audio Systems:** Preventing audio clipping, lag, and interaction issues during playback and user input.
* **Defensive Algorithmic Engineering:** Solving timing problems caused by fast note sequences and timeline pauses.
* **Binary File Compilation:** Turning recorded user input into valid downloadable MIDI files directly in the browser.
