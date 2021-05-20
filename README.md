# Classifying Human Cell Proteins in Microscope Images

Developing an accurate and reliable model for automatic human cell protein classification can address a major bottleneck in biology research and accelerate the efforts to understand human diseases and find treatments. With a large amount of microscope images manually annotated by subject matter experts, we train a convolutional neural network based on EfficientNetB7 that can classify the cell proteins at the image level with an accuracy of .82 in F1. Furthermore, we provide empirical results of the variations in model performance based on different backbone models and hyperparameter settings. After segmenting individual cells in each image for cell-level classification, the task can be categorized as weak supervision because there are no cell-level gold-standard labels. In order to address this issue, we propose various methods of data analysis for detecting and denoising the anomalies in the dataset.

Due to the size of the dataset and access to accelerators, our experiments were conducted on Kaggle Notebook. Please take a look at the following notebooks for reference. 
* [Exploratory Data Analysis / EfficientNetB7 / Class Weights / Anomaly Detection](https://www.kaggle.com/kicksomeasphalt/classifying-cells)
* [Backbone Experiments / Hyperparameter Tuning](https://www.kaggle.com/scottbamford/hyperparameter-tuning#EfficentNetB7)

![Poster](https://github.com/hgjlee/cell_classification/blob/1a15b75944403a604c02ed599207597af3a7483b/ML%20-%20Final%20Project%20Poster%20.png?raw=true)
