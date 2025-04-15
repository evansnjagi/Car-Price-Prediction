# Car Price Prediction Model with MVP

This project focuses on building a car price prediction model using machine learning techniques, along with a Minimal Viable Product (MVP) to demonstrate the model’s performance. The workflow involves data wrangling, feature engineering, model building, and evaluation.

---

### Key Features of the Project:

#### 1. **Data Wrangling**:
   - **Preprocessing**: A custom `wrangle` function is implemented to clean and prepare the dataset for modeling. This includes:
     - Removing **outliers** to ensure data quality and prevent model distortion.
     - Dropping features with **low or high cardinality** that have little predictive power.
     - Eliminating **multicollinear features** to avoid redundant information that could lead to overfitting.
     - Discarding features that are **uncorrelated** with the target variable, **price**.

#### 2. **Data Splitting**:
   - The dataset is split into **training** and **testing** sets, ensuring the model's ability to generalize well on unseen data.

#### 3. **Machine Learning Pipeline**:
   - The model is built using a **machine learning pipeline** that includes:
     - **SimpleImputer**: Handles missing data by imputing values based on strategy (mean/median).
     - **Ridge Regression**: A regularized linear regression model that helps prevent overfitting.
     - **OneHotEncoder**: Converts categorical variables into numerical features to be used by the model.
   - The pipeline is **fit** on the training data, and predictions are made on the test data.

#### 4. **Model Evaluation**:
   - The model is evaluated using **accuracy** and other performance metrics such as **R²** and **Mean Squared Error (MSE)**:
     - **86% accuracy** on the training data.
     - **71% accuracy** on the test data.
   - These metrics help assess the model's predictive power and guide further improvements.

#### 5. **Feature Importance**:
   - A **feature importance plot** is created to visualize how each feature impacts the model's predictions, providing valuable insights into the dataset.

#### 6. **Minimal Viable Product (MVP)**:
   - A simple **MVP** is developed to demonstrate the car price prediction model in action. It allows users to input data and receive a car price prediction in real-time.
   
  - [![Watch the video](https://github.com/evansnjagi/Car-Price-Prediction/blob/Video-and-Pictures/WhatsApp%20Image%202025-04-15%20at%209.10.05%20AM.jpeg)](videos/demo.mp4)

---
### Technologies Used - Logos

<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/c/c3/Python-logo-notext.svg" alt="Python" width="50" height="50"/>
  <sub>Python</sub>
  &nbsp;&nbsp;&nbsp;&nbsp;

  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Pandas_logo.svg/512px-Pandas_logo.svg.png" alt="Pandas" width="50" height="50"/>
  <sub>Pandas</sub>
  &nbsp;&nbsp;&nbsp;&nbsp;

  <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg" alt="Scikit-learn" width="50" height="50"/>
  <sub>Scikit-learn</sub>
  &nbsp;&nbsp;&nbsp;&nbsp;

  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/31/NumPy_logo_2020.svg/1280px-NumPy_logo_2020.svg.png" alt="NumPy" width="50" height="50"/>
  <sub>NumPy</sub>
  &nbsp;&nbsp;&nbsp;&nbsp;

  <img src="https://th.bing.com/th/id/OIP.tjvlNzMv9E4Q364jkHGc_QHaBf?w=350&h=70&c=8&rs=1&qlt=90&o=6&pid=3.1&rm=2" alt="Matplotlib" width="50" height="50"/>
  <sub>Matplotlib</sub>
  &nbsp;&nbsp;&nbsp;&nbsp;

  <img src="https://th.bing.com/th/id/OIP.HVPhVIc7d6w0MLqWx3cmEgHaEK?w=333&h=187&c=8&rs=1&qlt=90&o=6&pid=3.1&rm=2" alt="Seaborn" width="50" height="50"/>
  <sub>Seaborn</sub>
  &nbsp;&nbsp;&nbsp;&nbsp;

  <img src="https://th.bing.com/th/id/OIP.9s5zkiCnpIWl_krakzzpCwHaEK?rs=1&pid=ImgDetMain" alt="Jupyter Notebook" width="50" height="50"/>
  <sub>Jupyter Notebook</sub>
</p>


### Repository Structure

The project repository is organized into the following key components:

```plaintext
/car-price-prediction
    ├── CarPriceModelling.ipynb    # Notebook where, Preprocessing, Modelling and Communication done
    ├── Video-and-Pictures         # Project Images and Video
    ├── Datasets                   # Dataset use in this project
