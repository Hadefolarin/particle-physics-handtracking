<div align="center">

# 🌌 Aether: Gesture-Controlled Physics Engine

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-red?style=for-the-badge&logo=opencv&logoColor=white)](https://opencv.org/)
[![MediaPipe](https://img.shields.io/badge/MediaPipe-Hand%20Tracking-teal?style=for-the-badge&logo=google&logoColor=white)](https://google.github.io/mediapipe/)
[![VPython](https://img.shields.io/badge/VPython-3D%20Rendering-orange?style=for-the-badge)](https://vpython.org/)

**A volumetric particle simulation that responds to human touch.**
<br>
Running on a custom-built physics engine powered by Computer Vision.

[View Demo](#-visual-demo) • [Installation](#-installation) • [How It Works](#-how-it-works)

---

</div>


## 🚀 Overview

**Aether** is an experimental project exploring the intersection of **Physics Simulations** and **Human-Computer Interaction (HCI)**. By leveraging Google's MediaPipe for hand tracking and VPython for WebGL rendering, this engine allows users to manipulate 1,200+ particles in a 3D space using natural hand gestures.

Unlike static simulations, Aether treats every particle as an individual physics entity with mass, velocity, friction, and attraction properties.

### ✨ Key Features
* **Volumetric Rendering:** Simulates 1,200+ individual particles with depth-based distribution.
* **Real-time Hand Tracking:** Latency-free interaction using MediaPipe's lightweight model.
* **Custom Physics Logic:**
    * *Interaction:* Particles react to hand velocity (Repulsion vs. Attraction).
    * *Stability:* "Hard-stop" friction logic to prevent jittering during inspection.
* **Lab Mode Control:** Full 3D camera control (Zoom/Pan/Rotate) for detailed analysis.

---

## 🛠️ Tech Stack

| Component | Technology | Description |
| :--- | :--- | :--- |
| **Core Logic** | `Python 3.9` | Main orchestration and physics calculations. |
| **Vision** | `MediaPipe` | Skeletal hand tracking and landmark extraction. |
| **Processing** | `OpenCV` | Frame capture and image preprocessing. |
| **Rendering** | `VPython` | WebGL-based 3D visualization in the browser. |

---

## 💻 Installation

### Prerequisites
Ensure you have Python 3.9 or newer installed.

### 1. Clone the Repository
```bash
git clone [https://github.com/DrajatAkbarr/particle-physics-handtracking.git](https://github.com/DrajatAkbarr/particle-physics-handtracking.git)
cd particle-physics-handtracking
### 2. Install Dependencies
```bash
pip install -r requirements.txt
### 3. Run the Engine
```bash
python main.py
