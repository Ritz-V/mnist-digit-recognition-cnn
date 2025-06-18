# 🧠 Handwritten Digit Recognition using CNN

## 📌 Project Overview

This project implements a **Convolutional Neural Network (CNN)** to recognize handwritten digits (0–9) using the **MNIST dataset**. It provides an intuitive user interface to upload an image, draw a digit, or use the webcam for live digit prediction.


## ✅ Key Features

* Trained a CNN using the MNIST dataset with 99%+ accuracy
* Image input options:

  * 📤 Upload handwritten digit image
  * 🎥 Capture digit via webcam
  * ✏️ Draw digit using an interactive canvas
* Real-time prediction with confidence score
* Includes complete image preprocessing pipeline
* Built entirely in Google Colab
* Model saved in `.h5` format for reuse


## 🛠️ Tech Stack

* Python
* TensorFlow / Keras
* OpenCV
* NumPy, Matplotlib
* Google Colab

 📁 File Structure


digit-recognition-cnn/
├── 📂 model/
│   └── mnist_cnn_model.h5            # Trained model (HDF5 format)
│
├── 📂 notebooks/
│   ├── cnn_model_training.ipynb      # Notebook for training the CNN
│   └── digit_recognition_interface.ipynb  # Final notebook with UI (upload/draw/camera)
│
├── 📄 README.md                      # Project documentation
├── 📄 requirements.txt               # Python libraries used
├── 📄 .gitignore                     # Ignore unnecessary files


 🧠 CNN Architecture Summary

 Input: 28x28 grayscale image
 Conv2D (3x3) + ReLU + MaxPooling
 Flatten → Dense(128) → Dense(10 with Softmax)
 Optimizer: Adam
 Loss: Sparse Categorical Crossentropy



🚀 How to Use

1. Open the notebook `digit_recognition_interface.ipynb` in Google Colab
2. Run the cells to load the trained model
3. Choose input method:

    Upload image
    Use webcam
    Draw using canvas
4. Get the prediction with confidence level!



 ⚠️ Limitations

 Accuracy may vary with poor lighting or unclear handwriting
 Model is trained only on MNIST (digits 0–9)
 Webcam input may require multiple tries for correct prediction



 📈 Future Improvements

 Retrain on more diverse datasets (like EMNIST)
 Add mobile support or deploy as web app
 Integrate with real-time OCR systems


Made with ❤️ by Riddhi Vyas


