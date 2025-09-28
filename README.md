# 🚗 Self-Driving Car Simulation

This repository contains a project that demonstrates end-to-end steering angle prediction for self-driving cars using deep learning.

## 📌 Overview

The goal of the project is to train a model that predicts the steering angle of a car from camera images. It leverages convolutional neural networks with transfer learning to map visual input to driving commands.

## 🔄 Workflow

1. **Dataset**: Driving images and steering logs are provided (from the `track/` folder).
2. **Preprocessing**: Images are cropped, resized, normalized, and augmented to improve generalization.
3. **Modeling**: A CNN model (based on VGG19) is trained to predict steering angles.
4. **Training & Evaluation**: The model is trained with mean squared error loss and evaluated with validation data.
5. **Results**: Training/validation loss curves and sample predictions are visualized.
6. **Saving**: The final model is saved as `Saved_Model.h5` for reuse.

## 📊 Results

* Steering-angle prediction model trained for 25 epochs.
* Training and validation performance visualized.
* Model saved for later inference.

## 📂 Project Files

```
Self_Driving_Car.ipynb    # Main notebook with code and explanations
track/driving_log.csv     # Driving log with steering data
track/IMG/                # Image dataset
Saved_Model.h5            # Trained model (output)
```

## 🛠️ Tools & Libraries

* Python, TensorFlow/Keras
* OpenCV, Albumentations
* NumPy, Pandas, Matplotlib

## 🚀 Usage

1. Clone dataset and repository.
2. Open and run `Self_Driving_Car.ipynb`.
3. Train the model and save predictions.

## 🌐 Deployment

The exported model (`Saved_Model.h5`) can be integrated into driving simulators such as **CARLA** or the **Udacity Self-Driving Car Simulator** to visualize and test real-time steering predictions.

---

