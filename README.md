# Vision Transformer Driven LiDAR Data Fusion for Enhanced Hyperspectral Image Classification
For any queries, please contact at srinadhml99@gmail.com

This work has been accepted to the 2024 IEEE India GeoScience and Remote Sensing Symposium. 
# Abstract
Multimodal fusion using Hyperspectral (HS) and Light Detection and Ranging (LiDAR) data has become a pivotal research focus in remote sensing and geospatial analysis. Vision Transformers (ViTs) have emerged as a transformative technology, offering sophisticated multimodal feature extraction and data fusion capabilities. This study investigates two previously unexplored multimodal fusion strategies for land cover classification tasks within the ViT architecture: self-attention-based and cross-attention-based fusion. These strategies aim to enhance the classification performance by utilizing shared and modality-specific parameters. Extensive experiments on benchmark datasets from the University of Houston demonstrate that the proposed cross-attention fusion method with ViTs outperforms the baseline ViT, previously proposed ViT-based fusion methods, and self-attention-based fusion approaches. Further, we demonstrate that late fusion allows for better learning of modality-specific features separately compared to early fusion.

# Results
Using Trento data
CLS Token | Overall Accuracy (OA) | Average Accuracy (AA) | KAPPA Score | Number of Parameters
--- | --- | --- | --- | ---
Random (HSI) | 95.45 | 92.85 | 93.91 | 262758
Channel (HSI+LiDAR) | **98.05** | **96.96** | **97.38** | 263526
Pixel (HSI+LiDAR) | 95.47 | 91.28 | 93.93 | 263526

# Observations
We introduce ViT-SA and ViT-CA, new fusion frameworks within ViT for integrating HSI and LiDAR data for land cover classification. Combined with shared and modality-specific parameters, cross-attention fusion significantly improves performance, outperforming other methods on the Houston dataset. Late fusion proves superior, allowing early layers to focus on unimodal processing. Models and code will be made available, with future work exploring band selection and adaptive attention mechanisms.

