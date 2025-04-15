# 🚗 Car Price Prediction Model with MVP

This project focuses on building a car price prediction model using machine learning techniques, along with a Minimal Viable Product (MVP) to demonstrate the model’s performance. The workflow involves data wrangling, feature engineering, model building, and evaluation.

---

## 🔑 Key Features of the Project

### 1. 🧹 **Data Wrangling**
A custom `wrangle` function is implemented to clean and prepare the dataset for modeling. This includes:
- Removing **outliers** to ensure data quality and prevent model distortion.
- Dropping features with **low or high cardinality** that have little predictive power.
- Eliminating **multicollinear features** to avoid redundant information that could lead to overfitting.
- Discarding features that are **uncorrelated** with the target variable, **price**.

### 2. ✂️ **Data Splitting**
- The dataset is split into **training** and **testing** sets, ensuring the model's ability to generalize well on unseen data.

### 3. ⚙️ **Machine Learning Pipeline**
The model is built using a **machine learning pipeline** that includes:
- `SimpleImputer`: Handles missing data by imputing values based on strategy (mean/median).
- `Ridge Regression`: A regularized linear regression model that helps prevent overfitting.
- `OneHotEncoder`: Converts categorical variables into numerical features to be used by the model.

The pipeline is **fit** on the training data, and predictions are made on the test data.

### 4. 📈 **Model Evaluation**
The model is evaluated using key performance metrics:
- **86% accuracy** on the training data
- **71% accuracy** on the test data
- Additional metrics: **R²** and **Mean Squared Error (MSE)**

These metrics help assess the model's predictive power and guide further improvements.

### 5. 📊 **Feature Importance**
A **feature importance plot** is created to visualize how each feature impacts the model's predictions, providing valuable insights into the dataset.

### 6. 🧪 **Minimal Viable Product (MVP)**
A simple MVP is developed to demonstrate the car price prediction model in action:
- Users can input data and receive a car price prediction in real-time.
- 🎬 **You can watch the demo video below**:

[![Watch the video](videos/thumbnail.png)](videos/demo.mp4)

---

## 🧰 Technologies Used

| Technology        | Logo |
|-------------------|------|
| **Python**        | ![Python](https://upload.wikimedia.org/wikipedia/commons/c/c3/Python-logo-notext.svg) |
| **Pandas**        | ![Pandas](https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Pandas_logo.svg/512px-Pandas_logo.svg.png) |
| **Scikit-learn**  | ![Scikit-learn](https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg) |
| **NumPy**         | ![NumPy](https://upload.wikimedia.org/wikipedia/commons/3/31/NumPy_logo_2020.svg) |
| **Matplotlib**    | ![Matplotlib](https://matplotlib.org/_static/images/logo2.svg) |
| **Seaborn**       | ![Seaborn](https://seaborn.pydata.org/_static/logo-wide-lightbg.svg) |
| **Jupyter Notebook** | ![Jupyter](https://jupyter.org/assets/homepage/main-logo.svg) |

---

## 📁 Repository Structure
Car-Price-Prediction/
│
├── CarPriceModel.ipynb         # Main Jupyter notebook for the model
├── Datasets/                   # Contains the raw dataset(s)
├── Videos/                     # Demo video and thumbnail
│   ├── demo.mp4                # MVP demonstration video
│   └── thumbnail.png           # Thumbnail used for the video link
└── Images/                     # Feature importance plots and other visuals
