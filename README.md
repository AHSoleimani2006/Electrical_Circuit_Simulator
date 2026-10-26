# Electrical Circuit Simulator

![C++](https://img.shields.io/badge/C++-20-blue.svg)
![GUI Framework](https://img.shields.io/badge/GUI-ImGui-green.svg)
![Build](https://img.shields.io/badge/Build-CMake-orange.svg)

<!-- GIF 1: Replace the link below with the path to your main interface GIF -->
![Main GUI Demo](assets/your_first_gif_name.gif)

## Overview
A lightweight, graphical analog electrical circuit simulator written entirely in C++. Inspired by the workflow of LTspice, this tool allows users to visually place components, wire them together, and simulate complex analog circuits. Developed as an Object-Oriented Programming project, it bridges software architecture with core electrical engineering principles.

## Key Features
- **Intuitive GUI & Fast Drafting:** Drag-and-drop component placement with visual wire routing. Features extensive keyboard shortcuts for rapid circuit building:
  - `R`: Resistor | `C`: Capacitor | `L`: Inductor | `D`: Diode
  - `V`: Voltage Source | `I`: Current Source
  - `G`: Ground | `W`: Wire
- **Component Library:** Includes passive components (R, C, L), DC, AC, Pulse, Delta, and Voltage-Controlled sources, as well as ideal diodes.
- **Sub-Circuits (Black Box):** Modular circuit design capabilities. After drawing a full circuit, you can encapsulate it into a "black box" sub-circuit and reuse it as a single component within other circuits.
- **Simulation Engine:** Extensive simulation options including DC operating point, transient voltage and current (for nodes and components), AC sweep, and phase sweep using Modified Nodal Analysis (MNA).
- **Project Management:** Full file saving and loading functionality to preserve your circuit workspaces.
- **Object-Oriented Design:** Modular architecture utilizing polymorphism, allowing for the seamless addition of new electronic components without altering the core simulation loop.

<!-- GIF 2 & 3: Replace the links below with the paths to your simulation and sub-circuit GIFs -->
### Demonstrations
![Simulation Graphs](assets/your_second_gif_name.gif)
![Sub-Circuit Feature](assets/your_third_gif_name.gif)

## Tech Stack
- **Language:** C++ (Standard 20)
- **GUI & Graphics:** Dear ImGui, GLFW, and GLEW
- **Plotting:** ImPlot (for rendering simulation graphs and sweeps)
- **Serialization:** Cereal (for save/load functionality)
- **Build System:** CMake
- **Math Library:** Custom matrix solver for Modified Nodal Analysis (MNA)

## Installation & Build Instructions
This project uses CMake, allowing it to be compiled easily from the terminal on any machine (Windows, Linux, or macOS).

```bash
# 1. Clone the repository
git clone [INSERT_YOUR_GITHUB_REPOSITORY_LINK_HERE]

# 2. Enter the project directory
cd [INSERT_YOUR_REPOSITORY_NAME_HERE]

# 3. Create a build directory and navigate into it
mkdir build
cd build

# 4. Generate the build files using CMake
cmake ..

# 5. Compile the project
cmake --build .

# 6. Run the executable 
# (If your executable is named OOP_Phase2_complete, run the following:)

# On Windows:
.\OOP_Phase2_complete.exe

# On Linux/macOS:
./OOP_Phase2_complete
