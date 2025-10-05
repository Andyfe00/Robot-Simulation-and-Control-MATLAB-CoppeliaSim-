# Robot-Simulation-and-Control-MATLAB-CoppeliaSim-

This project implements a complete SCARA and cartesian manipulators simulation and control system
developed in MATLAB App Designer, with integration to CoppeliaSim (V-REP)
through the remote API.

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
- Robotics Toolbox (Peter Corke)
- CoppeliaSim with Remote API enabled

## Run
1. Open MATLAB and add the `/matlab` folder to path.
2. Start CoppeliaSim and run the scene `final.ttt`.
3. In MATLAB, run:
   ```matlab
   app = APP_SCARA;
