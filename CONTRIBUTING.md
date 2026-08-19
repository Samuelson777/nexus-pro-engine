# Contributing to Nexus Pro Engine V2

Thank you for your interest in contributing! Whether you are fixing bugs in the JavaScript switcher engine, improving the dark UI, or helping optimize the video animation pipeline, your contributions are welcome.

## 🚀 How to Get Started

1. **Fork the Repository:** Create your own copy of the project by clicking the Fork button at the top right of this page.
2. **Clone Your Fork:**
   ```bash
   git clone [https://github.com/Samuelson777/nexus-pro-engine.git](https://github.com/Samuelson777/nexus-pro-engine.git)

3. **Branching Strategy:** Create a descriptive branch for your work:
```bash
git checkout -b feature/synchronized-video-playback
# or
git checkout -b fix/tbar-drag-glitch

```



## 🛠️ Development Guidelines

### 1. Front-End Architecture (`index.html`)

* **ES6 `NexusEngine` Class:** Maintain the modular structure of the core switcher class. Ensure state changes (such as PGM/PST swaps or tally state updates) route cleanly through engine methods.
* **Styling:** Use **Tailwind CSS** utility classes where possible. Custom styles (such as glassmorphism, T-Bar range inputs, or overlay transitions) belong in the standard `<style>` block.
* **Canvas Rendering:** Keep render loops inside `requestAnimationFrame` lightweight to maintain a consistent 60fps execution.

### 2. Animation & Media Pipelines

* When contributing media assets or pre-rendered WebM overlays, preserve an aspect ratio of **16:9 (1280x720 base resolution)**.
* Ensure dynamic graphic assets maintain transparent alpha channels for Downstream Keyer (DSK) compatibility.

## 📋 Submitting Pull Requests (PRs)

1. Ensure your code runs cleanly without console errors or broken hotkeys (`1-4`, `Space`, `Enter`, `D`).
2. Commit your changes with clear, concise messages:
```bash
git commit -m "feat: add audio spatialization to PST/PGM channels"

```


3. Push your branch to GitHub and open a **Pull Request** against the `main` branch.
4. Provide a short description in your PR explaining what was changed, added, or fixed.

## 💬 Questions & Feedback

If you encounter a bug or have an idea for a feature enhancement, please open an **Issue** on GitHub before submitting a PR so we can discuss the approach.
