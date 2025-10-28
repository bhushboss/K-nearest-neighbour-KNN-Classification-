# K-nearest-neighbour-KNN-Classification-
 K-Nearest Neighbors (KNN) Classification Objective: Understand and implement KNN for classification problems. Tools: Scikit-learn, Pandas, Matplotlib
# K-Nearest Neighbors (KNN) Classification on the Iris Dataset

This project is a complete walkthrough of the K-Nearest Neighbors (KNN) algorithm for classification, implemented in Python. The model is trained on the classic Iris dataset to classify flowers into one of three species (Setosa, Versicolor, or Virginica) based on their sepal and petal measurements.

## 🎯 Objective

The guide follows five main objectives:
1.  Load and normalize a classification dataset.
2.  Implement the `KNeighborsClassifier` from Scikit-learn.
3.  Experiment with different values of K to find an optimal number.
4.  Evaluate the final model using accuracy and a confusion matrix.
5.  Visualize the resulting decision boundaries.

## 🧰 Tools and Libraries

* **Python 3**
* **Pandas:** For loading and managing the data.
* **Scikit-learn (sklearn):** For the `KNeighborsClassifier`, `StandardScaler`, `train_test_split`, and evaluation metrics.
* **Matplotlib & Seaborn:** For creating all visualizations.

## 📂 Dataset

The project uses the `Iris.csv` file, which contains 150 samples with 4 features each:
* `SepalLengthCm`
* `SepalWidthCm`
* `PetalLengthCm`
* `PetalWidthCm`

The target variable, `Species`, is categorical with three unique values: `Iris-setosa`, `Iris-versicolor`, and `Iris-virginica`.

## 🚀 How to Run

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/your-repository-name.git](https://github.com/your-username/your-repository-name.git)
    cd your-repository-name
    ```

2.  **Create and install requirements:**
    It's highly recommended to use a virtual environment.

    Create a `requirements.txt` file with the following content:
    ```
    pandas
    scikit-learn
    matplotlib
    seaborn
    ```
    
    Then, install the packages:
    ```bash
    pip install -r requirements.txt
    ```

3.  **Run the script:**
    If you named your script `knn_iris.py`, run:
    ```bash
    python knn_iris.py
    ```

## 📊 Results

Running the script will print the model's accuracy and classification report to the console. It will also generate and save the following three images:

### 1. K-Value vs. Accuracy
This plot helps determine the optimal value for K by showing the test accuracy for K values from 1 to 20.

![Accuracy vs. K Value](knn_accuracy_plot.png)

### 2. Confusion Matrix
This heatmap shows the performance of the final model (e.g., with K=7) on the test data.

![Confusion Matrix](confusion_matrix.png)

### 3. Decision Boundaries
This 2D plot visualizes the regions the model assigns to each class, based on Petal Length and Petal Width.

![Decision Boundaries](decision_boundaries.png)
