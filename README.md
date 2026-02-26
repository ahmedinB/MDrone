
https://github.com/user-attachments/assets/aa4e865e-5990-47dd-b433-a8bb75be7c3c

# XMDrone
XMDrone: Indoor Monocular RGB Drone Localization Using Object Detection, Depth Estimation, and Multi-Layer Perceptron Models

Abstract— The challenge of precise indoor localization for unmanned aerial vehicles (UAVs) has traditionally depended on depth and stereo RGB cameras. Despite their utility, these cameras are not as widespread or versatile as monocular RGB cameras, which are found in common devices like security cameras. This paper presents Monocular RGB Drone Localization (MDrone), an innovative approach to Monocular RGB Drone Localization that harnesses the widespread availability and accessibility of monocular RGB cameras. MDrone integrates a trio of advanced machine learning techniques: YOLOv8 for object detection, ZoeDepth for metric depth estimation from single images, and a Multi-Layer Perceptron (MLP) for the refinement of initial estimations. This approach was validated through a ground truth dataset captured via Vicon motion capture system. MDrone achieves a 70.33% improvement in error reduction for drone localization and depth estimations values compared to the combined use of YOLOv8 and ZoeDepth alone. The significant enhancements in accuracy introduced by MDrone not only advocate for the potential of RGB based localization. They also promise to catalyze further explorations and applications in the realm of indoor drone localization technology.

https://ieeexplore.ieee.org/document/11268730

### Discrepancy Between Predicted Values Using YOLOv8 and ZoeDepth and the Actual Drone Position

| Error in mm | Close | Far | Average |
| :--- | :--- | :--- | :--- |
| **X** | 503.396 | 1806.568 | 1154.982 |
| **Y** | 687.075 | 2069.704 | 1378.349 |
| **Z** | 2883.568 | 3618.084 | 3250.836 |
| **D** | 1922.000 | 831.945 | 1376.972 |
| **Average** | 1499.001 | 2081.575 | 1790.288 |



### Discrepancy Between Predicted Values Using MLP and the Actual Drone Position

| Error in mm | Close | Far | Average |
| :--- | :--- | :--- | :--- |
| **X** | 691.962 | 338.876 | 515.419 |
| **Y** | 336.441 | 1059.281 | 697.860 |
| **Z** | 105.887 | 100.122 | 103.004 |
| **D** | 700.750 | 924.548 | 812.649 |
| **Average** | 458.760 | 605.706 | 532.233 |

---
Test evaluation are categorized into distant drone images ("Far") and nearer ("Close") images in the dataset.
