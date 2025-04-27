Name:-kajal Rajendra bhise

Task3:-Iris flower classification

This project creates a machine learning model to classify Iris flowers into three species — **Setosa**, **Versicolor**, and **Virginica** — on the basis of sepal and petal lengths.

We aim to have high accuracy for species identification via appropriate preprocessing, feature selection, and model performance.

---

## ???? Dataset

The dataset has 150 samples with 5 columns:

- **Sepal Length (cm)**
- **Sepal Width (cm)**
- **Petal Length (cm)**
- **Petal Width (cm)**
- **Species** (Target: Setosa, Versicolor, Virginica)

Data Source: 
(https://archive.ics.uci.edu/ml/datasets/iris)


##  Preprocessing Details

- **Data Cleaning**: No missing values or null entries were encountered.
- **Feature Selection**: All four features were utilized at the beginning.
- **Label Encoding**: Species were converted to integers with the help of `LabelEncoder`.
- **Data Splitting**:
  - **Training set**: 80%  
  - **Testing set**: 20%
- **Scaling**: Not performed, since Random Forest is based on trees and scaling is not necessary.

---

##  Model Selection

- Model Used: **Random Forest Classifier** (`sklearn.ensemble.RandomForestClassifier`)
- Why Random Forest?
  - Works well with small datasets
  - Avoids overfitting from a single Decision Tree
  - Estimates feature importance automatically

- **Hyperparameters** (default used):
  - `n_estimators = 100`
  - `max_depth = None`
  - `random_state = 42`

---

##  Evaluation Results

| Metric      | Score         |
|--------------|---------------|
| Accuracy    | 1.00 (100%)    |
| Precision   | 1.00           |
| Recall         | 1.00          |
| F1-Score       | 1.00          |

The model was **100% accurate** on the test set.

**Feature Importance:**
- Petal length and petal width were the top features.

---
##  How to Run

1. Clone the repository
```bash
   git clone https://github.com/your-username/iris-flower-classification.git
   cd iris-flower-classification
```


