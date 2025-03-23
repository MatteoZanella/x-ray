# Classification of X-ray Images

This project focuses on developing a machine learning model to classify thoracic X-ray images and detect potential illnesses. The target illnesses of the classification are:

- No illness
- Viral Infection
- Bacterial Infection
- COVID-19

The classification task is approached using both traditional machine learning and neural networks, ensuring robust and accurate predictions.

## 📂 Dataset & Pre-processing

The dataset consists of various files in different formats. The pre-processing step involves converting these files into PyTorch tensors for efficient loading and processing. This step is I/O intensive and is recommended to be performed locally, with the processed files stored in a designated pre-processing folder.

## 🔬 Model Training

### Machine Learning Models

The following machine learning classifiers were trained using scikit-learn:
- Decision Tree Classifier (DT)
- Random Forest (RF)
- Nearest Neighbor Classifier (NN)
- Support Vector Machines (SVM)

Each model underwent hyperparameter tuning to identify the best-performing configuration.

### Neural Network Model

A deep learning model was implemented using PyTorch. The architecture includes:
- Fully connected layers with ReLU activations
- Batch normalization for stabilization
- Cross-entropy loss function for classification

The default weight initialization follows Kaiming Uniform, which improves training efficiency.

## 📊 Evaluation Metrics

The classification models were evaluated using three key metrics:
- Global Accuracy (Acc) – Overall classification performance.
- Mean Class Accuracy (mAcc) – Class-balanced accuracy.
- Mean Intersection-over-Union (mIoU) – Measures per-class overlap between predicted and true labels.

![Traditional ML performances](https://github.com/user-attachments/assets/12075401-156e-4601-aa88-26fb1f8b370b)
