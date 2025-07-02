# Multi Robot Production Pipeline [Dual UR5, TurtleBot3] Using ROS
Multi-robot production-line in Gazebo, featuring two UR5 arms and a TurtleBot3 mobile robot, to autonomously pick up a box from a conveyor, transport it between stations, and place it into a final bin.


### 🗺️ TurtleBot3 SLAM Mapping

TurtleBot3 explores and maps an unknown environment using SLAM (Simultaneous Localization and Mapping). The 2D occupancy grid below was generated using LIDAR data in a simulated Gazebo world.

<p align="center">
  <img src="https://github.com/user-attachments/assets/5c3ca959-f20d-4f6c-aa58-b7c1d7bd37c0" alt="TurtleBot3 SLAM Mapping" width="500"/>
</p>

---


### 🤖 Robot Arm Manipulation with MoveIt

Using the MoveIt framework, a robotic arm (UR5) plans and executes precise pick-and-place motions. Below is a video showing trajectory planning and object manipulation in a simulated environment.

<p align="center">
  <a href="https://youtu.be/YOUR_VIDEO_LINK">
    <img src="https://github.com/user-attachments/assets/9c11ac93-fcc2-4f87-b570-c9769a0ae26f" alt="MoveIt Manipulation Video" width="500"/>
  </a>
</p>


---

### 🧭 Autonomous Navigation with TurtleBot3

The TurtleBot3 robot autonomously navigates between waypoints using the ROS Navigation Stack. The system handles localization, path planning, and real-time obstacle avoidance.

<p align="center">
  <a href="https://youtu.be/YOUR_VIDEO_LINK">
    <img src="https://github.com/user-attachments/assets/9b9f42f0-5af8-44a0-b319-4084aa1764d7" alt="Autonomous Navigation" width="500"/>
  </a>
</p>



---

### 🏭 Multi-Robot Factory Automation

The final capstone simulation presents a smart production line in Gazebo:  
- **Two UR5 arms** pick and place packages  
- A **TurtleBot3 mobile robot** transports them between stations  
- Entire sequence is autonomous, coordinated, and vision-aware

<p align="center">
  <a href="https://youtu.be/YOUR_VIDEO_LINK">
    <img src="https://github.com/user-attachments/assets/abafff73-52f3-4768-b1d2-ec6fea4bcf95" alt="Multi-Robot Factory Simulation" width="500"/>
  </a>
</p>

---



## 🚀 Project Overview
This repository contains a comprehensive robotics project built with ROS, demonstrating how to model, simulate, and control robots in virtual environments. Over six stages, it walks through:

1. **Environment Modeling & Robot Description**
2. **Autonomous Navigation**
3. **Robot Manipulation**
4. **Computer Vision Integration**
5. **Factory Automation**

Each stage is organized into its own folder, complete with code, launch files, and documentation.

## 🎯 Objectives
- Design and simulate robot models using URDF
- Build and configure virtual worlds in Gazebo
- Implement autonomous navigation with the ROS navigation stack
- Develop manipulation routines for robotic arms
- Integrate vision pipelines for detection and tracking
- Orchestrate multi‐robot factory processes

## 📂 Repository Structure
```text
├── Week1/                                # Environment setup & basic ROS concepts
├── Week2_URDF_& Environment_Modelling/   # URDF robot description & Gazebo worlds
├── Week3_Autonomous_Navigation/          # SLAM, path planning & navigation stack
├── Week4_Robot_Manipulation/             # MoveIt! setups and pick-and-place routines
├── Week5_Robot_Vision/                   # Vision tasks using OpenCV and ROS image topics
└── Week6_Autonomous Factory/             # Coordinated factory simulations with multiple agents
