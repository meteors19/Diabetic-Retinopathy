# Diabetic-Retinopathy
**Diabetic Retinopathy Detection using Deep Learning**

**Project Overview **


This project implements a custom Deep Learning pipeline to automate the detection of Diabetic Retinopathy (DR) from retinal fundus images. Utilizing the ResNet50 architecture and Transfer Learning, the model classifies eye scans into five distinct clinical stages: No DR, Mild, Moderate, Severe, and Proliferative.


**Technical Stack & Skills **

1. Deep Learning Framework: TensorFlow / Keras (Functional API).

2. Computer Vision: OpenCV (Image normalization, resizing, and interpolation).

3.Architecture: ResNet50 (Pre-trained on ImageNet) with custom GlobalAveragePooling2D and Dense layers.

4. Data Pipeline: Advanced use of ImageDataGenerator for real-time augmentation and efficient batch processing via flow_from_dataframe.

5. Performance Optimization: Implementation of EarlyStopping to prevent overfitting and class_weight balancing to handle medical data skew.

6.Evaluation Metrics: Scikit-Learn integration for Confusion Matrices, Precision, Recall, and F1-Scores to ensure clinical reliability.

**Key Features**

1. End-to-End Pipeline: From raw image processing (handling .png file indexing) to model deployment readiness.

2. Robust Pre-processing: Automated image rescaling and resizing to $224 \times 224$ pixels to satisfy ResNet requirements.
 
3. Evaluation Focus: Prioritizes Recall for advanced stages of DR, minimizing the risk of false negatives in medical diagnosis.
 
**Setup & Usage**

1. Environment: Requires Python 3.12+, TensorFlow, OpenCV, and Scikit-Learn.
 
2. Data: Ensure images are structured with a corresponding CSV containing id_code and diagnosis columns.
 
3.Execution: Run the Jupyter Notebook to train the model and generate performance heatmaps.
