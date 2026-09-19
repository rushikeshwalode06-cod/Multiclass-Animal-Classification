# 🐾  Multiclass-Animal-Classification
Animal Classification is a deep learning project that classifies animal images into 15 different categories using a custom CNN model. The project includes image preprocessing, data augmentation, convolutional layers, pooling, and model training with Adam optimizer. The trained model can predict animal classes from new images.

# 🐾 Animal Classification Using CNN

## 📌 Project Overview

Animal Classification is a deep learning image classification project that identifies animals from images using a **Convolutional Neural Network (CNN)**. The model is trained on an animal image dataset and can classify images into **15 different animal categories**.

## 🎯 Objective

The main objective of this project is to build a CNN-based image classification model that can automatically recognize different animal species from input images.

## 🛠️ Technologies & Skills

* 🐍 Python
* 🧠 Deep Learning
* 🤖 TensorFlow / Keras
* 🖼️ Computer Vision
* 🧩 Convolutional Neural Network (CNN)
* 🔄 Data Augmentation
* 📊 NumPy
* 📈 Matplotlib
* 📦 KaggleHub

## 📂 Dataset

The project uses an animal image dataset downloaded using **KaggleHub**.

The model is designed to classify images into 15 animal categories.

### 🐯 Animal Classes

* 🐻 Bear
* 🐦 Bird
* 🐱 Cat
* 🐄 Cow
* 🦌 Deer
* 🐕 Dog
* 🐬 Dolphin
* 🐘 Elephant
* 🦒 Giraffe
* 🐎 Horse
* 🦘 Kangaroo
* 🦁 Lion
* 🐼 Panda
* 🐯 Tiger
* 🦓 Zebra

The class names are defined in the trained-model prediction file.

## 🔄 Project Workflow

1. 📥 Download the animal dataset
2. 🗂️ Load images from the dataset
3. 🖼️ Resize images to **160 × 160**
4. 🔄 Apply data augmentation
5. ⚙️ Rescale image pixel values
6. 🧠 Build CNN architecture
7. 🏋️ Train the model
8. 📊 Validate model performance
9. 💾 Save/load the trained model
10. 🔍 Predict the animal class from a new image

![ml](https://github.com/rushikeshwalode06-cod/Multiclass-Animal-Classification/blob/main/Animai1_image.png?raw=true)

## 🧠 CNN Model Architecture

The project uses a custom CNN architecture consisting of:

* Random Flip & Random Rotation
* Rescaling
* Conv2D — 16 filters
* MaxPooling2D
* Conv2D — 32 filters
* MaxPooling2D
* Conv2D — 64 filters
* MaxPooling2D
* Flatten
* Dense — 128 neurons
* Dense — 15 neurons with Softmax

The architecture is implemented directly in the project file.

## ⚙️ Model Configuration

| Parameter       | Value                           |
| --------------- | ------------------------------- |
| Image Size      | 160 × 160                       |
| Batch Size      | 32                              |
| Optimizer       | Adam                            |
| Learning Rate   | 0.0001                          |
| Loss Function   | Sparse Categorical Crossentropy |
| Metric          | Accuracy                        |
| Training Epochs | 50                              |
| Output Classes  | 15                              |

These training settings are defined in the project code.

## 🔄 Data Augmentation

To increase image variation during training, the project applies:

* 🔁 Random Horizontal Flip
* 🔄 Random Rotation

This helps create variations of training images before they are passed to the CNN.

## 🔍 Prediction

A separately saved model can be loaded using Keras and used to predict the class of a new animal image.

The prediction process includes:

**Input Image → Image Array → Model Prediction → Argmax → Animal Class**

The trained model is loaded from `Multi_Animal_class.h5`.

## 📊 Model Evaluation

The project tracks:

* Training Accuracy
* Validation Accuracy
* Training Loss
* Validation Loss

These metrics can be used to understand how the CNN performs during training.

## 🚀 Future Improvements

* Improve classification accuracy
* Add more animal categories
* Use transfer learning with pretrained CNN models
* Add a prediction confidence score
* Deploy the model using **Streamlit or Flask**
* Create a user-friendly web interface
* Add real-time image classification

## 🏁 Conclusion

This project demonstrates how a **Convolutional Neural Network** can be used for multi-class animal image classification. The model uses image preprocessing, augmentation, convolutional layers, pooling, and dense layers to learn visual patterns and classify images into 15 animal categories.

![ml](https://github.com/rushikeshwalode06-cod/Multiclass-Animal-Classification/blob/main/Animal_image.png?raw=true)
