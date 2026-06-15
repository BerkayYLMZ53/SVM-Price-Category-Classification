# 📱 Price Category Classification with Support Vector Machines (SVM)

This project is a multi-class classification study developed to analyze the technical specifications of devices/products and assign them to their respective **price categories (Low, Medium, High, Very High)**.

## 🎯 Project Objective
To examine the impact of hardware specifications (battery power, microprocessor, memory, RAM, etc.) on cost and market positioning, and to build an SVM model to estimate the price segment based on these features.

## 🛠️ Model Architecture and Hyperparameter Optimization
A **Scikit-Learn Pipeline** structure was implemented to maintain code quality and prevent data leakage:
* **Feature Scaling:** Since SVM algorithms are sensitive to the scale of input features when calculating margin boundaries, all data were normalized using `StandardScaler`.
* **Hyperparameter Tuning (GridSearchCV):** A grid search was performed to select the optimal regularization parameter (`C`) and the kernel function (such as radial basis function - RBF, linear, etc.).

## 📈 Performance Evaluation
The model's performance was analyzed using a detailed `classification_report`. Additionally, a confusion matrix was visualized using `ConfusionMatrixDisplay` with a green color palette to observe prediction distributions and potential misclassifications across price categories.

## 🚀 Running the Project Locally
```bash
git clone https://github.com/BerkayYLMZ5353/price-category-svm.git
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook SVM_Odev.ipynb
```
```
