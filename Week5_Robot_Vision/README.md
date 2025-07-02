
# Week 5 – Robot Vision Integration

This stage introduces perception capabilities to the robot by mounting an RGB camera and processing its image stream using ROS . The vision node detects specific objects in the scene and can communicate their positions to support manipulation tasks. This forms the foundation for vision-guided pick-and-place operations in robotic production setups.

---

## 🧩 Key Concepts Implemented

1. **Camera Sensor Simulation**
   - A simulated camera is mounted on the robot model in Gazebo.
   - The camera plugin streams live images over the `/camera/rgb/image_raw` topic.
   - Camera info and frame transforms are published for correct visualization and processing.

2. **Image Processing **
   - A Python node subscribes to the camera image topic.
   - It uses OpenCV to:
     - Convert BGR to HSV
     - Apply color thresholding
     - Detect contours and calculate centroids
     - Optionally draw bounding boxes
   - The result is published to a debug topic (`/camera/processed_image`) for visualization.

3. ** Position Publishing**
   - The node can also publish the (x, y) image coordinate of the object for use by manipulation pipelines.

4. **RViz Visualization**
   - Camera stream and object detection overlays are displayed in RViz.
   - TF tree confirms alignment of the camera frame with the robot base.
