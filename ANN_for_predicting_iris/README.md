# 🌸 Iris Flower Classification (ANN - PyTorch)

📖 **Overview**  
This project implements an **Artificial Neural Network (ANN)** using **PyTorch** to classify iris flowers into three species — *Setosa*, *Versicolor*, and *Virginica* — based on sepal and petal features from the classic **Iris dataset**.

🧠 **Skills Demonstrated**  
- Data preprocessing and feature scaling with `StandardScaler`  
- Tensor conversion and DataLoader usage in PyTorch  
- Building a fully connected neural network (feedforward ANN)  
- Training using **Adam optimizer** and **CrossEntropyLoss**  
- Batch-based training, forward and backward propagation  
- Model evaluation and prediction interpretation  

🧰 **Tools Used**  
Python, PyTorch, Scikit-learn  

⚙️ **Model Architecture**  
- Input Layer: 4 neurons (for 4 features)  
- Hidden Layer: 16 neurons with ReLU activation  
- Output Layer: 3 neurons (for 3 flower classes)  

🚀 **Results**  
- Model successfully learned to classify all three flower types.  
- Training loss decreased steadily over 50 epochs.  
- Predictions closely matched actual labels in the test set.  

📊 **Example Predictions**
| Predicted | Actual | Class Name |
|------------|---------|------------|
| 1 | 1 | Versicolor |
| 2 | 2 | Virginica |
| 0 | 0 | Setosa |

📂 **Notebook**  
See [`Building_ANN.ipynb`](./Building_ANN.ipynb)
