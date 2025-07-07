😷 Face Mask Detection using CNN and SVM

This project presents a comparative study between a **Convolutional Neural Network (CNN)** and a **Support Vector Machine (SVM)** model for face mask detection using image classification.

The goal is to determine whether individuals in an image are **wearing a face mask or not**, and to evaluate the performance of both traditional machine learning and deep learning approaches.

📁 Dataset

- The dataset contains two folders:
  - `With Mask`: Images of people wearing masks
  - `Without Mask`: Images of people without masks
- All images were resized to **64x64 pixels** for training
- Dataset used: [Face Mask Detection Dataset](https://www.kaggle.com/datasets/omkargurav/face-mask-dataset) (mounted via Google Drive in Colab)

🧠 Models Used

1. **CNN Model (Keras with TensorFlow backend)**
- Automatically extracts spatial features
- Achieved **~90% accuracy**
- Layers: Conv2D, MaxPooling2D, Flatten, Dense
- Used ImageDataGenerator for training/validation split and augmentation

2. **SVM Model (Traditional ML)**
- Images flattened into 1D vectors (64×64×3 = 12288 features)
- Trained using `sklearn.svm.SVC`
- Achieved **~85.64% accuracy**
- Faster to train but lower performance than CNN

📊 Evaluation Metrics

- Accuracy
- Precision, Recall, F1-Score (via classification report)
- Comparison of both approaches based on performance and simplicity

🚀 How to Run

1. Open `CNN_Model.ipynb` or `SVM_Model.ipynb` in Google Colab
2. Mount your Google Drive (for dataset access)
3. Install required libraries if needed
4. Run all cells

---

✍️ Author

- Tanisha Sharma
- MCA Researcher | AI Enthusiast | Kaggle Learner

