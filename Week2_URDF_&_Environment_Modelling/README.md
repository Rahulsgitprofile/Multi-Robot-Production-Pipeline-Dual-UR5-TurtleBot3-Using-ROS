# Week 2 – Robot Modeling & Environment Setup (URDF + Gazebo)

This stage focuses on building custom robot models and virtual environments to simulate realistic robotic interactions. Using URDF (Unified Robot Description Format), the robot’s physical structure, joints, sensors, and visuals are defined. These models are integrated with Gazebo for testing inside a simulated world. The setup forms the digital twin of the robot for future tasks like navigation, manipulation, and perception.

---

## 🛠️ Components Developed

- **URDF Robot Model (TurtleBot3-like)**  
  - Base link, wheels, caster, sensors modeled
  - Xacro-based modular design for reusability
- **Custom Gazebo World**  
  - Basic simulated environment with ground plane, walls, and boxes
- **RViz & Gazebo Integration**  
  - Launch files for simultaneous RViz and Gazebo visualization
  - Static and dynamic transforms set up
