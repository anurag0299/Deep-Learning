# Flower Classification Using Deep Learning 🌸

This project is a deep learning model built to classify images of flowers into different species using Convolutional Neural Networks (CNNs). By leveraging this model, we aim to distinguish between five types of flowers based on their visual features.

## Dataset

The dataset used in this project is the [Flowers Dataset by Rahma Sleam](https://www.kaggle.com/datasets/rahmasleam/flowers-dataset?resource=download) from Kaggle. It contains a variety of images from five flower species, making it ideal for image classification and computer vision projects.

### Flower Categories

1. **Daisy** - Known for its classic white petals with a yellow center.
2. **Dandelion** - Recognized for bright yellow petals, commonly found in fields.
3. **Roses** - A symbol of love, roses appear in multiple colors like red, pink, and white.
4. **Sunflowers** - Known for their large size, yellow petals, and brown center.
5. **Tulips** - Elegant blooms in various vibrant colors.

### Dataset Structure

- **Total Images**: 4,670 images
- **Image Distribution**:
  - Daisy: 633 images
  - Dandelion: 898 images
  - Roses: 641 images
  - Sunflowers: 699 images
  - Tulips: 799 images

Download the dataset [here](https://www.kaggle.com/datasets/rahmasleam/flowers-dataset?resource=download).

## Project Overview

The goal of this project is to build a CNN model to accurately classify images of flowers. The following steps were taken:

1. **Data Preprocessing**:
   - Images were resized, rescaled, and augmented to improve the model’s robustness.
   - The dataset was split into training and validation sets.
   
2. **Model Architecture**:
   - Built a CNN model with layers like Conv2D, MaxPooling2D, and Dense layers.
   - Applied Dropout for regularization to reduce overfitting.
   
3. **Training and Evaluation**:
   - The model was trained for 20 epochs using categorical cross-entropy loss and the Adam optimizer.
   - Early stopping and learning rate reduction were used to select the best-performing model.

4. **Prediction**:
   - After training, the model was tested on unseen images, with predictions displayed alongside the actual images.

## Technologies Used

- **Programming Language**: Python
- **Deep Learning Library**: TensorFlow / Keras
- **Data Manipulation**: NumPy, Pandas
- **Image Processing**: OpenCV
- **Visualization**: Matplotlib

## Project Structure

```plaintext
flower_classification/
├── flower_photos/
│   ├── daisy/
│   ├── dandelion/
│   ├── roses/
│   ├── sunflowers/
│   └── tulips/
├── flower_classification.py
├── README.md
└── requirements.txt
