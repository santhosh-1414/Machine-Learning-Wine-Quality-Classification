

# Machine Learning: Wine Quality Classification

## Project Overview

This project focuses on identifying and classifying red wine quality using machine learning techniques. Two classification algorithms, Random Forest and K-Nearest Neighbors (KNN), are implemented and evaluated to identify the better-performing model.

The project also investigates class imbalance in the dataset and applies the Synthetic Minority Over-sampling Technique (SMOTE) to balance the training data and evaluate its effect on model performance.

## Academic Information

- **Course:** Machine Learning – Assignment 1
- **Institution:** Blekinge Institute of Technology (BTH)
- **Location:** Karlskrona, Sweden
- **Authors:**
  - Santhosh Birada
  - Ayyappa Mitta

## Dataset

The project uses the Red Wine Quality dataset from the UCI Machine Learning Repository.

Dataset: [UCI Wine Quality Dataset](https://archive.ics.uci.edu/dataset/186/wine+quality)

The dataset contains physicochemical properties of red wine samples and their corresponding quality scores.

The input features include:
- Fixed acidity
- Volatile acidity
- Citric acid
- Residual sugar
- Chlorides
- Free sulfur dioxide
- Total sulfur dioxide
- Density
- pH
- Sulphates
- Alcohol

**Target variable:** Wine quality.

## Technologies and Libraries

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Imbalanced-learn (SMOTE)

## Machine Learning Algorithms

Two classification algorithms were selected:

1. **Random Forest Classifier:** An ensemble learning algorithm that combines multiple decision trees to perform classification.
2. **K-Nearest Neighbors (KNN):** A distance-based classification algorithm that predicts classes based on the nearest training samples.

## Methodology

The project follows these steps:

1. **Data Inspection:** Examining the dataset, feature information, class distribution, and class imbalance.
2. **Data Splitting:** Dividing the dataset into training (80%) and testing (20%) sets.
3. **Data Scaling:** Applying StandardScaler to normalize the input features.
4. **Model Training and Validation:** Evaluating Random Forest and KNN using Repeated K-Fold Cross-Validation with 3 splits and 10 repeats.
5. **Model Selection:** Comparing the average accuracy and standard deviation to identify the best-performing classifier.
6. **Testing:** Training the selected classifier on the training set and evaluating it on unseen test data.
7. **Class Balancing:** Applying SMOTE to the training data to address class imbalance.
8. **Re-evaluation:** Repeating model validation and testing using the balanced training data.

## Cross-Validation Results

The following results were obtained from the original training dataset:

| Classifier | Mean Accuracy | Standard Deviation |
|---|---:|---:|
| Random Forest | 0.86 | 0.012 |
| K-Nearest Neighbors | 0.78 | 0.013 |

Random Forest achieved the highest mean accuracy among the two classifiers and was selected as the best-performing model.

*Note: These are the reported cross-validation results. Refer to the assignment report and notebook for the test-set evaluation and SMOTE experiments.*

## Repository Contents

| File | Description |
|---|---|
| `wine_quality_classification.ipynb` | Python implementation and experiments |
| `ML_Assign-1_Report.pdf` | Academic assignment report |
| `requirements.txt` | Required Python libraries |
| `README.md` | Project documentation |

## Installation and Execution

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/Machine-Learning-Wine-Quality-Classification.git
```

### 2. Navigate to the project directory

```bash
cd Machine-Learning-Wine-Quality-Classification
```

### 3. Install the dependencies

```bash
pip install -r requirements.txt
```

### 4. Download the dataset

Download the Red Wine Quality dataset from the UCI repository and place `winequality-red.csv` in the project directory.

### 5. Run the notebook

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open `wine_quality_classification.ipynb` and execute the cells sequentially.

## Conclusion

The project demonstrates the application of supervised machine learning techniques to wine quality classification. Random Forest performed better than KNN in the reported cross-validation experiments.

The project also explores how class imbalance can be addressed using SMOTE and how balancing the training data can influence classification performance.

---

## Authors

**Santhosh Birada**  
Master's in Computer Science  
Blekinge Institute of Technology, Sweden

**Ayyappa Mitta**  
Computer Science  
Blekinge Institute of Technology, Sweden
=======
# Machine-Learning-Wine-Quality-Classification
Wine quality classification using Random Forest, KNN and SMOTE with Python.
>>>>>>> 90633d5b4b6afe0ca934f097c9a914cccd6d2c6c
