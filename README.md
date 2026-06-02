# NeoKeys 🎹

NeoKeys is a web-based MIDI piano trainer with falling notes, practice mode, MIDI input, and a clean mobile-friendly interface.

The project is inspired by piano learning apps with falling-note visualizations, but it is made as my own web-based experiment for learning frontend development, MIDI input, canvas rendering, and interactive music tools.

## 🌐 Live Website

NeoKeys runs online using Vercel.

Vercel link: https://neo-keys.vercel.app

## 🎮 About the Project

NeoKeys shows an 88-key piano at the bottom of the screen and falling notes that move toward the keys.

It supports loading local `.mid` files and can also react to physical or wireless MIDI keyboard input through the browser using the Web MIDI API.

## 🚀 Features

- 88-key piano visualizer
- Falling-note waterfall animation
- HTML5 Canvas rendering
- Local `.mid` file loading
- MIDI file parsing using `@tonejs/midi`
- Web MIDI API support for physical MIDI keyboards
- Key highlighting when MIDI notes are played
- Normal playback mode
- Practice mode / wait-for-note mode
- Left hand / right hand / both hands practice options
- Speed slider
- Mobile-friendly landscape UI
- Sound effects
- Deployed with Vercel

## 🛠 Tools & Technologies Used

- HTML
- CSS
- JavaScript
- HTML5 Canvas
- Web MIDI API
- Tone.js MIDI parser
- VS Code
- Vercel
- AI assistance

## ▶️ How to Run Locally

This project can be opened using a local server.

Recommended method:

1. Open the project folder in VS Code
2. Install the Live Server extension
3. Right-click `index.html`
4. Click **Open with Live Server**

The site should open in your browser at a local address like:

http://127.0.0.1:5500/index.html

## 🎹 MIDI Keyboard Support

NeoKeys uses the browser Web MIDI API.

For MIDI input to work:

- Use a browser that supports Web MIDI, such as Google Chrome
- Connect a MIDI keyboard or wireless MIDI device
- Allow MIDI permissions when the browser asks
- Load a `.mid` file or use the keyboard input features directly

## 📁 Project Structure

neokeys/
│
├── index.html
├── README.md
└── screenshots/

## 📌 Status

This is an experimental project and may still be improved.

Some features may behave differently depending on the browser, MIDI device, screen size, or loaded MIDI file.

## ⚠️ Note

NeoKeys is not affiliated with Synthesia or any other piano learning software.

It is a personal web development and game-style music training experiment made for learning and showcasing frontend, MIDI, and canvas programming skills.

## 🧠 What I Learned

While making this project, I practiced:

- Building a single-file web app
- Using HTML, CSS, and JavaScript together
- Canvas rendering
- Game loop logic
- MIDI file parsing
- Physical MIDI input handling
- Mobile UI design
- Practice mode / wait-state logic
- Deploying a web project with Vercel
- Using AI as a development helper
