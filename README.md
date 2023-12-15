# Causal Discovery In Video via Deep Neural Networks

## Introduction
This project focuses on identifying Granger causal relationships in video data using Deep Neural Networks, with a specific emphasis on sports video analysis. Here is our [final report](https://github.com/QijunYang1/Causal-Discovery-In-Video-via-DNNs/blob/main/Final_Report_Causal_Discovery_In_Video_via_DNNs.pdf). To replicate our results, please see our [google drive](https://drive.google.com/drive/folders/1zSfbF2Nk4oLh6U5NoPAc0LnLpip3G1eV?usp=sharing) for more information.

## Methodology
The project is divided into three phases:
1. **Dataset Selection and Augmentation**: Utilizing the SportsMOT dataset ([paperswithcode.com/dataset/sportsmot](https://paperswithcode.com/dataset/sportsmot)) with additional augmentation for object obstruction scenarios.
2. **Video-Based Object Detection**: Implementation of algorithms like Faster R-CNN and YOLOv8.
3. **Granger Causality Estimation with Neural Networks**: Developing algorithms for causality estimation from video data.

## Implementation
- **Detection Algorithms**: Faster R-CNN for accuracy and YOLOv8 for speed.
- **Tracking Algorithm**: DeepSORT for object tracking.
- **Granger Causality Analysis**: Using cMLP and cLSTM models.

## Results
- Advanced object detection and tracking algorithms successfully implemented.
- Neural networks effectively used for causal analysis in sports videos.

## Discussion and Conclusion
- Showcases the effectiveness of advanced detection and tracking in sports scenarios.
- Demonstrates Granger causality models' potential in analyzing dynamic interactions.

## Contributions
- Haoran: YOLO-DeepSORT + Neural Causality Network.
- Elinor: YOLOv8 + Neural Causality Network.
- Qijun: Faster RCNN + Neural Causality Network.
