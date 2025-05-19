
## 🧠 CIFAR-10 Image Classification using CNN & ResNet50 🚀

This project demonstrates how to classify images from the [CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar.html) using deep learning models in Python with TensorFlow and Keras.


### 📁 Dataset

* CIFAR-10 📷: A labeled dataset of **60,000 32x32 color images** in 10 classes:

  
  airplane ✈️, automobile 🚗, bird 🐦, cat 🐱, deer 🦌,
  dog 🐶, frog 🐸, horse 🐴, ship 🚢, truck 🚛
  

* 📥 Downloaded using Kaggle API

*  Includes:

  * train.7z: 50,000 training images
  * trainLabels.csv: Corresponding labels
  * test.7z (optional)

### 🔧 Project Structure

1. ** Dataset Handling**

   * Uses Kaggle API to download CIFAR-10 dataset
   * Extracts .zip and .7z files
   * Reads labels from trainLabels.csv

2. ** Data Preprocessing**

   * Reads images and converts to NumPy arrays
   * Maps string labels to integers
   * Scales pixel values to \[0, 1]
   * Splits data into training & testing sets

3. ** Model 1: Basic Neural Network**

   * Flatten → Dense(64, ReLU) → Dense(10, Softmax)
   * Trained for 10 epochs with adam optimizer

4. ** Model 2: Transfer Learning with ResNet50**

   * Uses ResNet50 (pre-trained on ImageNet)
   * Resizes CIFAR-10 images to (256, 256)
   * Adds custom classification head
   * Fine-tuned for 10 epochs

5. **📊 Evaluation & Visualization**

   * Accuracy and loss plotted over epochs
   * Evaluates on test set

### 📈 Results

 Both models achieve decent accuracy on CIFAR-10.
 ResNet50 performs significantly better due to its deep architecture.

