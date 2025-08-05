# **Handwritten Digit Classification with CNN (0.99157 Accuracy 🎯)**

## 📌 **Overview**

This project implements a **Convolutional Neural Network (CNN)** for handwritten digit classification using **PyTorch**. The model was trained on the **MNIST dataset** and achieved a **remarkable accuracy of 99.157%**.

## 🏆 **Achievements**

- **Final Score:** `0.99157`
- **Trained using PyTorch & GPU acceleration**
- **Model saved as `MNIST_DATASET_MODEL.pth`**

## 🛠 **Setup & Installation**

### **1️⃣ Clone the Repository**

```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo
```

### **2️⃣ Install Dependencies**

```bash
pip install -r requirements.txt
```

### **3️⃣ Run Inference on New Data**

```python
import torch
from model import MyModel  # Replace with your model class

# Load the trained model
model = MyModel()
model.load_state_dict(torch.load("MNIST_DATASET_MODEL.pth"))
model.eval()

# Example prediction
import numpy as np
input_tensor = torch.tensor(np.random.rand(1, 1, 28, 28), dtype=torch.float32) 
prediction = torch.argmax(model(input_tensor)).item()
print(f"Predicted Label: {prediction}")
```

## 🚀 **Training Process**

1. Preprocessed the dataset
2. Built a deep **CNN architecture**
3. Trained using **Adam optimizer** with cross-entropy loss
4. Achieved high accuracy through **hyperparameter tuning**

## 📝 **Model Details**

- **Input:** Handwritten digits (grayscale images, 28x28 pixels)
- **Architecture:** CNN with multiple convolutional and fully connected layers
- **Output:** Predicted digit (0-9)

## 📂 **Files in this Repository**

- `MNIST_DATASET_MODEL.pth` → Trained model
- `mnist-dataset.ipynb` → Model training script
- `predictions (1).csv` → Prediction File
- `README.md` → This documentation

## 💪 **Contributing**

Feel free to fork this repo, submit issues, or contribute improvements!

## ✨ **License**

This project is open-source and available under the [MIT License](LICENSE).
