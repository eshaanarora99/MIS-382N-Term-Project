# MIS 382N Term Project - ScanSense AI: Enhancing Grocery Self Checkout with Machine Learning

The term project for the MIS 382N (Advanced Machine Learning) Course for Fall 2024

### Overview
ScanSense AI is a machine learning solution designed to streamline the self-checkout process for non-barcoded items in grocery stores. By leveraging deep learning models and robust preprocessing techniques, ScanSense AI enhances the accuracy and efficiency of item classification, even in challenging real-world conditions such as poor lighting or items wrapped in plastic bags or produce bags.

### Key Features
- **Convolutional Neural Network (CNN):** The initial model, designed for baseline item classification.
- **ResNet Model:** A refined, deeper architecture that addresses the limitations of the CNN.
- **Data Augmentation:** Real-world variability is simulated through techniques (e.g., random rotations, brightness adjustments, cropping, and Gaussian blur.)
- **Image Segmentation:** Using OpenCV and HSV-based color space processing, the system isolates produce from backgrounds, enhancing model focus and accuracy.
- **Cost-Aware Fallback Strategy:** Minimizes customer dissatisfaction and financial losses by undercharging when confidence in classification is low.

### Repository Contents
- **AML_Final_Project_CNN_Final.ipynb:** Implementation and results of the CNN model for item classification.
- **AML_Final_Project_Resnet_Final.ipynb:** Final ResNet model used for robust grocery item classification.
- **DataAugmentation.ipynb:** Notebook detailing the data augmentation pipeline.
- **Predict_and_Misclassification_Code.ipynb:** Notebook to evaluate predictions, highlight misclassification scenarios, and test fallback strategies.
- **README.md:** This file, providing an overview of the project and its key components.

### Dataset
The model utilizes a dataset sourced from Kaggle, featuring 36 classes of fruits and vegetables. The dataset is split into training, validation, and testing sets, with data preprocessing and augmentation ensuring optimal performance. The dataset is available at: https://www.kaggle.com/datasets/kritikseth/fruit-and-vegetable-image-recognition

### Results
- **ResNet Performance:** Achieved a validation accuracy of 78.6% and improved classification in challenging scenarios such as distorted or bagged items.
- **Fallback Mechanism:** Reduced customer overcharging by predicting lower-cost items when confidence thresholds are not met.

### Future Enhancements
- Improve model accuracy with larger, more diverse datasets.
- Incorporate advanced architectures like Vision Transformers.
- Refine the fallback mechanism to address confident misclassifications.

### How to Use
1. Clone the repository:  
   ```bash
   git clone https://github.com/eshaanarora99/MIS-382N-Term-Project/
   ```
2. Open the notebooks in a Jupyter environment to explore and execute individual components.
