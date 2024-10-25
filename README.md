# Autonomous Car Project

This project consists of multiple subprojects focused on developing systems for autonomous vehicles. The main areas of research include 3D object detection, lane detection, and depth estimation. Each subproject leverages advanced deep learning techniques to enhance the functionality and safety of autonomous cars.

## Subproject 1: 3D Object Detection

We have implemented a 3D object detection system using the **RTM3** neural network, which has been calibrated on our custom dataset and deployed on the **Jetson Nano** platform. This system utilizes depth estimation information obtained from the **BTS** neural network to enhance 3D detection capabilities. 

### Implementation Details

1. **RTM3 Network**: The RTM3 neural network has been tailored for real-time 3D object detection.
2. **Depth Estimation**: The BTS neural network provides depth information, which is crucial for accurately identifying and classifying objects in the environment.
3. **Deployment**: The entire system is deployed on the Jetson Nano, optimizing it for use in autonomous vehicles.

![3D Detection Result](result_3d_detection.png)

## Subproject 2: Lane Detection

The lane detection system is designed to identify and visualize road markings using keypoints extracted from images. This involves applying polynomial equations to the detected points to draw accurate lane lines on the road.

### Implementation Details

1. **Keypoint Detection**: The system extracts relevant points from the input images to identify the locations of lane markings.
2. **Polynomial Fitting**: The identified points are processed using polynomial equations to accurately represent the road lanes.
3. **Visualization**: The final output is a visual representation of the detected lanes overlaid on the original image.

![Lane Detection Result](result_lane_detection.png)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/YourUsername/Autonomous_Car_Project.git
