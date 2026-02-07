## Alzheimer's Disease Image Classification (Deep Learning)

### Project Overveiw


Alzheimer’s Disease (AD) is a progressive neurological disorder that affects memory, thinking, and behavior. Early and accurate classification of Alzheimer’s stages can significantly improve diagnosis and treatment planning.

This project applies Deep Learning and Transfer Learning techniques to classify brain MRI images into different stages of Alzheimer’s Disease using a ResNet50 model.

The work was carried out using Kaggle Notebooks with GPU acceleration and focuses on building a memory-efficient, scalable image classification pipeline.

## Objectives
. Perform image preprocessing and exploratory data analysis
. Handle large image datasets edfficiently on kaggle
. Apply a Transfer Lerarning (ResNet50) for feature extraction 
. Build a robust multi class image classifier
. Evaluate model performance using standard metrics 
. Demostrate best practice for healthcare ML workflows

 ## Dataset
 Source: Kaggle- Alzheimer's Multiclass Dataset (Augmented)

 ### Classes:
 . NonDemented
 . VeryMildDemented
 . MildDemented
 . ModerateDemented

 ### Directory Structure:
 alzheimer's multiclass dataset-equal-and-augumented/


## Tools and Technologies
. Python
. TensorFlow / Keras
. Numpy 
. Matplotlib, Seaborn
. Sciokit-Learn
. Kaggle GPU (Tesla P100)
. Streamlit


## Methodology
1. Data Loading  (Memory Efficient)
Instead of loading all images into RAM (which causes kernel crashes), images are:
. Loaded by file path
. Processed on the fly using tf.data.Dataset
This approach prevent memory overflow and improves performance.

2. Image Preprocessing
. Resize image to 224 * 224
. Normalize pixel values
. Apply ResNet50 preprocessing


3. Feature Extraction 
. Used ResNet50 pretrained on ImageNet
. Removed top classification layers
. Extracted deep features using global average pooling
. Froze ResNet weights to prevent overfitting

4. Model Training
. Dense neural network built on extracted features
. Optimizer: Adam
. Loss function: Categorical Crossentropy
. Batch size carefully chosen to avoid GPU memory errors

5. Evaluation
. Accuracy
. Confusion Matrix
. Classification Report (Precision, Recall, F1-Score)


### Model Performance
. Accuracy: 89%
. Precission: High
. Recall: High
. F1-Score: High
The model demostrates strong predictive performance and  generalization capability.

Author: Khadijat Abubakar




 
