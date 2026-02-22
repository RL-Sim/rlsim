# 🛣 Project Roadmap: Right-before-Left Simulator

This roadmap outlines the development phases for the Rust + WASM + SVG traffic simulator.

---

## 🟢 Phase 1: Core Engine (Current)

- [x] Initial Project Setup (Rust + WASM-Pack)
- [x] Basic SVG Rendering (Roads & Single Vehicle)
- [x] Basic Game Loop (`requestAnimationFrame` integration)
- [x] Static Coordinate Movement

## 🟡 Phase 2: Traffic Intelligence

- [ ] **Path Following:** Transition from simple X/Y movement to SVG Path navigation.
- [ ] **Yielding Logic:** Implement the "Priority to the Right" check in Rust.
- [ ] **Collision Buffer:** Create "Sensor Zones" in front of cars to prevent rear-end collisions.
- [ ] **Multi-Car Spawning:** Logic to generate cars from all four cardinal directions.

## 🟠 Phase 3: Simulator Features

- [ ] **Directional Indicators:** Visual "blinkers" when a car is turning.
- [ ] **Intersection Logic:** Handle left-turn yielding (yielding to oncoming traffic).
- [ ] **Variable Speed:** Different speeds for different vehicle types (Trucks vs. Cars).
- [ ] **Deadlock Resolution:** Logic to handle the "4-way stop" paradox where everyone has someone on their right.

## 🔴 Phase 4: UI & Analytics

- [ ] **Speed Control:** UI slider to speed up or slow down the simulation time.
- [ ] **Telemetry:** Dashboard showing "Wait Times" and "Intersection Efficiency."
- [ ] **Incident Logging:** Log and highlight when a priority rule is violated.
- [ ] **Responsive Design:** Ensure the SVG viewBox scales perfectly for mobile devices.

## 🟣 Phase 5: Deployment & Integration

- [ ] **GitHub Actions:** Automate `wasm-pack` builds on every push.
- [ ] **GitHub Pages:** Host the live simulation.
- [ ] **Interactive Mode:** Allow users to "click" to spawn cars and test specific scenarios.
