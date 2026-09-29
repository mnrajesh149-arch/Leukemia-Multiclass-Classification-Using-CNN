# Leukemia Multiclass Classification Using CNN

This project implements a **deep learning-based image classification system for leukemia classification** using a Convolutional Neural Network (CNN) with TensorFlow and Keras.

The model is trained on the **Kaggle Leukemia dataset** and performs multiclass classification into four categories:

* **Benign**
* **Early**
* **Pre**
* **Pro**

## Project Workflow

1. Download the Leukemia dataset using `kagglehub`.
2. Mount Google Drive for accessing images.
3. Resize input images to **224 × 224 pixels**.
4. Normalize pixel values using rescaling.
5. Split the dataset into **80% training and 20% validation**.
6. Build a CNN architecture using:

   * Conv2D layers
   * MaxPooling2D layers
   * Flatten layer
   * Dense layers
   * Softmax output layer
7. Train the model for **10 epochs** using the Adam optimizer.
8. Save the trained model as `leukemia.h5`.
9. Load the saved model for prediction.
10. Test the model on a new leukemia image and generate the predicted class.

## Dataset

The project uses the Kaggle **Leukemia** dataset by `mehradaria`.

The notebook contains **3,256 images** in total:

* Training: 2,607 images
* Validation: 649 images
* Number of classes: 4

## Model Architecture

The CNN consists of:

* Conv2D — 32 filters
* MaxPooling2D
* Conv2D — 64 filters
* MaxPooling2D
* Conv2D — 128 filters
* MaxPooling2D
* Flatten
* Dense — 128 neurons
* Dense — 4 neurons with Softmax activation

The model uses:

* **Optimizer:** Adam
* **Loss:** Categorical Crossentropy
* **Metric:** Accuracy
* **Input size:** 224 × 224 × 3

## Results

During training, the model achieved a training accuracy of approximately **97.12%** in the 10th epoch, while the highest validation accuracy observed in the notebook was approximately **79.82%**.

The notebook also demonstrates prediction on an individual image, with the sample image classified as **Early**.

## Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Matplotlib
* KaggleHub
* Google Colab
* Convolutional Neural Networks (CNN)
* Deep Learning
* Image Classification

## Files

```text
Leukemia_multiclass_classification.ipynb
```

## Disclaimer

This project is intended for **educational and research purposes**. The model's predictions should not be considered a medical diagnosis or a replacement for professional medical evaluation.
