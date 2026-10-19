# 🌸 Iris Flower Classification using Machine Learning

## 📌 Project Overview

This project classifies Iris flowers into three species using machine learning classification algorithms. It uses flower measurements such as sepal length, sepal width, petal length, and petal width to predict the species.

Three classification algorithms are implemented and compared:

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Gaussian Naive Bayes

## 🎯 Objectives

- Understand a classification problem using the Iris dataset.
- Perform label encoding on categorical target values.
- Split data into training and testing sets.
- Train multiple machine learning models.
- Evaluate model performance using accuracy, confusion matrices, and classification reports.

## 📂 Dataset

The dataset contains **150 records and 6 columns**.

| Column | Description |
|---|---|
| `Id` | Unique record identifier |
| `SepalLengthCm` | Sepal length in centimeters |
| `SepalWidthCm` | Sepal width in centimeters |
| `PetalLengthCm` | Petal length in centimeters |
| `PetalWidthCm` | Petal width in centimeters |
| `Species` | Iris flower species |

The target contains three species:

- Iris-setosa
- Iris-versicolor
- Iris-virginica

## 🛠️ Technologies Used

- Python
- Pandas
- Scikit-learn
- Jupyter Notebook

## 🤖 Machine Learning Algorithms

### 1. Logistic Regression
A classification algorithm used to predict the flower species from its measurements.

### 2. K-Nearest Neighbors (KNN)
A distance-based algorithm that classifies a flower based on the nearest observations. The notebook uses `n_neighbors=5`.

### 3. Gaussian Naive Bayes
A probabilistic classification algorithm based on Bayes' theorem, assuming features follow Gaussian distributions within each class.

## ⚙️ Project Workflow

1. Load the Iris dataset using Pandas.
2. Inspect and sample the data.
3. Convert species names into numeric labels using `LabelEncoder`.
4. Separate features (`X`) and target (`y`).
5. Split the data into training and testing sets.
6. Train Logistic Regression, KNN, and Gaussian Naive Bayes models.
7. Evaluate the models using accuracy, confusion matrices, and classification reports.

## 📊 Model Configuration

The notebook uses the following settings:

- **Test size:** 50%
- **Random state:** 42
- **Logistic Regression:** `max_iter=1000`
- **KNN:** `n_neighbors=5`
- **Naive Bayes:** `GaussianNB()`

## 📈 Results

Using the notebook's train-test split and evaluating the fitted models on the held-out test set:

| Algorithm | Test Accuracy |
|---|---:|
| Logistic Regression | 100% |
| K-Nearest Neighbors (KNN) | 100% |
| Gaussian Naive Bayes | 100% |

**Note:** These results are specific to the current split. The notebook also evaluates predictions on the complete dataset, including training observations, which can overstate generalization performance. For a fair comparison, evaluate on `X_test` and `y_test` only.

## 📁 Project Structure

```text
Iris-Flower-Classification/
├── iris_flower(1).ipynb
├── Iris(1).csv
└── README.md
```

## 🚀 How to Run the Project

### 1. Install Dependencies

```bash
pip install pandas scikit-learn jupyter
```

### 2. Open Jupyter Notebook

```bash
jupyter notebook
```

### 3. Open the Notebook

Open `iris_flower(1).ipynb` and run the cells sequentially.

**Important:** The notebook currently loads `iris.csv`. If you keep the uploaded dataset filename, update the loading statement to:

```python
df = pd.read_csv("Iris(1).csv")
```

## 📚 Learning Outcomes

- Data loading and exploration with Pandas
- Label encoding
- Train-test splitting
- Supervised machine learning classification
- Logistic Regression, KNN, and Naive Bayes
- Model evaluation and comparison

## ⚠️ Disclaimer

This project is intended for educational purposes and machine learning practice.

## 👨‍💻 Author

**Sohrab Ahmad Siddiqui**  
B.Tech Graduate — Computer Science Engineering (AI & ML)
