# Heart Disease Prediction

## Exercise Summary
Implements logistic regression for heart disease prediction: EDA, training/viz, reg, SageMaker deployment.

## Dataset Description
Kaggle Heart Disease (303 patients; features: Age 29-77, Chol 112-564 mg/dL, etc.; ~55% presence rate). Downloaded from https://www.kaggle.com/datasets/neurocipher/heartdisease.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

You need to have **Python 3.x** installed. The project relies on the following libraries:

*   **Pandas**: For data manipulation and CSV loading.
*   **NumPy**: For vectorization and mathematical operations.
*   **Matplotlib**: For Data Visualization.

```bash
pip install pandas numpy matplotlib
```

### Installing

1.  Clone the repository.
2.  Ensure `Heart_Disease_Prediction.csv` is in the same directory as the notebook.
3.  Open `heart_disease_lr_analysis.ipynb` in Jupyter Notebook or VS Code.

## Project Structure

The Jupyter Notebook (`heart_disease_lr_analysis.ipynb`) contains:

1.  **Step 1: Data Preparation**: Loads the dataset, performs EDA (Exploratory Data Analysis), splits the data (70/30), and normalizes features using Z-score.
2.  **Step 2: Logistic Regression**: Defines the `sigmoid` function, `compute_cost` (Binary Cross-Entropy), and the `gradient_descent` algorithm. It trains the model and outputs metrics (Accuracy, Precision, Recall, F1).
3.  **Step 3: Visualization**: Plots decision boundaries for specific feature pairs (e.g., Age vs. Cholesterol) to visualize how the model separates the classes.
4.  **Step 4: Regularization**: Implements L2 Regularization (Ridge) to prevent overfitting and tunes the regularization parameter $\lambda$.

**Evidence**:

AREP-LAB02/Images/Eda.png

AREP-LAB02/Images/Plot.png

AREP-LAB02/Images/Step2.png

AREP-LAB02/Images/2.1.png

AREP-LAB02/Images/3.1.png

AREP-LAB02/Images/3.2.png

AREP-LAB02/Images/3.3.png

AREP-LAB02/Images/4.png

**Inference Test**:
*   **Tested Input**: `Age=60, Chol=300`
*   **Output**: `Prob=0.68 (high risk)`

## Author

David Villadiego
