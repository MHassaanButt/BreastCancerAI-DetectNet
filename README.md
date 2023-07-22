# BreastCancerAI-DetectNet

## Description
BreastCancerAI-DetectNet is an AI-powered breast cancer detection algorithm that leverages the power of EANet (External Attention Transformer) for image classification. The goal of this project is to automatically identify whether a patient is suffering from breast cancer or not by analyzing biopsy images.

Breast cancer is the second most common cancer in women and men worldwide. It occurs when cells in the breast start to grow uncontrollably, forming tumors that can be observed on x-rays or felt as lumps. Detecting breast cancer at an early stage is crucial for effective treatment and improved patient outcomes.

## The Challenge
The primary challenge in this project is to build a robust and accurate algorithm that can effectively distinguish between malignant (cancerous) and benign (non-cancerous) breast tissues based on biopsy images. The algorithm must be capable of identifying patterns and features in the images to make accurate predictions.

## Data
The dataset used for training and evaluation can be downloaded from the [Breast Cancer Histopathological Database (BreakHis)](https://web.inf.ufpr.br/vri/databases/breast-cancer-histopathological-database-breakhis/). This dataset contains microscopic biopsy images of breast tissue samples, and it is a binary classification problem, with one class representing malignant cases and the other representing benign cases.

## Performance Metrics
To evaluate the model's performance, traditional accuracy is not the ideal metric due to class imbalance in the dataset. Instead, we will focus on the following metrics:

- **Precision**: The ratio of correctly predicted positive observations to the total predicted positive observations.
- **Recall**: The ratio of correctly predicted positive observations to all the observations in the actual positive class.
- **F1-Score**: The harmonic mean of Precision and Recall, providing a balance between the two metrics.

These metrics give us a better understanding of true positives, true negatives, false positives, and false negatives, enabling us to assess the classifier's performance more effectively.

## Confusion Matrix
The Confusion Matrix is a crucial metric for analyzing misclassifications. Each row of the matrix represents instances in a predicted class, while each column represents instances in the actual class. The diagonals represent the classes that have been correctly classified, which allows us to identify the classes that are being misclassified and the classes to which they are misclassified.

![ETA_Confusion_Matrix](https://github.com/MHassaanButt/BreastCancerAI-DetectNet/assets/30599669/6dea4aab-3354-458f-8f13-0f7d82614328)

## Classification Report

The classification report provides a comprehensive summary of various performance metrics for the model, including precision, recall, and F1-score, for both classes (malignant and benign). It gives a quick overview of the model's overall performance.

### Classification Report:
          precision    recall  f1-score   support

       0       0.99      0.85      0.91       250
       1       0.87      0.99      0.92       250

accuracy                           0.92       500


## Contributions
Contributions to BreastCancerAI-DetectNet are welcome! If you have suggestions, bug fixes, or improvements, feel free to open an issue or submit a pull request.

## License
This project is licensed under the [MIT License](LICENSE).

---
By building BreastCancerAI-DetectNet, we aim to make a positive impact in the early detection of breast cancer, ultimately contributing to better patient outcomes and improved healthcare. We hope that this project will be a valuable resource for researchers and practitioners in the medical field. Let's work together to combat breast cancer with the power of AI!
