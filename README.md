

## Exploratory Data Analysis (EDA)
EDA was performed to understand:

- Class distribution  
- Image dimensions and consistency  
- Potential class imbalance  

Key insights from EDA guided preprocessing decisions such as image resizing and normalization.

---

## Data Preprocessing
The following preprocessing steps were applied:

- Image resizing to **224 × 224**  
- Normalization of pixel values  
- Train-test split  
- Feature extraction using ResNet50  
- Machine learning classification using Random Forest  

These steps ensure compatibility with the model architecture and improve performance.



## Model Architecture

- **Base Model:** ResNet50 (pretrained on ImageNet)  
- **Approach:** Transfer Learning  
- **Input Shape:** (224, 224, 3)  
- **Optimizer:** Adam  
- **Loss Function:** Categorical Crossentropy  

ResNet50 was used as a feature extractor to leverage learned representations from large-scale image datasets.


## Model Performance

The trained model was evaluated using standard classification metrics:

- **Accuracy:** 89%  
- **Precision:** High  
- **Recall:** High  
- **F1-Score:** High  

The model demonstrates strong predictive performance and good generalization capability.


## Observations

- The model performs best in identifying **NonDemented** cases  
- Some misclassification occurs between **MildDemented** and **VeryMildDemented**, likely due to visual similarity  
- Overall, the model shows good generalization with minimal overfitting  


## Future Improvements

- Hyperparameter tuning  
- Use of more advanced architectures (e.g., EfficientNet)  
- Increase dataset size  
- Model deployment for real-time prediction  


##  Connect With Me

- LinkedIn: www.linkedin.com/in/khadijat-abubakar  
-  GitHub: https://github.com/your-username  
