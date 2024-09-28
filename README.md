# Queue Management System with Advanced Object Detection and Force Analysis

## Introduction
This project presents a solution for optimizing queue management by integrating object detection models (YOLOv7, YOLOv8, and YOLOv10), regression analysis, statistical methods, and force-based outlier detection. The system is designed to enhance accuracy and real-time performance by detecting individual body points, calculating optimal paths, and visualizing deviations using saliency maps and color coding.

## Features
1. **Object Detection**: Uses YOLO models (YOLOv7, YOLOv8, YOLOv10) to detect individuals in a queue and identify key body points.
2. **Regression Analysis**: Employs linear and polynomial regression to find the optimal line individuals should follow.
3. **Outlier Detection**: Identifies individuals deviating from the optimal path using a 95% confidence interval and the tension in spring concept.
4. **Visualization**: Generates color-coded saliency maps representing force magnitudes acting on individuals in the queue.

## Models and Techniques
### 1. Object Detection Models
The system utilizes the following YOLO models:
- **YOLOv7**: Improved model architecture for higher accuracy.
- **YOLOv8**: Faster inference times with optimized network design.
- **YOLOv10**: The latest iteration with state-of-the-art techniques for real-time performance.

### 2. Regression Techniques
- **Linear Regression**: Used to model simple relationships between body point coordinates and the optimal path.
- **Polynomial Regression**: Extends linear regression to capture more complex, non-linear relationships.

### 3. Outlier Detection
- **95% Confidence Interval**: Statistical outliers are detected by comparing the body points to the optimal path within a confidence interval.
- **Physics-Based Detection**: The tension in spring concept, derived from Hooke's Law, is used to identify deviations in force between individuals.

### 4. Visualization
- **Saliency Maps**: Color-coded visualization of force magnitudes using a jet colormap (blue for low, red for high).
