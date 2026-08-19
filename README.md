# Nexus Pro Engine V2 & Interactive Animated Web Series

**By** : SAMUELSON G

This repository houses the **Nexus Pro Engine V2**, a browser-based, broadcast-grade switcher interface, alongside the production framework for a multi-camera animated web series. This project transforms passive viewers into active participants, allowing them to act as the live director of a fully animated episode by switching camera angles in real-time.

## 🎬 Project Overview

The project marries a high-fidelity 2D animation pipeline with a custom HTML/JS web application. Viewers are presented with a live broadcast desk where they can switch between wide shots, close-ups, and parallax environments while the animated narrative unfolds.

### The Animation Pipeline

The visual content is driven by a sophisticated production workflow:

* **Performance Capture & Animation:** Adobe Character Animator is used for multi-pass recording, capturing nuanced lip-sync and facial performances.
* **Compositing & Effects:** Premiere Pro and After Effects handle the parallax environments, dynamic lighting, and VFX overlays (like smoke).
* **Workflow:** Adobe Dynamic Link is leveraged to maintain a smooth, non-destructive production pipeline between character capture and final scene assembly, complete with Lumetri color grading.

## 🚀 Engine Features

The `NexusEngine` (ES6 Class Architecture) powers the front-end interactive experience:

* **Professional Switcher Logic:** Functioning Preview (PST) and Program (PGM) buses with T-Bar, hard cut, and 1-second auto-dissolve transitions.


* **Broadcast Graphics:** Downstream Keying (DSK) CSS overlays for lower-thirds and broadcast safe area margins (action/title safe).


* **Engineering Bay:** Simulated network packet loss/glitch generation and ISO recording functionality that exports the live PGM feed to a WebM/VP8 format.


* **Audio & Monitoring:** Master audio console featuring simulated ballistics for VU meters and real-time SMPTE timecode generation.


* **Dark UI Theme:** A customized Tailwind CSS interface optimized for broadcast environments with animated drawers and tally indicators.



## 🛠️ Installation & Usage

1. Clone the repository:
```bash
git clone https://github.com/Samuelson777/nexus-pro-engine.git

```


2. Navigate to the project directory and open the application:
* Simply open `index.html` in any modern web browser. No local server is strictly required for the core UI, though a local server (like Live Server) is recommended when fetching local video assets.




3. **Controls:**
* `1-4`: Select PST Bus.


* `Spacebar`: Hard Cut.


* `Enter`: Auto Transition.


* `D`: Toggle DSK (Downstream Keyer).





## 🎯 Conclusion

The development of this interactive web series represents a highly innovative approach to digital storytelling. By wrapping a high-fidelity animation pipeline inside a custom-built web application, the project successfully marries traditional broadcast control mechanics with interactive entertainment. The Nexus Pro Engine V2 acts as a robust proof-of-concept, proving that audiences can seamlessly live-switch between rendered character shots directly in the browser.

## 🔮 Future Enhancements

### Application & Interactivity

* **Synchronized Video Playback:** Upgrade the `NexusEngine`'s channel routing to handle synchronized playback of the rendered web series animation files, ensuring all camera angles remain locked in time during a transition.


* **"Director's Cut" Social Sharing:** Enhance the `MediaRecorder` API to allow viewers to effortlessly download and share their uniquely live-switched "edit" on social media.


* **Audio Spatialization:** Expand the `AudioContext` capabilities to automatically pan audio or adjust room reverb based on the active camera angle (e.g., direct sound for close-ups, reverb for wide shots).



### Production Pipeline

* **Web-Triggered Visual Effects:** Bridge the After Effects workflow with the web app by adding UI buttons that trigger pre-rendered VFX overlays (like transparent WebM elements) over the live program feed.
* **Multiplayer "Watch Party" Mode:** Implement WebSockets to allow multiple users to watch an episode together, with a designated "director" controlling the live stream for the entire lobby.
