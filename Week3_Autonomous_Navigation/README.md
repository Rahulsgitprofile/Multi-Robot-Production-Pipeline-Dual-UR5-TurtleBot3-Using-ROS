
# Week 3 – Autonomous Navigation & Mapping

This stage implements the core navigation capabilities for a mobile robot, including map creation, localization, and path planning. You’ll use the ROS Navigation Stack—with GMapping for SLAM, AMCL for localization, and Move Base for planning—to enable a TurtleBot3 to explore, map, and autonomously navigate a known environment :contentReference[oaicite:0]{index=0}.

---

## 🛠️ Components Developed

1. **SLAM-Based Map Generation**  
   - Configured and launched `gmapping` to build a 2D occupancy grid map as the robot explores.  
   - Tuned laser scan parameters and odometry settings for accurate loop closure and map quality 

2. **Adaptive Monte Carlo Localization (AMCL)**  
   - Loaded the generated map using `map_server`.  
   - Set up the `amcl` node to estimate the robot’s pose on the pre-built map.  
   - Adjusted particle filter parameters (e.g., `min_particles`, `laser_z_hit`) for stable localization.

3. **Path Planning with Move Base**  
   - Integrated `move_base` with `amcl` to send the robot to arbitrary goal poses.

4. **Obstacle Avoidance & Recovery**  
   - Enabled dynamic obstacle detection via laser scans and costmap inflation.  
   

---
