# Signature-Verification-using-CNN-and-Traditional-Feature-Extraction]
# Signature Verification using CNN and Traditional Feature Extraction

This project focuses on classifying handwritten signatures as genuine or forged using Convolutional Neural Networks (CNN) and comparing its performance with traditional feature engineering techniques like HOG and SIFT.

## 📁 Dataset
We used the [Signature Verification Dataset](https://www.kaggle.com/datasets/robinreni/signature-verification-dataset) from Kaggle. The dataset contains genuine and forged signatures for 55 individuals in structured folders.

## 🧠 Methods Implemented
- **CNN**: A custom convolutional neural network was trained on preprocessed 128x128 grayscale images.
- **HOG + Logistic Regression**: Histogram of Oriented Gradients features extracted and classified using logistic regression.
- **SIFT + SVM**: Scale-Invariant Feature Transform used for keypoint-based feature extraction, classified using Support Vector Machines.

## ⚙️ Preprocessing
- Images resized to 128x128 pixels
- Normalization
- Data leakage prevention using MD5 hashes
- CSV header adjustments and pair matching

## 📊 Evaluation Metrics
- **Precision**
- **Recall**
- **F1-score**
- **Accuracy**
- **Confusion Matrix**

## 🧪 Results
| Model                  | Accuracy | Precision | Recall | F1-score |
|------------------------|----------|-----------|--------|----------|
| CNN                   | 93%      | 0.94      | 0.93   | 0.93     |
| HOG + LogisticRegression | 73%     | 0.73      | 0.73   | 0.73     |
| SIFT + SVM            | 63%      | 0.63      | 0.63   | 0.63     |

## 📈 Visualizations
- Training & test accuracy plots
- Confusion matrices
- Model architecture tables

## 🧩 Conclusion
The CNN model significantly outperformed traditional methods. With the application of data augmentation and regularization techniques, the CNN model achieved higher accuracy and generalization capabilities.

## 📄 Report
For a detailed breakdown, check out the [Report.pdf](./Report.pdf) in this repository.
