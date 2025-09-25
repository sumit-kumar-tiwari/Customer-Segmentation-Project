# Customer Segmentation using K-Means Clustering

## Project Overview

This project uses the K-Means clustering algorithm, a popular unsupervised machine learning technique, to segment customers of a retail mall. The goal is to group customers into distinct clusters based on their annual income and spending score. This analysis helps the business to understand its customer base better and create targeted marketing strategies for each segment.

---

## Dataset

The project utilizes the "Mall Customer Segmentation Data" dataset, which is publicly available on Kaggle.

The dataset contains the following columns:
* `CustomerID`: Unique ID for each customer.
* `Gender`: Gender of the customer.
* `Age`: Age of the customer.
* `Annual Income (k$)`: The annual income of the customer in thousands of dollars.
* `Spending Score (1-100)`: A score assigned by the mall based on customer behavior and spending nature (1 being the lowest, 100 being the highest).

For this clustering task, we primarily focus on the **`Annual Income`** and **`Spending Score`** features.

---

## Methodology

The project follows these key steps:
1.  **Data Loading:** The dataset is loaded using the pandas library.
2.  **Feature Selection:** `Annual Income` and `Spending Score` are selected as the features for clustering.
3.  **Finding Optimal Clusters:** The Elbow Method is used to determine the optimal number of clusters (K). The analysis showed that **K=5** is the ideal number of clusters for this dataset.
4.  **Model Training:** The K-Means algorithm is trained with K=5 to create the customer segments.
5.  **Visualization:** The final clusters are visualized using a scatter plot to understand the characteristics of each group.

---

## Customer Segments Identified

The analysis revealed 5 distinct customer segments:

* **Standard:** Customers with average income and average spending scores.
* **Target:** High-income customers who also have a high spending score. These are the most valuable customers.
* **Careless:** Low-income customers with high spending scores.
* **Careful/Thrifty:** High-income customers who spend very little.
* **Sensible:** Low-income customers who also have a low spending score.

*(Note: To display an image of your final plot, upload the screenshot to your GitHub repository and add a line like this: `![Customer Segments Plot](your_image_name.png)`)*

---

## How to Run This Project

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/sumit-kumar-tiwari/Customer-Segmentation-Project.git](https://github.com/sumit-kumar-tiwari/Customer-Segmentation-Project.git)
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd Customer-Segmentation-Project
    ```
3.  **Install the required libraries:**
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```
4.  **Run the Python script:**
    ```bash
    python customer_segmentation.py
    ```

---

## Libraries Used

* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
