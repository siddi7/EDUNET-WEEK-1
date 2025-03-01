# EDUNET-WEEK-1
Plant Disease Classification 

**Dataset Structure:**

The "New Plant Diseases Dataset" contains approximately 87,000 RGB images

38 different classes of healthy and diseased crop leaves

Split into 80% training and 20% validation sets


**Preprocessing and Augmentation:**

Resizing images to 224x224 pixels

Normalization (scaling pixel values to 0-1)

**Data augmentation techniques including:**

Random rotation (up to 20 degrees)

Width and height shifts (up to 20%)

Shear and zoom transformations

Horizontal flipping


Batch processing to efficiently manage memory


**Model Architecture:**

Hybrid CNN-LSTM model combining spatial and temporal features

**CNN component for feature extraction:**

4 convolutional layers with increasing filters (32, 64, 128, 256)

Max pooling layers to reduce dimensionality


**LSTM component for sequence analysis:**

2 LSTM layers (256 and 128 units)

Dense layer (512 units) with ReLU activation

Dropout (50%) for regularization

Final softmax layer for multi-class classification

**Training Strategy:**

Categorical cross-entropy loss function

Adam optimizer

Batch size of 32

Early stopping to prevent overfitting

Model checkpoint to save the best model

30 epochs maximum with early stopping

**Evaluation Metrics:**

Accuracy: Overall correctness of predictions

Precision: Ratio of true positives to all positive predictions

Recall: Ratio of true positives to all actual positives

F1 Score: Harmonic mean of precision and recall

ROC-AUC: Area under the Receiver Operating Characteristic curve

Confusion Matrix: Detailed breakdown of correct and incorrect classifications

**Visualization:**

Original and augmented images

Training and validation accuracy/loss curves

Sample predictions with correct/incorrect labels

Confusion matrix heatmap
