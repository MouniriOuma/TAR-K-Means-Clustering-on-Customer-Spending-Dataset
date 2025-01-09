# K-Means Clustering on Customer Spending Dataset

This project demonstrates the application of **K-Means Clustering** on a customer spending dataset to group customers based on their demographics and spending behavior. The dataset includes features such as age, gender, annual income, and spending score. The goal is to identify meaningful customer segments for targeted marketing strategies.


## 📁 Dataset

The dataset used in this project contains the following columns:

- **CustomerID**: Unique identifier for each customer.
- **Gender**: Gender of the customer (Male/Female).
- **Age**: Age of the customer.
- **Annual Income (k$)**: Annual income of the customer in thousands of dollars.
- **Spending Score (1-100)**: Spending score assigned to the customer (1 = low, 100 = high).

For this clustering task, we focus on the following features:
- `Age`: Customer age.
- `Gender`: Gender of the customer (converted to numerical values: 0 = Male, 1 = Female).
- `Annual Income (k$)`: Annual income.
- `Spending Score (1-100)`: Spending score.


## 🛠️ Code Overview

The code performs the following steps:

1. **Data Loading**:
   - The dataset is loaded from a CSV file (`spending_score_predict.csv`).

2. **Data Preprocessing**:
   - Relevant features (`Age`, `Gender`, `Annual Income (k$)`, `Spending Score (1-100)`) are selected.
   - The `Gender` column is converted to numerical values (0 for Male, 1 for Female).
   - The data is normalized using `StandardScaler` to ensure all features are on the same scale.

3. **K-Means Clustering**:
   - The K-Means algorithm is applied to the normalized data.
   - The number of clusters is set to 4 (`n_clusters=4`).

4. **Visualization**:
   - The clusters are visualized using a scatter plot matrix with `plotly.express`.
