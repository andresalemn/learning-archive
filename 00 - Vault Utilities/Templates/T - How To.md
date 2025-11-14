---
title: Procedure: {{title}}
created: {{date}} {{time}}
category:
tags:
related_concept:
---

# 🛠️ Procedure: {{title}}

## 🎯 Goal

*   **Successfully build and source a new C++ package in the ROS2 workspace.*

## ⚠️ Pre-requisites

*   You must be in the `src` directory of your `ros2_ws`.
*   You must have `colcon` and `ament_cmake` installed.

## 🚶 Steps

1.  **Create the package:**
    ```bash
    ros2 pkg create --build-type ament_cmake my_new_package --dependencies rclcpp std_msgs
    ```
2.  **Move back to workspace root:**
    ```bash
    cd ..
    ```
3.  **Build the workspace:**
    ```bash
    colcon build --packages-select my_new_package
    ```
4.  **Source the setup file:**
    ```bash
    source install/setup.bash
    ```

## 🧠 Why This Works (Link to Understanding)

*   The `colcon build` command is explained in the [[]] note.
*   The `source` command is required to update the shell environment's path variables, which is detailed in the [[]] note.