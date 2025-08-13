# KNN Classification on Iris Dataset

## 📌 Overview
This project implements the **K-Nearest Neighbors (KNN)** algorithm on the classic **Iris flower dataset** to classify iris flowers into three species:
- Iris-setosa
- Iris-versicolor
- Iris-virginica

We test multiple values of **K** and evaluate model performance using accuracy, confusion matrix, and classification report.

---

## 📂 Dataset
We use the **`load_iris`** dataset from `sklearn.datasets`.

### Features:
- Sepal Length (cm)
- Sepal Width (cm)
- Petal Length (cm)
- Petal Width (cm)

### Target Classes:
- `0` → Iris-setosa
- `1` → Iris-versicolor
- `2` → Iris-virginica

---

## ⚙️ Requirements
Install required libraries:
```bash
pip install pandas matplotlib seaborn scikit-learn
---

## ⚙️ Steps Performed
1. **Data Loading & Preprocessing**  
   - Read the CSV file into a Pandas DataFrame.  
   - Removed unnecessary columns (`Id`).  

2. **Data Splitting**  
   - 70% training data, 30% testing data.  
   - Stratified split to preserve class distribution.  

3. **Model Training & Evaluation**  
   - Trained KNN models for different `k` values: **1, 3, 5, 7, 9**.  
   - Computed **accuracy** for each `k`.  
   - For `k=5`, generated the confusion matrix and classification report.  

4. **Visualization**  
   - Plotted accuracy vs k values.  
   - Created a pairplot to visualize feature relationships and class separation.  
   - Displayed heatmap for correlation between features.

---

## 📊 Results

### Accuracy for Different k Values
| k  | Accuracy |
|----|----------|
| 1  | 0.967    |
| 3  | 1.000    |
| 5  | 1.000    |
| 7  | 1.000    |
| 9  | 1.000    |
