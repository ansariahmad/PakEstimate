# 🏘️ PakEstimate

## 📌 Project Overview

This project involves scraping house listings from [Zameen.com](https://www.zameen.com/) for four major cities in Pakistan — **Islamabad**, **Rawalpindi**, **Lahore**, and **Karachi** — and using this data to build predictive models for estimating house prices.

---

## 🗺️ Workflow

1. **Scraping Phase**

   * Visited [zameen.com](https://www.zameen.com/)
   * Selected city pages for **Islamabad**, **Rawalpindi**, **Lahore**, and **Karachi**
   * Scraped links to individual house listings
   * Stored links in Pickle format for reuse
   * Extracted detailed house data from each listing and saved it in a CSV file

2. **Data Preprocessing**

   * Removed **null values** and **duplicate records**
   * Detected and removed **outliers**
   * Performed **normality checks** using:

     * Shapiro-Wilk Test
     * Kolmogorov-Smirnov Test
     * D'Agostino's K-squared Test
   * Applied **one-hot encoding** for categorical features
   * Applied **log transformation** to reduce skewness in numeric features

3. **Modeling**

   * Trained the following regression models:

     * Linear Regression
     * Decision Tree Regressor
     * Random Forest Regressor
   * Evaluated models using **Adjusted R-Squared**
   * **Random Forest** performed best with an Adjusted R² score of **0.88**

4. **Model Interpretation**

   * Performed **Partial Dependence Plots (PDPs)** to interpret the impact of key features on the predicted house prices

---

## 🧰 Technologies Used

* **Python** (3.x)
* **BeautifulSoup** & **Requests** for web scraping
* **Pandas** & **NumPy** for data processing
* **Scikit-learn** for machine learning
* **Matplotlib** & **Seaborn** for data visualization
* **SciPy** & **Statsmodels** for statistical tests

---

---

## 📊 Results

* **Best Model:** Random Forest Regressor
* **Adjusted R² Score:** 0.88
* **Key Features Identified:** Location, Area, Number of Bedrooms, Price per Square Foot, etc.

---

## 📌 Future Work

* Incorporate **more cities** and historical pricing trends
* Deploy a **web application** for real-time price prediction
* Use **deep learning models** for image-based house feature extraction (optional)

---

## 🧠 Author

**Ahmad Talha Ansari**
