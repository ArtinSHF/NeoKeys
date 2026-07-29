# 🕯️ Cozy Studio

---

Cozy Studio is a web-based lofi focus timer that combines a Pomodoro-style productivity system with ambient soundscapes, animated cozy atmospheres, a task list, and daily streaks.

The project is inspired by ambient "study with me" and lofi timer apps, built as a personal experiment in canvas animation, layered Web Audio playback, local persistence, and building a fully self-contained, single-file front-end tool.

## 🌐 Live Website

Cozy Studio runs online using Vercel.

**Live site:** *(add your Vercel URL here)*

## 🎮 About the Project

Cozy Studio renders a warm, glassmorphic focus timer at the center of the screen, backed by a full-screen animated canvas atmosphere.

The application is a full session companion: it tracks focus/break intervals with customizable durations, layers ambient soundscapes and lofi songs simultaneously, keeps a running daily streak of completed sessions, and manages a lightweight task list — all persisted locally so your setup is remembered on return visits.

---

## 🚀 Features

### Core Timer & Visual Engine

* **Circular Progress Ring Timer:** SVG ring animates smoothly around a large tabular-number clock display.
* **Focus / Break Presets:** Quick-select chips for Short Break, Long Break, Focus, and Deep Work sessions.
* **Fully Custom Durations:** Set custom minute values for any session type directly from Settings.
* **Auto-Start Breaks:** Optional toggle to automatically transition from a finished focus session into a break.
* **10 Animated Atmospheres:** Switch the full-screen canvas background between Particle Dust, Rain on Glass, Aurora Glow, Embers, Starry Night, Autumn Leaves, Bokeh Blur, Foggy Window, Sunbeams, and Snowfall.
* **Reduced-Motion Aware:** Respects the browser's `prefers-reduced-motion` setting.

### Ambient Sound & Music System

* **Dual-Layer Audio:** Play an ambient soundscape and a lofi song simultaneously for a layered cozy effect.
* **10 Ambient Soundscapes:** Includes real field recordings (Rain, Fireplace Crackle, Coffee Shop, Ocean Waves, Night Crickets, Wind Chimes, Quiet Library) alongside in-browser synthesized loops (Forest Birds, Vinyl Crackle, Stream Water) that never buffer or break.
* **10 Royalty-Free Lofi Tracks:** Streamed directly from the Internet Archive for uninterrupted background music.
* **Independent Volume Controls:** Separate volume sliders for ambience and songs, both on the main panel and in Settings.
* **Now-Playing Indicators:** Pulsing status dots show which layer is actively playing.

### Gamified Productivity Tools

* **Daily Streak Counter:** Tracks completed focus sessions for the current day, with a running best-day record.
* **Focus Task List:** Add, complete, and delete lightweight daily tasks with animated check-off states.
* **Rotating Cozy Notes:** A daily-rotating quote/affirmation widget with a manual "another note" refresh option.
* **Chime Alarm System:** Choose between Warm Bell, Soft Marimba, or Wind Chime alarm styles, with adjustable volume and a one-click test button.
* **Browser Notifications:** Requests permission to notify when a session completes.

### Personalization & Settings

* **Warm Lighting Intensity:** Adjustable ambient glow/vignette strength.
* **UI Glass Opacity:** Control how transparent or solid the glassmorphic cards appear.
* **Clock Font Style:** Switch between monospace and rounded clock typography.
* **Resume Last Sound:** Optionally auto-resume the last-played ambience on page load.
* **Persistent Preferences:** All settings, durations, streaks, and tasks are saved locally between sessions.

---

## 🛠 Tools & Technologies Used

* **HTML5:** Structure and Canvas API
* **CSS3:** Custom properties, glassmorphism, and warm cyber-cozy styling
* **JavaScript:** ES6+, Web Audio API, Canvas animation loops, and local persistence
* **Web Audio API:** Layered playback, synthesized ambient loops, and chime generation
* **Google Fonts:** Quicksand & DM Mono
* **Internet Archive:** Source for royalty-free ambient recordings and lofi tracks
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

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
| :--- | :--- |
| <kbd>Spacebar</kbd> | Start / Pause the timer |
| <kbd>R</kbd> | Reset the timer |

---

## 📁 Project Structure

```text
cozy-studio/
│
├── index.html        # Main single-file app
├── README.md         # Repository documentation
└── screenshots/      # UI layout and feature screenshots
```

---

## 📌 Status

This is an actively maintained experimental portfolio project.

Updates are focused on expanding ambient soundscapes, refining the animated atmospheres, and improving audio reliability across devices.

---

## ⚠️ Note

Cozy Studio is a standalone, independent web application.

It is a personal development and productivity-design experiment made for educational purposes and to showcase front-end animation, audio engineering, and interactive UI design skills.

Cozy Studio is not affiliated with any commercial focus-timer or "study with me" product.

---

## 🧠 What I Learned

While building Cozy Studio, I gained hands-on experience with:

* **Layered Web Audio Playback:** Mixing streamed recordings with in-browser synthesized loops without conflicts.
* **Canvas Atmosphere Rendering:** Building ten distinct animated background systems sharing one render loop.
* **State Persistence:** Saving timer durations, streaks, tasks, and appearance settings locally between sessions.
* **Session-Based Gamification:** Designing a streak and task system that reinforces focus habits.
* **Custom Theming Systems:** Building adjustable warmth, opacity, and font controls driven by CSS custom properties.