# Task-3: Cats vs. Dogs Image Classification with SVM

### 🎯 Objective
The goal of this project is to develop a machine learning model that can accurately classify images as either cats or dogs. 
***

### 📚 Dataset
The dataset used for this project is the **Microsoft Cats vs Dogs Dataset** from Kaggle, downloaded directly within the notebook using `kagglehub`.
* **Source:** [https://www.kaggle.com/datasets/shaunthesheep/microsoft-catsvsdogs-dataset](https://www.kaggle.com/datasets/shaunthesheep/microsoft-catsvsdogs-dataset)

***

### 🛠️ Methodology
1.  **Data Preprocessing:** Images are loaded, resized to 224x224 pixels, and preprocessed according to the requirements of the VGG16 model.
2.  **Feature Extraction:** Instead of using raw pixel values, **transfer learning** is employed. A pre-trained **VGG16 model** is used as a feature extractor. The top classification layers are removed, and the model's bottleneck features are used as input for the classifier.
3.  **Model Training:** The extracted features are then used to train a **Support Vector Machine (SVM)** classifier. The SVM is configured with a Radial Basis Function (RBF) kernel and a class-weighting parameter to handle any potential data imbalance.
4.  **Evaluation:** The model's performance is evaluated using various metrics, including accuracy, a classification report, a confusion matrix, and the ROC AUC score.

***

### 💻 Technologies and Libraries
* **Python:** The core programming language.
* **Keras:** For loading and using the pre-trained VGG16 model.
* **KaggleHub:** For direct download of the dataset.
* **Scikit-learn:** For the SVM model, data splitting, scaling, and evaluation metrics.
* **NumPy:** For efficient numerical operations.
* **Matplotlib:** For visualizing the confusion matrix and ROC curve.
* **Joblib:** For saving the trained model and other artifacts.

***

### 📊 Model Performance
The model achieved excellent performance on the test set, demonstrating the effectiveness of using VGG16 for feature extraction in image classification.

* **Accuracy:** **98.22%**
* **ROC AUC Score:** **0.9978**

The confusion matrix shows a low number of misclassifications:
* **True Positives (Cat):** 2449
* **False Negatives (Dog predicted as Cat):** 36
* **False Positives (Cat predicted as Dog):** 53
* **True Negatives (Dog):** 2462

Visualizations of the **Confusion Matrix** and the **ROC Curve** are included in the notebook for a more comprehensive analysis of the model's performance.

***

### 💾 Saved Model
The trained SVM model, along with the Label Encoder and StandardScaler, are saved to a file named `cats_vs_dogs.joblib`. This allows the model to be loaded and used for new predictions without the need to retrain.


***

### 👩🏻‍💻Author
`Debaswini`

***
