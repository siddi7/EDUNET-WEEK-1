# EDUNET-WEEK-1
Plant Disease Classification 

**Dataset Structure:**

The "New Plant Diseases Dataset" contains approximately 87,000 RGB images

38 different classes of healthy and diseased crop leaves

**Preprocessing and Augmentation:**

Resizing images to 224x224 pixels

**Data augmentation techniques including:**

Horizontal flipping

**Model Architecture:**

Hybrid CNN-LSTM model combining spatial and temporal features

**CNN component for feature extraction:**

4 convolutional layers with increasing filters (32, 64, 128, 256)

Max pooling layers to reduce dimensionality

**LSTM component for sequence analysis:**

2 LSTM layers (256 and 128 units)

**Training Strategy:**

Categorical cross-entropy loss function

Adam optimizer

30 epochs maximum with early stopping

**Evaluation Metrics:**

Accuracy, Precision, Recall, F1 Score, ROC-AUC, Confusion Matrix

**Visualization:**

Training and validation accuracy/loss curves, Sample predictions with correct/incorrect labels, Confusion matrix heatmap
