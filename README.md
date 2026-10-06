<img width="1332" height="643" alt="Screenshot 2026-10-06 at 08 36 41" src="https://github.com/user-attachments/assets/cf7db876-a5ce-4a96-86dd-4e214a26988a" />

# 📟 CYBER-DECK TELEMETRY CONSOLE // MK-VI

A zero-dependency, retro-futuristic mission control dashboard built with **Vanilla JavaScript (ES6+)**, **HTML5 Canvas API**, and **Tailwind CSS**. It emulates CRT phosphor monitors and real-time computational telemetry streams combining geometric transformations, wave synthesis, and signed distance field physics.

---

## ⚡ Live Demo
Experience the console directly in your browser:  
👉 **[Launch Cyber-Deck Console](https://inandenizturk.github.io/cyberdeck-telemetry/)**

---

## 🔬 Mathematical & Physical Foundations

### 1. 2D Torus Signed Distance Field (SDF) Visualizer
* **Analytical Field Formulation:** Implements a closed-form ring SDF defined by:
  $$d(p) = \vert{}\Vert{}p\Vert{} - R_{\text{major}}\vert{} - r_{\text{minor}}$$
* **Dynamic Isoline Sampling:** Evaluates concentric zero-crossing contours and surface intersections via animated radial probe rays ($d = 0$).

### 2. Polar Radar & Archimedean Spiral Morphing
* **Polar-to-Cartesian Mapping:** Real-time projection using:
  $$x = c_x + r \cdot \cos(\theta), \quad y = c_y + r \cdot \sin(\theta)$$
* **Topological Interpolation (Lerp):** Smooth dynamic blending between an Archimedean spiral ($r \propto \theta$) and discrete quantized orbital shells.
* **Vector Displacements:** Real-time mouse coordinate perturbations warping the polar field with harmonic modulations.

### 3. Fourier Signal & Oscilloscope Telemetry
* **Harmonic Synthesis:** Composite multi-frequency signal rendering:
  $$y(t) = \sum_{k} A_k \sin(\omega_k x \pm \phi_k t) + \eta$$
* **Amplitude Modulation (AM Envelope):** Carrier wave suppression modulated by a low-frequency envelope generator simulating interference beats.

---

## 🛠 Features

- **Triple Canvas Synchrony:** High-DPI scaled independent render engines running inside a unified 60 FPS animation loop.
- **CRT Phosphor Filter:** CSS scanline overlays, radial vignette gradients, and HUD bloom optics.
- **Dynamic Chromatic Engine:** Live hot-swappable color profiles (**Phosphor Green**, **Amber CRT**, **Deep Cyan**).
- **Interactive TTY Terminal:** Command dispatch parser (`help`, `scan`, `warp`, `color`, `status`) and simulated assembly/hex stream.

---

## 🚀 Quick Start (Local Run)

No `npm`, `node_modules`, or build pipeline required.

1. Clone the repository:
   ```bash
   git clone [https://github.com/inandenizturk/cyberdeck-telemetry.git](https://github.com/inandenizturk/cyberdeck-telemetry.git)
