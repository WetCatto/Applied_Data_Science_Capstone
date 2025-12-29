# SpaceX Falcon 9 First Stage Landing Prediction

## Project Overview
This repository contains the Capstone Project for the **IBM Data Science Professional Certificate**. 

The goal of this project is to predict whether the Falcon 9 first stage will land successfully. SpaceX advertises Falcon 9 rocket launches on its website with a cost of 62 million dollars; other providers cost upward of 165 million dollars. A significant amount of the savings is due to SpaceX's ability to reuse the first stage. Therefore, if we can determine if the first stage will land, we can determine the cost of a launch.

## Problem Statement
Build a machine learning pipeline to predict if the Falcon 9 Space X first stage will land successfully.

## Repository Structure

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

## Methodology

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

## Results

* **Best Performing Model:** All models (Logistic Regression, SVM, Decision Tree, and KNN) performed similarly on the test set.
* **Accuracy Score:** 83.33%
* **Key Insight:** Launch success rates have improved significantly as the flight number increases. Additionally, specific orbits (ES-L1, GEO, HEO, SSO) have remarkably high success rates, while payload mass alone is not a strict indicator of failure.

## Technologies Used
* **Languages:** Python, SQL
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Folium, Plotly Dash, BeautifulSoup, Requests.
