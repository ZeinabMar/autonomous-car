# lane_detection
### Implementation Details

1. **Keypoint Detection**: The system extracts relevant points from the input images to identify the locations of lane markings.
  
2. **Average Calculation**: An average of the detected points in 3D space is computed to represent the lane more accurately.

3. **Polynomial Fitting**: The identified points are processed using polynomial equations to accurately represent the road lanes.

4. **Visualization**: The final output, including the calculated average points and the polynomial representations, is visualized on the original image. The implementation and visualization process can be found in the `src/lane_model.ipynb` file.

