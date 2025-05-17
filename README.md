# 🤖 Graspify

**Graspify** is a Unity-based simulation tool that intelligently detects and analyzes optimal grasp points on 3D objects using mesh data — designed to identify the **most stable 2-point contact regions** for robotic manipulation or automated picking systems. It prioritizes grasp **stability** and **efficiency**, aiming to reduce the required force while maximizing object control.

This project was built during a 48-hour hackathon as a demonstration of how geometric reasoning and Unity's 3D engine can be combined to power smarter robotic simulations.

---

## 🚀 Try It Out

🎥 Watch the demo: [youtu.be](https://youtu.be)

---

## 💡 Inspiration

Robots often grip objects using brute force or trial-and-error methods. We wanted to explore a geometry-driven solution — one that could **precisely determine where a robotic claw should grip an object**, with **minimal force and maximum stability**. This is especially useful for robotic arms in manufacturing, logistics, or surgery where precision and efficiency matter.

---

## 🧠 What It Does

- 🧊 **3D Shape Classification** — Detects primitive shapes (cube, cylinder, sphere, etc.) based on mesh geometry.
- ✋ **Grasp Point Analysis** — Identifies two or more ideal grasp points that require minimal force and provide high stability.
- 📄 **JSON Output** — Exports data like shape, grasp points, and strategy to structured JSON for further processing or integration.
- 🧪 **Drag-and-Drop Interface** — Seamless Unity component lets users test any mesh model quickly inside the editor.

---

## 🔧 How We Built It

- Developed in **Unity** with **C#** scripts to handle mesh parsing, shape detection, and grasp point logic.
- Used **ProBuilder** to test and visualize custom mesh shapes.
- Created utility functions to compute **bounding boxes**, **radial distances**, **extrema**, and **midline symmetry** to guide grasp placement.
- Exported structured grasp data as **JSON** to simulate integration with external robotic systems.

---

## 🧗‍♂️ Challenges We Ran Into

- Accurately identifying shape types from arbitrary mesh data required balancing **speed vs. precision**.
- Mapping a consistent grasp strategy that applies across different shapes (cones, cubes, spheres) proved nontrivial.
- Unity’s coordinate systems and mesh normals required careful alignment to ensure grasp points were meaningful.
- Handling models exported from third-party sources (.STL, .FBX) required sanitizing and preprocessing data.

---

## 🏆 Accomplishments That We're Proud Of

- Built a working prototype in under 48 hours!
- Successfully classified various shapes and computed grasp points that **mimic real-world gripping logic**.
- Created a reusable Unity tool that can be adapted for robotics, simulation, and research environments.

---

## 📘 What We Learned

- Unity can be repurposed for more than just games — it’s a powerful tool for **interactive robotics simulations**.
- Geometric reasoning is a robust alternative to AI/ML for certain tasks like grasp planning.
- Writing editor tooling in Unity can drastically improve workflow and testing speed.

---

## 🔮 What’s Next for Graspify

- ✅ Add GUI for visualizing grasp vectors in real time
- 🤖 Simulate multi-finger grasp planning
- 🌐 Export for **WebGL** or integrate into a **ROS2** robotic simulation
- 🧠 Experiment with ML-based shape prediction for more complex or organic meshes

---

## 🛠️ Built With

- 🧰 Unity Engine
- 💬 C#
- 🎨 ProBuilder
- 📦 .STL / .FBX Mesh Format Support
- 📄 JSON Serialization
- 🌐 JavaScript (for potential WebGL display/visualizer)


