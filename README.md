## Subproject 1: 3D Object Detection

We have implemented a 3D object detection system using the **RTM3** neural network, which has been calibrated on our custom dataset and deployed on the **Jetson Nano** platform. This system utilizes depth estimation information obtained from the **BTS** neural network to enhance 3D detection capabilities. 

### Implementation Details

1. **RTM3 Network**: The RTM3 neural network has been tailored for real-time 3D object detection. The output consists of the 3D coordinates of all detected objects in the image, along with their respective labels, which are saved in the `image.txt` file.

2. **Depth Estimation**: The BTS neural network employs ASPP as an encoder and local planar guidance layers as a decoder to achieve a full spatial resolution depth map. The depth estimation outputs are saved in images with filenames labeled as `Car1*1`, `Car2*2`, etc.

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
