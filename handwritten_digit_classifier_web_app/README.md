# Handwritten Digit Classifier (MNIST)

This repository contains a **Convolutional Neural Network (CNN)** model trained on the **MNIST dataset** to classify handwritten digits (0-9). The project also includes a **Streamlit web app** to upload images and recognize handwritten digits in real-time.  

---

## 🗂️ Project Overview

| Project | Description | Tools |
|---------|-------------|-------|
| Handwritten Digit Classifier | A CNN-based model trained on MNIST dataset to classify digits from 0 to 9. Includes a Streamlit app for real-time digit recognition. | Python, PyTorch, Torchvision, Streamlit, Matplotlib, Seaborn |

---

## 📊 Dataset

- **MNIST dataset** of handwritten digits
- **Training samples:** 60,000  
- **Test samples:** 10,000  
- **Image size:** 28x28 pixels (grayscale)  

The dataset is loaded using `torchvision.datasets.MNIST` and normalized to improve model performance.

---

## 🖥️ Model Architecture

**CNNModel** consists of:  

1. **Conv Layer 1:** 1 input channel → 16 output channels, kernel size 3x3  
2. **ReLU activation**  
3. **Max Pooling:** 2x2  
4. **Conv Layer 2:** 16 → 32 channels, kernel size 3x3  
5. **ReLU activation**  
6. **Max Pooling:** 2x2  
7. **Fully Connected Layer 1:** 32*7*7 → 512  
8. **ReLU activation**  
9. **Fully Connected Layer 2:** 512 → 10 (digit classes)  

**Loss Function:** CrossEntropyLoss  
**Optimizer:** Adam (learning rate = 0.001)  

---

## 📈 Training Performance

- **Epochs:** 10  
- **Final Accuracy:** ~99% on test set  

**Classification Report:**

| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| 0 | 0.99 | 1.00 | 0.99 | 980 |
| 1 | 1.00 | 0.99 | 1.00 | 1135 |
| 2 | 1.00 | 0.99 | 0.99 | 1032 |
| 3 | 0.99 | 1.00 | 0.99 | 1010 |
| 4 | 1.00 | 0.99 | 0.99 | 982 |
| 5 | 0.99 | 0.99 | 0.99 | 892 |
| 6 | 0.99 | 0.99 | 0.99 | 958 |
| 7 | 0.99 | 0.99 | 0.99 | 1028 |
| 8 | 0.99 | 0.99 | 0.99 | 974 |
| 9 | 0.98 | 0.99 | 0.98 | 1009 |

- Confusion matrix shows most predictions are correct, with very few misclassifications.

---

## 🖼️ Web App (Streamlit)

- **Upload an image** of a handwritten digit.  
- **Click "Recognize"** to predict the digit.  
- Displays the uploaded image alongside predicted and true labels.

**Technologies:**  
- Streamlit (front-end)  
- PyTorch (model inference)  
- PIL (image handling)  
- Torchvision (image transformations)  

---

## ⚡ How to Run

1. Clone the repository:

```bash
git clone <repo_url>
cd mnist_cnn_app
```

2. Install dependencies:
```
pip install -r requirements.txt
```

3. Run the Streamlit app:
```
streamlit run app.py
```

4. Upload an image of a handwritten digit and see the prediction.
