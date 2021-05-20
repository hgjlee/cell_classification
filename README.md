# Classifying Human Cell Proteins in Microscope Images

Developing an accurate and reliable model for automatic human cell protein classification can address a major bottleneck in biology research and accelerate the efforts to understand human diseases and find treatments. With a large amount of microscope images manually annotated by subject matter experts, we train a convolutional neural network based on EfficientNetB7 that can classify the cell proteins at the image level with an accuracy of .82 in F1. Furthermore, we provide empirical results of the variations in model performance based on different backbone models and hyperparameter settings. After segmenting individual cells in each image for cell-level classification, the task can be categorized as weak supervision because there are no cell-level gold-standard labels. In order to address this issue, we propose various methods of data analysis for detecting and denoising the anomalies in the dataset.

Due to the size of the dataset and access to accelerators, our experiments were conducted on Kaggle Notebook. Please take a look at the following notebooks for reference. 
* [Exploratory Data Analysis / EfficientNetB7 / Class Weights / Anomaly Detection](https://www.kaggle.com/kicksomeasphalt/classifying-cells)
* [Backbone Experiments / Hyperparameter Tuning](https://www.kaggle.com/scottbamford/hyperparameter-tuning#EfficentNetB7)

### Backbone Experiments and Hyperparameter Tuning
![Experiment Results](https://github.com/hgjlee/cell_classification/blob/19eca8f578ca40ac959000d077ba046cfe91dd92/Table%20of%20Results.png?raw=true)

### Final Architecture
![Architecture](https://github.com/hgjlee/cell_classification/blob/e48871b26ade4a434233d529010ef5e32c7a6cd2/model_architecture.png)

### Performance Summary
![Architecture](https://github.com/hgjlee/cell_classification/blob/e48871b26ade4a434233d529010ef5e32c7a6cd2/classification_results.png)

### Color-based Anomaly Detection
![Histogram](https://github.com/hgjlee/cell_classification/blob/e48871b26ade4a434233d529010ef5e32c7a6cd2/color_histogram.png)

### Embedding-based Anomaly Detection
![Embeddings](https://github.com/hgjlee/cell_classification/blob/e48871b26ade4a434233d529010ef5e32c7a6cd2/embeddings.png)

### Fine-tuned Embeddings
![fine-tuned](https://github.com/hgjlee/cell_classification/blob/e48871b26ade4a434233d529010ef5e32c7a6cd2/fine_tuned.png)

### Class Weighting
![fine-tuned](https://github.com/hgjlee/cell_classification/blob/e48871b26ade4a434233d529010ef5e32c7a6cd2/class_weighting.png)

