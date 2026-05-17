# CNN-Based Manufacturing Defect Classification

## Project Objective

The objective of this project is to build a Convolutional Neural Network (CNN) model to classify manufacturing defect images into different categories.

The CNN model learns visual patterns such as:
- scratches
- dents
- stains
- normal surfaces

---

# Problem Identification

This dataset represents an Image Classification problem.

Reason:
- Each image belongs to only one class.
- Images are divided into four folders:
  - normal
  - scratch
  - dent
  - stain

The objective is to classify images into the correct category.

---

# Dataset Description

## Classes in Dataset

| Class | Description |
|---|---|
| normal | Surface without defect |
| scratch | Surface with scratch defect |
| dent | Surface with dent defect |
| stain | Surface with stain defect |

## Dataset Statistics

- Total Classes: 4
- Images per Class: 120
- Total Images: 480

## Image Dimensions

- Original Image Size: 96 × 96
- Resized Image Size: 128 × 128

---

# Image Preprocessing

The following preprocessing steps were applied:

1. Image resizing
2. Pixel normalization
3. Training-validation split
4. Data augmentation

## Augmentation Techniques

- Rotation
- Horizontal flip
- Zooming

---

# CNN Architecture

The CNN model contains:

1. Convolution Layer
2. ReLU Activation
3. Max Pooling Layer
4. Flatten Layer
5. Dense Layer
6. Dropout Layer
7. Softmax Output Layer

---

# Model Training

## Training Configuration

| Parameter | Value |
|---|---|
| Optimizer | Adam |
| Loss Function | Categorical Crossentropy |
| Epochs | 10 |
| Batch Size | 32 |

---

# Model Performance

## Final Results

| Metric | Value |
|---|---|
| Training Accuracy | 67% |
| Validation Accuracy | 79% |

The model successfully learned visual defect patterns.

---

# Confusion Matrix Analysis

The confusion matrix shows:
- Normal images were classified most accurately.
- Some confusion occurred between dent and stain classes.
- Scratch images were moderately classified.

---

# Classification Report Analysis

The classification report indicates:

- Best performing class: normal
- Lowest performing class: stain

Overall Accuracy:
- 33%

The model performance can improve with:
- more training data
- deeper CNN architecture
- transfer learning

---

# CNN Concept Explanation

## What is Convolution?

Convolution is a mathematical operation used to extract important image features such as edges, textures, and shapes.

CNN filters scan across the image and learn useful patterns automatically.

---

## Why is Pooling Used?

Pooling reduces image dimensions and computational complexity.

Benefits:
- reduces overfitting
- reduces training time
- preserves important features

---

## Why is ReLU Commonly Used?

ReLU helps CNN models train faster.

ReLU Formula:

f(x) = max(0, x)

Benefits:
- avoids vanishing gradient problem
- improves learning speed

---

## Why CNNs Are Better Than Feed-Forward Networks?

CNNs are specifically designed for image processing.

Advantages:
- automatic feature extraction
- spatial relationship learning
- parameter sharing
- better image understanding

Feed-forward networks cannot efficiently process image structures.

---

# Business Use Case

## Manufacturing Industry

This CNN-based solution can be used for automated quality inspection in manufacturing industries.

Applications:
- scratch detection
- dent detection
- stain detection
- defective product identification

Benefits:
- reduced human error
- faster inspection
- improved product quality
- real-time monitoring

---

# Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Pillow

---

# Conclusion

The CNN model successfully demonstrated image classification using manufacturing defect images.

The project demonstrated:
- convolution operations
- pooling
- activation functions
- CNN training
- image preprocessing
- model evaluation

Future improvements:
- transfer learning
- larger datasets
- deeper CNN architectures
- advanced augmentation techniques