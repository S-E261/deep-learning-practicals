# 🧠 Deep Learning Practicals — TensorFlow & Keras

A complete collection of hands-on Deep Learning practicals implemented using **TensorFlow**, **Keras**, **NumPy**, **Scikit-learn**, and **Matplotlib**. This repository covers foundational topics from linear algebra with tensors all the way through Autoencoders and RNNs, organized topic by topic for easy navigation.

---

## 📁 Repository Structure

```
deep-learning-practicals/
│
├── 01_tensorflow_basics/
│   ├── matrix_multiplication_2x2.ipynb
│   ├── matrix_multiplication_and_eigen_decomposition.ipynb
│   └── eigenvalues_eigenvectors_3x3.ipynb
│
├── 02_feedforward_neural_networks/
│   ├── regression_ffnn_advertising.ipynb
│   ├── binary_classification_ffnn_diabetes.ipynb
│   └── multiclass_classification_ffnn_iris.ipynb
│
├── 03_regularization_and_early_stopping/
│   ├── regularization_l1_l2.ipynb
│   └── early_stopping_fashion_mnist.ipynb
│
├── 04_cnn/
│   └── cnn_mnist.ipynb
│
├── 05_rnn_lstm/
│   └── rnn_lstm_stock_price.ipynb
│
├── 06_autoencoder/
│   └── autoencoder_mnist.ipynb
│
├── requirements.txt
├── .gitignore
└── README.md
```

---

## 📚 Topic-by-Topic Overview

### 01 — TensorFlow Basics

Before building neural networks, it helps to understand how TensorFlow represents and operates on data. These notebooks cover `tf.constant`, tensor shapes, `tf.matmul` for matrix multiplication, and `tf.linalg.eigh` for computing eigenvalues and eigenvectors — the linear algebra concepts that underpin everything a neural network does internally.

| Notebook | What it covers |
|---|---|
| `matrix_multiplication_2x2.ipynb` | Creating 2×2 constant tensors and multiplying them |
| `matrix_multiplication_and_eigen_decomposition.ipynb` | 2×3 and 3×2 matrix multiplication + eigendecomposition of a 2×2 matrix |
| `eigenvalues_eigenvectors_3x3.ipynb` | Random 3×3 matrix eigenvalues and eigenvectors |

---

### 02 — Feedforward Neural Networks (FFNN)

This is the core of the practicals. All three types of supervised learning tasks are implemented using feedforward networks:

| Notebook | Task | Dataset | Key Concepts |
|---|---|---|---|
| `regression_ffnn_advertising.ipynb` | Regression | Advertising.csv (TV, Radio, Newspaper → Sales) | MSE loss, linear output |
| `binary_classification_ffnn_diabetes.ipynb` | Binary Classification | Pima Indians Diabetes | Sigmoid output, Binary Cross-Entropy |
| `multiclass_classification_ffnn_iris.ipynb` | Multiclass Classification | Iris (3 classes) | One-hot encoding, Softmax, Categorical Cross-Entropy |

The three tasks show how the same base architecture changes only at the output layer and loss function — a fundamental insight in deep learning.

---

### 03 — Regularization & Early Stopping

Overfitting is one of the most common problems when training neural networks. These notebooks demonstrate how to prevent it:

| Notebook | What it covers |
|---|---|
| `regularization_l1_l2.ipynb` | L1, L2, and L1+L2 (ElasticNet) regularization on the Moons dataset — comparison of all three using accuracy curves |
| `early_stopping_fashion_mnist.ipynb` | Training with vs without EarlyStopping callback on Fashion MNIST — shows how to restore best weights |

---

### 04 — Convolutional Neural Networks (CNN)

| Notebook | What it covers |
|---|---|
| `cnn_mnist.ipynb` | Image classification on MNIST using Conv2D + MaxPooling2D + Dense layers. Covers normalization, reshaping for 2D input, one-hot labels, and evaluation |

---

### 05 — Recurrent Neural Networks / LSTM

| Notebook | What it covers |
|---|---|
| `rnn_lstm_stock_price.ipynb` | Time series prediction on Google Stock Price data using a stacked LSTM with Dropout. Covers sliding window sequences, MinMaxScaler normalization, and sequence reshaping |

---

### 06 — Autoencoder

| Notebook | What it covers |
|---|---|
| `autoencoder_mnist.ipynb` | Unsupervised feature compression using a simple Autoencoder on MNIST. Builds separate encoder and decoder models, trains end-to-end, and reconstructs images |

---

## 🛠️ Tech Stack

- **Python 3.10+**
- **TensorFlow / Keras** — model building, training, callbacks
- **NumPy** — numerical operations and data preparation
- **Scikit-learn** — datasets, train/test split, preprocessing, evaluation
- **Matplotlib** — training curves and visualizations
- **Pandas** — data loading and exploration

---

## 🚀 Getting Started

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/deep-learning-practicals.git
cd deep-learning-practicals

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook
```

> **Note on datasets:** Some notebooks use external CSV files (`Advertising.csv`, `pima-indians-diabetes.csv`, `Google_Stock_Price_Train.csv`). These are not included in the repository. You can download them from Kaggle or the UCI Machine Learning Repository. Place the CSV in the same folder as the notebook before running.

---

## 🗺️ Learning Path

If you're exploring this repo to learn, the recommended order is:

**Tensors → FFNN (Regression) → FFNN (Binary) → FFNN (Multiclass) → Regularization → Early Stopping → CNN → RNN/LSTM → Autoencoder**

Each topic builds on the previous one. The FFNN section is the foundation — once you understand how the output activation and loss change across the three task types, everything else becomes much easier to follow.

---

## 👤 Author

Practicals completed as part of a Deep Learning study series using TensorFlow/Keras.
