# 🧠 Digit Cave – Handwritten Digit Recognition (CNN vs MLP)
An intermediate-level deep learning project that compares Convolutional Neural Networks (CNN) and Multi-Layer Perceptrons (MLP) on the MNIST handwritten digits dataset.
This project demonstrates data augmentation, learning rate scheduling, and visual comparison of model performance — ideal for students and developers building a solid foundation in image classification and model optimization.

# 🚀 Project Overview
The Digit Cave aims to explore how architectural depth and feature extraction impact performance in handwritten digit recognition.
Two models were trained:
1. 🧩 MLP (Baseline) – Fully connected layers with flattened 28×28 inputs.
2. 🎯 CNN (Enhanced) – Convolutional and pooling layers for spatial pattern extraction.
Dataset: MNIST Handwritten Digits
Images: 70,000 grayscale digits (28×28 px)

# ⚙️ Features Implemented
✅ Model comparison: CNN vs MLP
📈 Data augmentation (rotation, shift, zoom)
🔁 Learning rate scheduler (ReduceLROnPlateau)
🧮 Accuracy, loss, and confusion matrix visualizations
🔍 Evaluation metrics: precision, recall, F1-score
🖼️ Sample prediction visualization

# 🧩 Model Architecture
## CNN
- 2 Conv2D layers (ReLU + MaxPooling)
- Dropout regularization
- Dense(128) → Output(10, softmax)

## MLP
- Flatten input → Dense(512) → Dropout → Output(10, softmax)

# 📊 Results and Comparison
## Model	 Train Accuracy	 TestAccuracy	 Parameters	      Observations
MLP	     98.1%	             97.0%	       ~0.7M	     Good baseline,but overfits slightly
CNN	     99.5%	             99.1%	       ~1.2M	     Better generalization & spatial awareness

# 📉 Performance Visualization
## Training vs Validation Accuracy

<img width="413" height="391" alt="image" src="https://github.com/user-attachments/assets/6083a0ca-9bda-4598-ac65-93d8dbc25e63" />

## Training vs Validation Loss

<img width="439" height="387" alt="image" src="https://github.com/user-attachments/assets/063df650-dfc2-4061-ba04-5fc51d03601c" />

## Confusion Matrix (CNN)

<img width="546" height="444" alt="image" src="https://github.com/user-attachments/assets/116d33bc-b487-49b3-8974-748acd2da188" />

# 🧠 Insights
- CNNs significantly outperform MLPs in spatial recognition tasks like MNIST.
- Data augmentation improves generalization and prevents overfitting.
- ReduceLROnPlateau dynamically lowers the learning rate, stabilizing convergence.
- Even small CNN architectures can achieve >99% accuracy on MNIST with tuning.

# 🧰 Tech Stack
- Language: Python 3.x
- Frameworks: TensorFlow / Keras
- Libraries: NumPy, Matplotlib, Seaborn, Scikit-learn
- Environment: Jupyter Notebook

# 📦 How to Run
## Clone this repo:
git clone https://github.com/18mahi/digital_cave.git
-cd  Digit-Cave

## Install dependencies:
pip install -r requirements.txt

### 🧾 requirements.txt
Create a file named requirements.txt in your project folder with the following content:
tensorflow==2.16.1
numpy==1.26.4
matplotlib==3.9.0
seaborn==0.13.2
scikit-learn==1.5.0
pandas==2.2.2
jupyter==1.1.0

## Run the notebook:
jupyter notebook Digit_Cave.ipynb

# 🏁 Future Improvements
- Add deeper CNNs (LeNet, VGG-style)
- Experiment with dropout rates and batch normalization
- Deploy via Streamlit for interactive digit recognition

# 🧑‍💻 Author
Mahi Jindal
🎓 CSE (AI/ML) | Passionate about Deep Learning & Robotics
🌐 LinkedIn-https://www.linkedin.com/in/mahi-jindal-867109245/
 • GitHub- https://github.com/18mahi

# 📄 License
This project is open-source under the MIT License.
