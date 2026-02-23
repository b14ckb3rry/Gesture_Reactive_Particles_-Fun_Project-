# Gesture Reactive Particle Core ✋✨

An immersive, real-time **gesture-controlled particle system** built with **Three.js** and **MediaPipe Hands**, where hand tension dynamically reshapes thousands of particles into expressive 3D forms.

This project blends **computer vision**, **procedural geometry**, and **interactive graphics** to create a living particle sculpture that reacts to human motion.

---

Visit Live Website : [Click Here] (https://b14ckb3rry.github.io/Gesture_Reactive_Particles_-Fun_Project-/)
## 🚀 Features

- **Real-time Hand Tracking**
  - Powered by **MediaPipe Hands**
  - Tracks hand presence, motion, and tension using landmark distances

- **Gesture-Driven Particle Physics**
  - Open hand → particles expand and breathe
  - Closed hand (tension) → particles compress and jitter with energy
  - Smooth interpolation for organic motion

- **Procedural 3D Shapes**
  - Heart
  - Flower (Rose Curve)
  - Saturn (Planet + Rings)
  - Buddha (Multi-sphere silhouette)
  - Fireworks
  - Globe (Spherical distribution)

- **High-Performance Rendering**
  - ~8,000 GPU-accelerated particles
  - Additive blending with soft radial textures
  - Efficient BufferGeometry updates

- **Modern Glass-Morphism UI**
  - Shape switching
  - Live color customization
  - Camera & tracking status feedback

---

## 🧠 How It Works

### 1. Hand Tension Detection
Using MediaPipe landmarks:
- Distance between **wrist** and **index finger tip**
- Normalized to detect **open vs closed hand**
- Smoothed for stability

```text
Open Hand   → Low tension → Expansion
Closed Hand → High tension → Compression
