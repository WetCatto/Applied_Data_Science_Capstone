# SpaceX Falcon 9 First Stage Landing Prediction

![Project Status](https://img.shields.io/badge/Status-Completed-success)
![Python](https://img.shields.io/badge/Python-3.x-blue)

## 📄 Project Overview
This repository contains the Capstone Project for the **IBM Data Science Professional Certificate**. 

The goal of this project is to predict whether the Falcon 9 first stage will land successfully. SpaceX advertises Falcon 9 rocket launches on its website with a cost of 62 million dollars; other providers cost upward of 165 million dollars. A significant amount of the savings is due to SpaceX's ability to reuse the first stage. Therefore, if we can determine if the first stage will land, we can determine the cost of a launch.

## ❓ Problem Statement
Build a machine learning pipeline to predict if the Falcon 9 Space X first stage will land successfully.

## 📂 Repository Structure

The project follows the standard data science methodology:

| File Name | Description |
| :--- | :--- |
| **Data Collection API.ipynb** | Collected data from the SpaceX API (Request/Response). |
| **Data Collection Web_Scrapping.ipynb** | Scraped Falcon 9 launch data from Wikipedia (BeautifulSoup). |
| **Data Wrangling.ipynb** | Cleaned the dataset, handled missing values, and formatted dates. |
| **EDA SQL.ipynb** | Performed Exploratory Data Analysis using SQL queries. |
| **EDA Data Viz.ipynb** | Visualized relationships between variables using Matplotlib and Seaborn. |
| **Interactive Visual Analytics - Folium.ipynb** | Created interactive maps to visualize launch sites and success rates. |
| **Interactive Visual Analytics - Plotly.py** | Built a Dashboard application using Plotly Dash. |
| **Machine Learning Prediction.ipynb** | Built and tuned classification models (Logistic Regression, SVM, Decision Tree, KNN). |

## 📊 Methodology

1.  **Data Collection:** Used the SpaceX REST API and web scraping to gather launch data.
2.  **Data Wrangling:** Filtered for Falcon 9 launches, handled missing payloads and landing details, and created class labels (1 for success, 0 for failure).
3.  **Exploratory Data Analysis (EDA):** Used SQL and visualizations to understand launch trends, success rates by site, and payload mass effects.
4.  **Interactive Visual Analytics:**
    * Used **Folium** to map launch sites and visualize success/fail clusters.
    * Used **Plotly Dash** to create a dynamic dashboard for user interaction.
5.  **Predictive Analysis:**
    * Standardized the data.
    * Split into training and testing sets.
    * Tuned hyperparameters using GridSearchCV.
    * Compared model accuracy.

## 📈 Results

* **Best Performing Model:** [Insert Model Name, e.g., Decision Tree Classifier]
* **Accuracy Score:** [Insert Score, e.g., 83.33%]
* **Key Insight:** [Insert a quick sentence, e.g., "Launch success has improved significantly over time, and heavier payloads do not necessarily correlate with failure."]

*(Optional: Add a screenshot of your best Confusion Matrix or your Dash App here)*

## 🛠 Technologies Used
* **Languages:** Python, SQL
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Folium, Plotly Dash, BeautifulSoup, Requests.

## 📜 Credits
This project was completed as part of the [IBM Data Science Professional Certificate](https://www.coursera.org/professional-certificates/ibm-data-science) on Coursera.
