
# Week 6 – Multi-Robot Autonomous Factory Pipeline

This final stage integrates all previous capabilities into a comprehensive multi-robot simulation of an autonomous factory production line. Two UR5 robotic arms and a TurtleBot3 mobile robot work collaboratively in a Gazebo environment to pick up boxes from a conveyor belt, transport them between stations, and place them into final bins—demonstrating coordination between navigation, manipulation, and vision.

---

## 🛠️ Components Integrated

1. **Factory Environment Setup**  
   - Full Gazebo world with conveyor belt, bins, and multiple robot spawn points.  
   - Objects are automatically spawned on the conveyor for processing.

2. **Robot Coordination**  
   - TurtleBot3 navigates autonomously between stations using navigation stack.  
   - UR5 arms execute pick-and-place tasks using MoveIt!  
   - Vision system identifies boxes and provides target positions for manipulation.

3. **Task Orchestration**  
   - A high-level state machine or node ( FlexBE coordinates the workflow):  
     - Detect box on conveyor  
     - UR5 picks and places it onto TurtleBot3  
     - TurtleBot3 transports the box to the next station  
     - UR5 at next station picks from TurtleBot3 and places into bin

---
