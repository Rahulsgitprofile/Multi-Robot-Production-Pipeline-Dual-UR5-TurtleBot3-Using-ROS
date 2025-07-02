# Week 1 – ROS Workspace Setup & Communication Nodes

This stage lays the groundwork for the robotics project by setting up the ROS development environment and implementing basic communication between nodes. It involves creating a workspace, defining custom packages, and building a publisher–subscriber system in both Python and C++. The structure serves as a minimal testbed for validating ROS messaging and tooling.

---

## 🛠️ Components Developed

- **Catkin Workspace**: Organized folder structure for managing ROS packages
- **Publisher–Subscriber Nodes**: Simple text-based message exchange using `std_msgs/String`
  - Implemented in both Python and C++
- **Turtlesim Interaction**: Used for visual validation of message publishing on `/turtle1/cmd_vel`
- **Launch File**: Single-click launch of the communication pipeline for faster iteration

---

## 📁 Directory Overview

```text
Week1/
├── install_ros.sh                   # Optional setup script for ROS Noetic
├── src/
│   └── basic_comms/
│       ├── package.xml
│       ├── CMakeLists.txt
│       ├── scripts/
│       │   ├── talker.py
│       │   └── listener.py
│       └── src/
│           ├── talker.cpp
│           └── listener.cpp
├── launch/
│   └── comms_test.launch
