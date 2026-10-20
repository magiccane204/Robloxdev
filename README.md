# ⚡ ApexEngine: Modular Luau Kinematic Character Controller & Network Bridge

## 💡 Why This Exists (The Justification)
Default Roblox character controllers are fine for standard games, but they lack the tight, responsive arcade feel required for high-velocity gameplay. **ApexEngine** was engineered from the ground up as a robust, object-oriented client-side controller framework.

It bridges the gap between smooth client prediction (sprinting, stamina consumption, fluid dashes, and double jumps) and secure server-authoritative event handling, serving as a comprehensive core template for modern action mechanics.

---

## ✨ Architectural Highlights

* **Object-Oriented Controller Paradigm (`Controller.new`):** Encapsulates individual character states, keeping physics, inputs, and attributes cleanly scoped per instance.
* **Dynamic Stamina & Resource Loop:** Features real-time delta-time (`dt`) calculations for draining and regenerating stamina during sprints and tactical dashes.
* **Kinematic Force & Velocity Management:** Utilizes custom `BodyVelocity` overrides and CFrame lerping to deliver snappy, predictable dash mechanics without fighting Roblox's default physics engine.
* **Unified Client-Server Remote Pipeline:** Automatically bootstraps `GameRemotes` to safely sync tool equipping, inventory states, and interaction events across the network boundary.

---

## 🛠️ Tech Stack

* **Language:** Luau (Roblox Lua)
* **Core Services:** `RunService`, `UserInputService`, `TweenService`, `ReplicatedStorage`, `Players`
* **Networking:** `RemoteEvent`, `RemoteFunction`

---

## 🚀 Initialization
Drop this script into a **LocalScript** under `StarterPlayer > StarterPlayerScripts`, and let the object-oriented chaos take the wheel.
