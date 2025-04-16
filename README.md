# Integrating Computer Vision in Educational Settings: A Case Study on Autonomous Vehicle Safety through Real-Time Road Surface Anomaly Detection

[Previous sections available in repository history]

## 3. Technical Foundations: Deep Learning and Real-Time Detection

### 3.1 Deep Learning Architectures: YOLOv12

Modern CV relies heavily on **Convolutional Neural Networks (CNNs)** and transformer architectures optimized for speed and accuracy. The UVU project utilizes **YOLOv12**, known for architectural refinements like enhanced feature pyramidal networks and anchor-free detection heads. These improvements reportedly yield **15% higher mean average precision (mAP)** over previous versions while maintaining real-time inference speeds [5, 3]. This balance makes YOLOv12 suitable for educational settings where students must manage trade-offs between model performance and computational constraints [6, 9].

### 3.2 Edge Computing for Real-Time Inference

**Edge computing** is critical, with inference performed locally on **NVIDIA Jetson modules** to ensure low-latency response times—essential for autonomous navigation [2, 5] (Figure 1). This approach aligns with industry trends towards decentralized AI processing, as seen in applications like Arctic AV localization systems functioning despite GPS denial [5]. Students gain direct experience with hardware-software co-design, optimizing techniques like model quantization and pruning to meet embedded system limitations [4, 10].

### 3.3 Data Pipeline Automation: RoboFlow

The project's data pipeline benefits significantly from **RoboFlow's auto-labeling** capabilities, which reportedly reduce manual annotation efforts by **40%** while preserving dataset quality [3]. This efficiency enables rapid iteration during model training, allowing students to systematically explore hyperparameter tuning and data augmentation strategies. Studies indicate that such automated workflows enhance learning outcomes in CV courses by freeing students to focus on higher-order design considerations rather than repetitive labeling tasks [4, 8].

## 4. Case Study: Real-Time Anomaly Detection and Autonomous RC Car Integration

UVU's two-phase project (summarized in Figure 2) demonstrates the scalability of CV education frameworks.

### 4.1 Phase 1: Road Anomaly Detection

Phase one focuses on **road anomaly detection** using a vehicle-mounted camera system. This system achieved **96% accuracy** in identifying potholes and cracks under varying illumination conditions [11, 3]. Students employed techniques like gradient thresholding and HLS color space transformations to isolate lane markings, integrating these with YOLOv12 detections for comprehensive road surface analysis [11, 10]. This multi-modal approach mirrors advanced driver assistance systems (ADAS) in commercial vehicles, providing authentic exposure to industry practices [2, 9].

### 4.2 Phase 2: Autonomous RC Car Navigation

Phase two transitions to **autonomous navigation** using a modified RC car platform, introducing challenges in sensor fusion and path planning. The system integrates **Lidar-based obstacle avoidance** with CV detections, requiring students to implement **Kalman filters** for robust state estimation [5, 10]. Simulating real-world scenarios (e.g., sudden obstacles, degraded lane markings) cultivates proficiency in designing fail-safe mechanisms—a critical competency for AV safety engineering [9, 12].

[... Content continues in next part due to length limits ...]