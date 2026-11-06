# Face Recognition System
### Comparative Performance Analysis of FaceNet, ArcFace and SFace

## Project Overview

This project focuses on developing and evaluating a face recognition system using three pretrained deep learning models: FaceNet, ArcFace and SFace.

The primary objective is to compare the recognition performance of these models using a common facial image dataset and a Support Vector Machine (SVM) classifier.

The system identifies individuals from facial images and investigates how different facial expressions and imaging conditions affect recognition performance.

## Project Objectives

- Develop a face recognition pipeline using pretrained deep learning models.
- Extract facial feature embeddings from input images.
- Train an SVM classifier for individual identification.
- Compare FaceNet, ArcFace and SFace using the same experimental dataset.
- Evaluate recognition performance using standard classification metrics.
- Investigate recognition performance across different facial variations.
- Identify the most effective model based on accuracy and computational efficiency.

## Dataset Information

**Dataset:** Yale Face Database

| Property | Details |
|---|---|
| Original Images | 165 |
| Original Individuals | 15 |
| Images per Individual | 11 |
| Selected Individuals | 10 |
| Selected Images | 110 |
| Image Format | GIF |
| Image Type | Grayscale |

The dataset contains facial variations including happy, sad, normal, surprised, sleepy, wink, glasses and different lighting conditions.

**Dataset source:**  
https://vision.ucsd.edu/datasets/yale-face-database

Original dataset files are maintained separately and are not included in this public repository.

## Models Used

The project compares three pretrained face recognition models.

### 1. FaceNet
- Generates numerical facial embeddings.
- Uses a 128-dimensional embedding representation in this implementation.
- Implemented using DeepFace.
- Combined with an SVM classifier.

### 2. ArcFace
- Uses an angular-margin-based face recognition approach.
- Generates discriminative facial embeddings.
- Combined with the same SVM classification approach.

### 3. SFace
- A lightweight face recognition model.
- Generates facial feature embeddings.
- Used to evaluate recognition performance and computational efficiency.

## System Methodology

The project follows a common experimental pipeline:

1. Dataset loading and inspection.
2. Selection of 10 individuals.
3. Image preprocessing.
4. Facial feature extraction using pretrained models.
5. Embedding normalization.
6. SVM classifier training.
7. Three-fold cross-validation.
8. Performance evaluation.
9. Comparative analysis of all three models.

## Technology Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Development Platform | Google Colab |
| Hardware Accelerator | NVIDIA T4 GPU (when available) |
| Deep Learning | TensorFlow, DeepFace |
| Face Recognition | FaceNet, ArcFace, SFace |
| Machine Learning | Scikit-learn |
| Image Processing | OpenCV, Pillow |
| Data Processing | NumPy, Pandas |
| Visualization | Matplotlib, Seaborn |
| Version Control | Git and GitHub |

## Evaluation Metrics

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- Facial Variation-wise Accuracy
- Model Loading Time
- Embedding Extraction Time
- SVM Training Time
- Prediction Time


## Team Contributions

This is a collaborative project involving three members.

| Team Member | Assigned Model |
|---|---|
| Member 1 | FaceNet |
| Member 2 | ArcFace |
| Member 3 | SFace |

All members follow the shared dataset and evaluation protocol to ensure a consistent comparison.



## Expected Outcome

The final system will provide a comparative evaluation of FaceNet, ArcFace and SFace.

The results will help determine which model performs best on the selected facial dataset in terms of recognition performance, robustness across facial variations and computational efficiency.

## Limitations

- The dataset contains a relatively small number of individuals and images.
- Evaluation results are specific to the selected dataset.
- Performance on controlled facial images may differ from real-world recognition scenarios.
- The experiment uses closed-set identity recognition.

## Academic Use

This repository is developed for academic and educational purposes.

Dataset usage and model-weight licensing conditions must be respected.

## Acknowledgements

We acknowledge the researchers and institutions responsible for developing and maintaining the Yale Face Database, FaceNet, ArcFace and SFace.

