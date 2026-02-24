# Customer Segmentation using Machine Learning

## Project Overview

This project applies **Machine Learning (K-Means Clustering)** to segment customers based on their demographic and purchasing behavior. The goal is to help businesses understand different customer groups and enable **targeted marketing, personalization, and business decision-making**.

The project also includes an **interactive Streamlit web app** where users can input customer details and predict their customer segment.

---

## Business Problem

Companies have large customer datasets but often lack clarity on:

* Who are the high-value customers?
* Which customers spend the most?
* Which customers are likely to respond to campaigns?

Customer segmentation helps answer these questions.

---

## Dataset

The dataset contains customer information such as:

* Age
* Income
* Education
* Marital Status
* Spending on different products
* Purchase behavior
* Website visits
* Campaign response

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Streamlit
* Joblib

---

## Project Workflow

### 1. Data Cleaning

* Removed missing values
* Converted date columns
* Created new features such as:

  * Age
  * Total Spending
  * Total Children
  * Customer Since

---

### 2. Exploratory Data Analysis (EDA)

Performed analysis using:

* Distribution plots
* Box plots
* Heatmaps
* Pivot tables
* Campaign analysis

Key insights:

* Income strongly affects spending
* Middle-age customers spend more
* Campaign acceptance varies across segments

---

### 3. Feature Engineering

Final features used for clustering:

* Age
* Income
* Total Spending
* NumWebPurchases
* NumStorePurchases
* NumWebVisitsMonth
* Recency

---

### 4. Feature Scaling

Used:

StandardScaler

to normalize the data.

---

### 5. Model Building

Algorithm used:

K-Means Clustering

Optimal clusters selected using:

Elbow Method

Final model:

6 Customer Segments

---

### 6. Visualization

Used PCA to visualize customer clusters:

* Clear separation between segments
* Easy to interpret clusters

---

### 7. Model Saving

Saved using:

* kmeans_model.pkl
* scaler.pkl

---

## Streamlit Web App

An interactive web application was built using Streamlit.

Users can:

* Enter customer details
* Predict customer segment instantly

---

## Project Structure

```
customer_segmentation

│
├── customer_segmentation.csv
├── segmentation.ipynb
├── segmentation.py
├── kmeans_model.pkl
├── scaler.pkl
├── README.md
```

---

## How to Run the Project

### Step 1: Clone repository

```
git clone https://github.com/yourusername/customer-segmentation.git
```

---

### Step 2: Install dependencies

```
pip install -r requirements.txt
```

or

```
pip install pandas numpy matplotlib seaborn scikit-learn streamlit joblib
```

---

### Step 3: Run Streamlit App

```
streamlit run segmentation.py
```

---

## Output

The app predicts:

Customer Segment (Cluster Number)

Example:

Cluster 0 – High Value Customers
Cluster 1 – Low Spending Customers
Cluster 2 – Frequent Buyers

---

## Business Impact

This project helps businesses:

* Identify high-value customers
* Improve marketing strategy
* Increase revenue
* Personalize customer experience

---

## Future Improvements

* Deploy on cloud (AWS / Streamlit Cloud)
* Add customer segment labels
* Use advanced clustering techniques
* Build dashboard

---

## Author

Priyam Dattagupta

Data Analyst | Machine Learning Enthusiast

---

## If you like this project, give it a star
