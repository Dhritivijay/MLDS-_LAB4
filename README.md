# MLDS Lab Experiment 04

## Image Classification using CNN and Transfer Learning

### Objective

The objective of this experiment is to perform image classification using deep learning techniques. A Convolutional Neural Network (CNN) model is built from scratch and compared with Transfer Learning using a pre-trained MobileNetV2 model. The aim is to observe how transfer learning improves accuracy and reduces training time.

---

### Dataset

The experiment uses the **TensorFlow Flower Dataset**, which contains images of five flower classes:

* Daisy
* Dandelion
* Roses
* Sunflowers
* Tulips

The dataset contains thousands of images and is divided into **training and validation sets** using an 80:20 split.

---

### Tools and Libraries Used

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* Jupyter Notebook

---

### Experiment Tasks

#### 1. Import Libraries

Required libraries such as TensorFlow, Keras, NumPy and Matplotlib are imported to perform image processing, model building and visualization.

#### 2. Load Dataset

The flower dataset is loaded using TensorFlow utilities. The images are automatically resized to **224 × 224 pixels** and divided into training and validation sets.

#### 3. Data Exploration

The dataset is explored by:

* Printing class labels
* Displaying sample images
* Checking image dimensions and batch size

This helps in understanding the structure of the dataset.

#### 4. CNN Model (From Scratch)

A Convolutional Neural Network is created with the following layers:

* Convolution layers for feature extraction
* MaxPooling layers for dimensionality reduction
* Global Average Pooling
* Dense layers for classification
* Dropout for regularization

The model is compiled using **Adam optimizer** and **categorical crossentropy loss**.

#### 5. Transfer Learning

A pre-trained **MobileNetV2** model is used as a feature extractor. The convolutional base is frozen and only the final classification layer is trained on the flower dataset.

This significantly improves training efficiency and performance.

#### 6. Fine Tuning

In the final step, some of the top layers of the pre-trained model are unfrozen and trained again with a smaller learning rate to improve accuracy.

---

### Results

* CNN from scratch achieved moderate accuracy.
* Transfer learning significantly improved accuracy and reduced training time.
* Fine tuning further enhanced the model performance.

This demonstrates the effectiveness of **transfer learning in deep learning applications**.

---

### Conclusion

In this experiment, image classification was performed using both a custom CNN and a transfer learning approach. The results showed that transfer learning with MobileNetV2 provided better performance compared to training a CNN from scratch. This approach is useful when working with limited datasets and helps achieve high accuracy with less training time.

---

### Applications

* Plant and flower recognition
* Medical image classification
* Object detection systems
* Agricultural monitoring

---
