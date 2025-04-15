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
- The dataset is split into **training** and **testing** sets to evaluate model generalization.

### 3. ⚙️ **Machine Learning Pipeline**
The model is built using a **machine learning pipeline** that includes:
- `SimpleImputer` for handling missing values
- `OneHotEncoder` to convert categorical variables
- `Ridge Regression` as the main model to reduce overfitting

The pipeline is trained on the training data and tested on unseen data.

### 4. 📈 **Model Evaluation**
- **86% accuracy** on the training data
- **71% accuracy** on the test data
- Additional metrics include **R²** and **Mean Squared Error (MSE)**

These metrics help assess the model’s predictive power and guide improvements.

### 5. 📊 **Feature Importance**
A **feature importance plot** visualizes which features impact car prices most.

### 6. 🧪 **Minimal Viable Product (MVP)**
- A simple interface allows users to input data and receive **real-time predictions**.
- 🎬 **Watch the demo video** below:

[![Watch the demo](https://github.com/evansnjagi/Car-Price-Prediction/edit/Video-and-Pictures/Images/WhatsApp Image 2025-04-15 at 9.10.05 AM.jpeg)](https://vm.tiktok.com/ZMBgdSsnb/)


---

## 🧰 Technologies Used

| Tool             | Logo                                                                 |
|------------------|----------------------------------------------------------------------|
| Python           | ![Python](https://upload.wikimedia.org/wikipedia/commons/c/c3/Python-logo-notext.svg) |
| Pandas           | ![Pandas](https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Pandas_logo.svg/512px-Pandas_logo.svg.png) |
| Scikit-learn     | ![Scikit-learn](https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg) |
| NumPy            | ![NumPy](https://upload.wikimedia.org/wikipedia/commons/3/31/NumPy_logo_2020.svg) |
| Matplotlib       | ![Matplotlib](https://matplotlib.org/_static/images/logo2.svg) |
| Seaborn          | ![Seaborn](https://seaborn.pydata.org/_static/logo-wide-lightbg.svg) |
| Jupyter Notebook | ![Jupyter](https://jupyter.org/assets/homepage/main-logo.svg) |

---

## 📁 Repository Structure
```plaintext
Car-Price-Prediction/
│
├── CarPriceModel.ipynb         # Main Jupyter notebook for the model
├── Datasets/                   # Contains the raw dataset(s)
├── Videos/                     # Demo video and thumbnail
│   ├── demo.mp4                # MVP demonstration video
│   └── thumbnail.png           # Thumbnail used for the video link
└── Images/
