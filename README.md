﻿# BSplineEditor

### Project by Altamash Sheikh 
Completed for COMP 438/6381 at Concordia University

## Overview  
This B-Spline Editor project is an interactive B-Spline surface editor that allows users to manipulate control lattices and visualize tensor-product B-Spline surfaces in real time. Designed to explore geometric modeling and interactive 3D editing, this tool enables intuitive control over B-Spline patches with a minimal but functional UI, using the Ligigl library with C++.

## Features  
- **Click & Drag Control Points** – Modify the shape of the B-Spline surface by moving control points in 3D space.  
- **Toggle Display Modes** – Switch between control lattice, B-Spline surface, or both.  
- **Multiple Patches** – Add and switch between multiple B-Spline patches dynamically.  
- **Keyboard Shortcuts**:
  - `1` - Toggle control lattice visibility  
  - `2` - Toggle B-Spline surface visibility  
  - `3` - Add a new B-Spline patch  
  - `4` - Switch to the next patch  
  - `5` - Toggle visibility of the current patch  

**Note**: You can only edit one patch at a time. Switching patches is necessary to make different control lattices interactive.

---

## Under the Hood  
This project is built using **libigl (C++)**, leveraging its mesh processing capabilities. The architecture is split into:  
1. **Frontend (UI & Interaction)** – Handles user input, point selection, and rendering toggles.  
2. **Backend (Mesh Deformation)** – Computes and updates the B-Spline surface based on control point transformations.

---

## Installation & Usage  

### Requirements  
- C++ compiler  
- CMake  
- libigl  

### Build Instructions  
```sh
git clone https://github.com/altam-sh/BSplineEditor.git
cd libigl-example-project
cd build
rmdir /S
cmake ..
make
./BSplineEditor
```
From there, simply navigate to `\libigl-example-project\build\Debug` and run the `example.exe`

**Note**: If the build fails or the `cmake ..` command is causing issues, I've found success running the following command instead:
```sh
cmake -DCMAKE_POLICY_VERSION_MINIMUM="3.5" ..
```

## Why this project?
I built this to explore the world of geometric modeling and interactive editing. B-Splines are widely used in CAD and animation, and implementing a real-time editor gave me a deeper understanding of their structure and behavior.

# [Thank you for your interest!]
