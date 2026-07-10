# BloodStrike Android External Overlay

A high-performance external overlay for **BloodStrike (NetEase)** on Android. This project utilizes the **Vulkan API** for smooth rendering and **Dear ImGui** for a clean, interactive user interface.

## 📋 Project Information
- **Target Game:** BloodStrike (com.netease.newspike)
- **Rendering Engine:** Vulkan API
- **UI Framework:** Dear ImGui
- **Programming Language:** C++20
- **Architecture:** External Native Surface Overlay

## ✨ Key Features

### 1. Visuals (ESP - Extra Sensory Perception)
*   **Player ESP:**
    *   **Skeleton/Bone:** Real-time bone tracking (Shoulders, Elbows, Knees, etc.).
    *   **Box ESP:** 2D/3D bounding boxes around enemies.
    *   **Snaplines:** Directional lines pointing towards targets.
    *   **Health & Info:** Displays enemy health bar, distance, and team ID.
*   **Loot & Item ESP:**
    *   **Supply Boxes:** Detection for Low, Medium, High, and Special Supply Boxes.
    *   **Equipment Levels:** Identification of Helmets, Armor, and Backpacks (Tier 1 to Tier 6).
    *   **Medkits & Weapons:** Specific icons/text for different medical supplies and weapon crates.

### 2. Aimbot System
*   **Auto-Aim:** Automatically locks onto targets.
*   **Target Selection:** Adjustable aim parts (Head, Chest, or Pelvis).
*   **Trigger Modes:** 
    *   Fire: Active while shooting.
    *   ADS: Active while aiming down sights.
    *   Always: Constant lock-on.
*   **Field of View (FOV):** Customizable circle to define the aimbot's active range.

### 3. System & UI
*   **Vulkan Rendering:** Optimized for low latency and high FPS.
*   **FPS Controller:** Limit frames (30, 60, 90, 120) to save battery and reduce heat.
*   **Touch Bypass:** Advanced touch event handling for seamless menu interaction.
*   **Hotkeys:** 
    *   **Volume Up:** Show Menu / Enable Floating Ball.
    *   **Volume Down:** Hide Menu.

## 🛠️ Build Requirements
- **Android NDK:** r21 or newer recommended.
- **CMake:** 3.10.2+
- **Root Access:** Required for reading the game process memory and injecting touch events.

## 🚀 How to Use
1. Compile the source using Android Studio or the provided JNI build scripts.
2. Push the compiled executable (e.g., `Starcool.sh`) to your device via ADB.
3. Grant root permissions and "Display over other apps" permission.
4. Launch **BloodStrike**.
5. Run the executable via terminal. The overlay will appear automatically.

## ⚠️ Disclaimer
This project is for **educational and research purposes only**. Using third-party tools in online games violates their Terms of Service and can result in your account being **permanently banned**. The developers of this project are not responsible for any misuse or damages.
