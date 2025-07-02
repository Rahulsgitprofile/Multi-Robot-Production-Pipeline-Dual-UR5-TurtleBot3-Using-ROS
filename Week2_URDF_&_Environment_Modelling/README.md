# Week 2 – Robot & Environment Modeling (URDF + Gazebo)

In this phase, the focus is on creating a **digital twin** of both the robot and its work environment using URDF and Gazebo. You’ll define the robot’s kinematic structure, visuals, and collision properties, then build a factory-like world—including three robots and a conveyor belt—for downstream navigation, manipulation, and vision tasks :contentReference[oaicite:0]{index=0}.

---

## 🛠️ Components Developed

1. **URDF/Xacro Robot Model**  
   - Modular description with `<link>` and `<joint>` elements  
   - Parameterized using Xacro for reuse and clarity  
   - Includes base, wheels, sensors, and end‑effector definitions :contentReference[oaicite:1]{index=1}

2. **Factory Environment**  
   - Custom Gazebo world (`.world`) containing:  
     - Three robot spawns (e.g., TurtleBot3, two UR5 arms)  
     - Conveyor belt modeled as a moving surface  
     - Static objects (bins, walls) for a realistic production line

3. **Visualization Configurations**  
   - RViz display setup (.rviz) for inspecting the URDF frames and sensor outputs  
   - TF tree verification to ensure correct link transformations

4. **Launch & Configuration**  
   - `gazebo_sim.launch` to spawn the robot and environment together  
   - Controller configuration YAML for joint/velocity controllers under `config/`

---
