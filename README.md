# 🩻 **Medical Image Classification using CNN**

This project leverages **Convolutional Neural Networks (CNNs)** to classify **medical images** and determine whether a bone is fractured or not. The goal is to develop an automated system to assist healthcare professionals by analyzing **X-ray images** and identifying bone fractures efficiently.

## 🗂️ **Dataset**

The dataset used in this project consists of **X-ray images** that are labeled as either "**fractured**" or "**not fractured**." These images are preprocessed to normalize and resize them, ensuring that they are suitable for training the **CNN model**.

## 🛠️ **Methodology**

###  **Preprocessing**:
- Images are resized to a fixed dimension.
- **Data augmentation** techniques such as **rotation**, **flipping**, and **scaling** are applied to increase the diversity of the dataset and improve the model’s robustness.

###  **CNN Architecture**:
- A **Convolutional Neural Network (CNN)** is implemented with several layers, including **convolutional layers**, **pooling layers**, and **dense layers**, to extract features and make predictions.

###  **Training**:
- The model is trained using a training set and evaluated on a separate test set to assess its performance.

###  **Evaluation Metrics**:
- **Accuracy**, **precision**, **recall**, and **F1-score** are calculated to evaluate the model's effectiveness in classifying bone fractures.

##  **Model Architecture**

The model is built using a simple **CNN** with the following structure:

- **Input Layer**: Takes **grayscale images** of size `SIZE x SIZE`.
- **Convolutional Layers**: Three layers (with **32**, **64**, and **128 filters**) learn features like edges and patterns.
- **Max Pooling Layers**: Reduce image size and keep the important features.
- **Flatten Layer**: Converts the 2D features into a 1D vector.
- **Fully Connected Layers**: The final layer predicts whether the bone is **fractured** or **not fractured** using a **sigmoid activation**.

## 📈 **Results**

The model will output its **accuracy** and **loss** on the test dataset, along with predictions for each image, indicating whether a bone is fractured or not.

##  **Requirements**

- **TensorFlow 2.x**
- **NumPy**
- **Matplotlib** (for visualizing results)
- **scikit-learn** (for data processing)
- **Gradio** (for interactive UI)

