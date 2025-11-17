---
title: Intro ros2
created: 14-11-2025 16:19
domain: "[[ROS2]]"
type: tool
tags:
  - ros2
source_note: "[[ROS2]]"
---
# ⚙️ Intro ros2

ROS2 is a framework (middleware) that helps different parts of a robot communicate with each other. It provides tools, message types, and a communication system so sensors, motors, and algorithms can work together.  

## 🧠 Basic concepts related to ROS2

- **Espacio de trabajo:** Es simplemente un directorio con una estructura particular. Permite a los desarrolladores agrupar, construir y gestionar paquetes de software de manera eficiente.
  - Suele estar vacío al inicio de un proyecto, a excepción de src.
  - Normalmente contienen un subdirectorio fuente (src).
- **Colcon:** Es una herramienta que permite realizar construcciones fuera del directorio de origen, mejorando la organización y facilitando la gestión de las dependencias y los paquetes.
  - Al construir con Colcon, se crean subdirectorios al mismo nivel que src.
  - [Using `colcon` to build packages](https://docs.ros.org/en/humble/Tutorials/Beginner-Client-Libraries/Colcon-Tutorial.html#using-colcon-to-build-packages "Link to this heading")

**Subdirectorios de un Workspace con Colcon**
- **src (source):** Ubicación del código fuente de los paquetes de ROS.
- **build:** El directorio de construcción será donde se almacenen los archivos intermedios. Para cada paquete se creará una subcarpeta en la que, por ejemplo, se invocará a CMake.
- **install:** El directorio de instalación es donde se instalará cada paquete. Por defecto, cada paquete se instalará en un subdirectorio separado.
- **log:** El directorio log contiene información sobre cada invocación de Colcon o información de registro.
![[ros2_ws structure.png|398x200]]

- **Instrucciones dentro de install**
  - `local_setup.bash` ---\> It will source that workspace, which we can call an overlay.
  - `setup.bash` -----------\> It will source this workspace, here, plus the underlay workspace, which is the global. En el curso se utilizará más esta segunda instrucción.

- **Paquetes:** Ayudan a separar el código en bloque reutilizables
- Paquetes de Python
  - `setup.cfg` ---\> Indica en cuál (¿dónde?) dirección se instalarán los nodos.
  - `setup.py` ----\> Los nodos o scripts que se instalarán.
- Paquetes de C++

![[ros2arch2.png|400x342]]

- **Librerías de ROS2**
  - **DDS** (Data Distribution Service). It handles all the communications in the applications. It's basically the lowest ROS2 client library you can use. Bridge to the ROS2 middleware. We don't use it directly.
  - **RCL** (ROS Client Library): Librería pura en C. Contains all the core functionalities.
  - **rclcpp:** Provides a binding for RCL functionalities into C++.
  - **rclpy:** Provides a binding for RCL functionalities into Python.

![[ros2arch1.png|444x250]]

## 🔗 Official & External Resources

*   **Official Docs Link Note:** [[ROS2 Documentation Links]]

---