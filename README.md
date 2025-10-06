# Robot-Simulation-and-Control-MATLAB-CoppeliaSim-

This project implements a complete SCARA and cartesian manipulators simulation and control system
developed in MATLAB App Designer, with integration to CoppeliaSim (V-REP)
through the remote API.

The project consists of two main MATLAB applications:

1. **APP_SCARA.m** – Simulates and controls a SCARA-type robot with:
   - Forward and inverse kinematics
   - Quadratic trajectory generation
   - 3D visualization
   - Remote control of the CoppeliaSim robot and gripper

2. **APP_Cartesiano.m** – Simulates a Cartesian robot manipulator with:
   - Linear direct and inverse kinematics
   - Position control and visualization
   - Trajectory plotting and motion profiles

Both apps can be launched independently or switch between each other with dedicated interface buttons.

---

## ⚙️ System Workflow

The full system executes a **collaborative trajectory** that demonstrates an industrial-style transport and handover process:

1. 🟢 **SCARA robot** picks up **five cubes** one by one.
2. 🟡 Each cube is placed into a **mobile cart** that moves across the simulated environment.
3. 🔵 The **Cartesian robot** receives the cubes from the cart.
4. 🟣 The Cartesian robot places the cubes at a designated drop-off zone on the opposite side.

This sequence showcases **object manipulation, robot coordination, and motion synchronization** in a shared environment.

## Features
- Forward and inverse kinematics (SCARA & Cartesian)
- Trajectory generation with quadratic velocity profiles
- Real-time visualization and animation
- Control of CoppeliaSim robot and gripper via remote API

## File structure
- `/matlab`: MATLAB code (App Designer files)
- `/coppeliasim_scene`: Scene and models
- `/docs`: Diagrams, screenshots, and explanations

## Requirements
- MATLAB R2021a or later
- Robotics Toolbox
- CoppeliaSim with Remote API enabled

## Run
1. Open MATLAB and add the `/matlab` folder to path.
2. Start CoppeliaSim and run the scene `simulation.ttt`.
3. In MATLAB, run:
   ```matlab
   app = APP_SCARA;

   > ⚠️ Academic Disclaimer  
> This project was developed as part of the  
> Robotics module at **Universidad Militar Nueva Granada (2017–2021)**.  
> The content is shared for educational and portfolio purposes only.  
> No proprietary or restricted university materials are included.
