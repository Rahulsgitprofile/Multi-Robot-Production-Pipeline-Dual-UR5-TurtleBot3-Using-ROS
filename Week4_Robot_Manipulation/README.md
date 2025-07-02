
# Week 4 – Manipulation & Motion Planning

At this stage, we integrate a 6‑DOF robotic arm into our factory simulation and enable it to perform basic pick‑and‑place tasks. Using **MoveIt!**, you’ll configure the UR5 arm, plan and execute trajectories with the `move_group` node, and build a simple pick‑and‑place pipeline—laying the groundwork for the full production‑line demo in Week 6 :contentReference[oaicite:0]{index=0}.

---

## 🛠️ Components Developed

1. **MoveIt! Setup Assistant Configuration**  
   - Use the MoveIt! Setup Assistant to generate a self‐contained MoveIt package for the UR5 arm.  
   - Define kinematic chains, planning groups, end‑effector link, and virtual joints for the arm–base connection 

2. **Motion Planning with `move_group`**  
   - Leverage the `move_group` ROS node to compute collision‐free trajectories.  
   - Test planning, goal execution, and planning scene updates via RViz controls 

3. **Pick‑and‑Place Pipeline**  
   - Implement a Python script (`pick_place.py`) that:  
     1. Moves the arm to a “home” pose.  
     2. Plans and executes a trajectory to a pre‑grasp pose above the object.  
     3. Lowers, “grasps” (simulated via attaching a collision object), lifts, and transports the object.  
     4. Places and detaches the object at a target location.

4. **Factory Environment Update**  
   - Modified the Week 2 factory world to include the UR5 arm at its station.  
   - Adjusted bin positions to align with the arm’s reachability.

---
