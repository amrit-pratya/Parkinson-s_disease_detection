# Parkinson-s_disease_detection
# Parkinson's Disease Detection using Machine Learning  This project uses a machine learning model to predict whether a person has Parkinson's disease based on a range of vocal measurements. The model is built using a Support Vector Machine (SVM) algorithm and trained on the "Parkinson's Data Set" from Kaggle.

## Project Overview

The notebook `Parkinson's_disease_detection.ipynb` covers the complete machine learning workflow:

1.  **Data Loading:** Downloads and loads the dataset using the `kagglehub` library.
2.  **Data Preprocessing:**
    * Checks for missing values.
    * Separates features (X) and the target variable (Y). The target variable is `status`, where `1` indicates Parkinson's positive and `0` indicates negative.
3.  **Data Splitting:** Splits the data into training (80%) and testing (20%) sets.
4.  **Data Standardization:** Scales the feature data using `StandardScaler` to ensure all features contribute equally to the model.
5.  **Model Training:** Trains a Support Vector Machine (SVM) model with a linear kernel on the training data.
6.  **Model Evaluation:** Evaluates the model's performance by calculating the accuracy score on both the training and test data.
7.  **Predictive System:** Includes a function to take new, unseen data (as a tuple) and predict the outcome.

## Model & Results

* **Model:** Support Vector Machine (SVM) with a linear kernel (`sklearn.svm.SVC(kernel='linear')`)
* **Test Data Accuracy:** 87.18%

## Technologies Used

* Python
* NumPy
* Pandas
* Scikit-learn
* KaggleHub

## Dataset

The project uses the **Parkinson's Data Set** [available on Kaggle](https://www.kaggle.com/datasets/thecansin/parkinsons-data-set). The notebook automatically downloads this dataset using the `kagglehub` library.

The dataset consists of 23 features (e.g., `MDVP:Fo(Hz)`, `MDVP:Jitter(%)`, `HNR`, `PPE`) and one target column, `status`, which is the label for the prediction.

## How to Use

To run this project on your local machine, follow these steps:

### 1. Clone the Repository

```bash
git clone [https://github.com/your-username/your-repository-name.git](https://github.com/your-username/your-repository-name.git)
cd your-repository-name

# For Windows
python -m venv venv
venv\Scripts\activate

# For macOS/Linux
python3 -m venv venv
source venv/bin/activate

pip install numpy pandas scikit-learn kagglehub jupyter

**jupyter notebook "Parkinson's_disease_detection.ipynb"**
