
# 🚀 SpaceX Falcon 9 Landing Success Prediction

This repository contains a comprehensive **data science and machine learning project** focused on predicting the success of **Falcon 9 first-stage landings** using historical launch data from the SpaceX API.

---

## 📌 Project Overview

SpaceX has revolutionized the aerospace industry by **reusing rocket first stages**, significantly reducing launch costs approximately **$62 million per launch**, compared to **$165+ million** for traditional launch providers.

Accurately predicting whether a Falcon 9 first stage will land successfully is crucial for:

* Estimating launch costs
* Assessing mission risk
* Evaluating competitiveness in the commercial launch market

This project applies **data analysis and machine learning** to model and predict landing success.

---

## 🎯 Project Objectives

* **Data Acquisition**
  Collect historical SpaceX launch data using multiple API endpoints.

* **Exploratory Data Analysis (EDA)**
  Identify relationships between launch parameters and landing success.

* **Predictive Modeling**
  Train and optimize classification models to predict landing outcomes.

* **Model Evaluation**
  Compare multiple machine learning algorithms and select the most reliable model.

---

## 🔍 Methodology

### 1. Data Collection & Wrangling

The dataset was constructed by querying several SpaceX API endpoints:

* **Rockets** – to determine booster versions
* **Launchpads** – to extract site names and geographic coordinates
* **Payloads** – to obtain payload mass and orbit information
* **Cores** – to identify reuse history, grid fins, landing legs, and landing outcomes

The data was cleaned, transformed, and merged into a single structured dataset suitable for analysis and modeling.

---


### 2. Exploratory Data Analysis (EDA)

Exploratory Data Analysis was performed using **SQL**, **Matplotlib**, and **Seaborn** to identify key factors influencing Falcon 9 landing success.

Key insights include:

* **Launch Sites:** Falcon 9 launches were conducted from three primary sites: **CCSFS SLC 40**, **KSC LC 39A**, and **VAFB SLC 4E**, with CCSFS SLC 40 being the most frequently used.

* **Landing Outcomes:** Successful landings (ASDS, RTLS, and Ocean) significantly outnumbered failures, indicating improved recovery reliability over time.

* **Failures by Site:** Most failed or missing landings occurred at CCSFS SLC 40, largely due to its higher launch volume.

* **Payload and Orbit Relationship:** Heavier payloads were associated with orbits such as **VLEO** and **Polar Orbits**, while **GTO** missions showed high launch frequency with moderate payload mass.

* **Launch Trends:** Falcon 9 launch activity increased steadily from **2010 to 2020**, reflecting SpaceX’s rapid operational growth.


---

### 3. Machine Learning Modeling

Four classification models were trained and optimized using **GridSearchCV**:

* **Logistic Regression**
  Selected for stability and strong regularization performance.

* **Support Vector Machine (SVM)**
  Used advanced kernels to capture complex decision boundaries.

* **Decision Tree**
  Provided high interpretability with competitive accuracy.

* **K-Nearest Neighbors (KNN)**
  Evaluated for pattern recognition based on proximity.

---

## 📊 Key Findings

* **Top Performing Models:**
  Logistic Regression, SVM, and Decision Tree all achieved **83.33% test accuracy**.

* **Selected Model:**
  **Logistic Regression** was chosen as the final model due to:

  * Strong generalization performance
  * High training accuracy
  * Simplicity and robustness

* **Key Insight:**
  Well-regularized, simpler models can achieve strong predictive performance when paired with effective feature engineering and preprocessing (e.g., standard scaling).

---

## 🛠 Technologies Used

* **Programming Language:** Python

* **Tools:**

  * Jupyter Notebook
  * SpaceX REST API

---

## ▶️ How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/spacex-prediction.git
```

### 2. Install Dependencies

```bash
pip install requests pandas numpy matplotlib seaborn scikit-learn prettytable

```

### 3. Run the Notebook

Open `SpaceX_Machine_Learning_Prediction.ipynb` in **Jupyter Notebook** or **Google Colab** and run all cells to reproduce the results.


## Author
Faisal Salama


---


