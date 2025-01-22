# Vision Transformer Driven LiDAR Data Fusion for Enhanced Hyperspectral Image Classification
Vision Transformer Driven LiDAR Data Fusion for Enhanced Hyperspectral Image Classification

# Details
In this work, I studied the performance of a new Multimodal Fusion Transformer (MFT) for Remote Sensing (RS) Image Classification proposed recently. The link for the original MFT paper is here https://arxiv.org/pdf/2203.16952.pdf. 

Transformer-based models are widely used in several image-processing applications due to their promising performance over Convolutional Neural Networks (CNNs). However, there are certain challenges while adapting transformer models for the Hyperspectral Image (HSI) classification tasks. In RS image classification, using images from multiple sources and exploiting complementary information is getting more attention with the increased availability of multi-sensor data. However, considering the patch-level processing in the transformer models and the number of spectral bands in the HSI data or the fused data (HSI+other modalities), the number of model parameters is becoming a major issue. A new transformer-based architecture with novel attention and tokenization mechanisms is proposed in the MFT work to obtain complementary information from other modalities through an external CLS token. They showed that the CLS token extracted from other multimodal data generalises well compared to the random CLS token used in general transformer models.

In this work, I specifically studied the performance of the MFT model with varying the CLS token. Specifically, I used the CLS token as 'random', processed through 'channel' and 'pixel' tokenization methods. I considered the 'Trneto' dataset to validate the performance of the MFT model.
The performance is studied using Overall Accuracy (OA), Average Accuracy (AA) and KAPPA Scores. The training loss and confusion matrix are also studied. 

