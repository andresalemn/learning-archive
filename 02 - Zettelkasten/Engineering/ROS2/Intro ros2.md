---
title: Intro ros2
created: 14-11-2025 16:19
domain: "[[ros2]]"
type: tool
tags:
  - ros2
source_note: "[[ros2]]"
---
# ⚙️ Intro ros2

> **A concise, 1-2 sentence explanation of the concept in my own words.** This is for quick recall.

## ❓ Why is this important? (The Context)

*   What problem does this tool/concept/function solve?
*   Where is it most often used in my projects (ROS2, C++ applications, etc.)?

## 🧠 My Synthesized Understanding (The Core Explanation)

*This section is your own, robust explanation, broken down into clear headers. Use simple language and strong analogies.*

### How it Works / Core Mechanism

*   *Analogy:* Think of it like a train-switch in a rail yard...
*   *Key steps:* 
    1.  ...
    2.  ...

### Examples (To Cement Understanding)

*   Link to a code block in a dedicated examples file: 
*   Link to a note detailing a relevant project: 

## 🔗 Official & External Resources

*   **Official Docs Link Note:** `[[{{tool_name}} Documentation Links]]`
*   **Deep Dive:** [Article/Paper for advanced reading](https://example.com)

---
%% REMINDER: This note must only contain synthesized understanding. Official documentation is stored in the 04-Resources/ link note above. %%

**Conceptos asociados a ROS2**

- **Espacio de trabajo:** Es simplemente un directorio con una estructura particular. Permite a los desarrolladores agrupar, construir y gestionar paquetes de software de manera eficiente.
  - Suele estar vacío al inicio de un proyecto, a excepción de src.
  - Normalmente contienen un subdirectorio fuente (src).
- **Colcon:** Es una herramienta que permite realizar construcciones fuera del directorio de origen, mejorando la organización y facilitando la gestión de las dependencias y los paquetes.
  - Al construir con Colcon, se crean subdirectorios al mismo nivel que src.

**Subdirectorios de un Workspace con Colcon**
- **src (source):** Ubicación del código fuente de los paquetes de ROS.
- **build:** El directorio de construcción será donde se almacenen los archivos intermedios. Para cada paquete se creará una subcarpeta en la que, por ejemplo, se invocará a CMake.
- **install:** El directorio de instalación es donde se instalará cada paquete. Por defecto, cada paquete se instalará en un subdirectorio separado.
- **log:** El directorio log contiene información sobre cada invocación de Colcon o información de registro.
![[ros2_ws structure.png|398x200]]
- **Instrucciones dentro de install**
  - local_setup.bash ---\> It will source that workspace, which we can call an overlay.
  - setup.bash -----------\> It will source this workspace, here, plus the underlay workspace, which is the global. En el curso se utilizará más esta segunda instrucción.

- **Paquetes:** Ayudan a separar el código en bloque reutilizables
- Paquetes de Python
  - setup.cfg ---\> Indica en cuál (¿dónde?) dirección se instalarán los nodos.
  - setup.py ----\> Los nodos o scripts que se instalarán.
- Paquetes de C++

- **Librerías de ROS2**
  - **DDS** (Data Distribution Service). It handles all the communications in the applications. It's basically the lowest ROS2 client library you can use. Bridge to the ROS2 middleware. We don't use it directly.
  - **RCL** (ROS Client Library): Librería pura en C. Contains all the core functionalities.
  - **rclcpp:** Provides a binding for RCL functionalities into C++.
  - **rclpy:** Provides a binding for RCL functionalities into Python.
