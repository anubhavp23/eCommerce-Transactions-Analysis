# Data Science Project: Customer Insights and Segmentation

## Project Overview

This project analyzes eCommerce transaction data to provide actionable insights about customers. The main objectives are:
1. **Exploratory Data Analysis (EDA):** Extract meaningful insights from customer, product, and transaction data.
2. **Lookalike Model:** Recommend similar customers based on transaction and profile data.
3. **Customer Segmentation:** Use clustering techniques to identify distinct customer groups for targeted marketing.

---

## Deliverables
- **Clustering Report**: 
  - Number of Clusters: 4
  - Davies-Bouldin Index: 1.27
  - Other relevant clustering metrics and insights.
- **Lookalike Recommendations**: CSV file with top-3 similar customers for each user.
- **Visualization**: Plots and graphs for EDA and clustering analysis.

---

## Files
| File Name                  | Description                                           |
|----------------------------|-------------------------------------------------------|
| `Customers.csv`            | Contains customer information.                       |
| `Products.csv`             | Contains product details.                            |
| `Transactions.csv`         | Contains transaction history.                        |
| `Lookalike.csv`            | Lookalike model results with top-3 recommendations.  |
| `Customer_Segments.csv`    | Customer segmentation results.                       |
| `Clustering_Report.xlsx`   | Detailed clustering metrics and insights.            |

---

## Methodology
1. **Exploratory Data Analysis (EDA):**
   - Checked data quality and missing values.
   - Analyzed sales trends, product performance, and regional sales distribution.
   - Visualized key findings using matplotlib.

2. **Lookalike Model:**
   - Computed customer similarity using **cosine similarity**.
   - Features used: TotalValue, Quantity, and Region (one-hot encoded).

3. **Customer Segmentation:**
   - Performed clustering using **KMeans**.
   - Determined the optimal number of clusters using the **Elbow Method** and **Davies-Bouldin Index**.
   - Segmented customers into 4 groups based on transaction and profile data.

---

## Results
### EDA Insights
- **Top Products**: Product Activewear Smartwatch contributes the most to total sales.
- **Sales Trends**: Sales peak during the holiday season.
- **Regional Performance**: Region South America generates the highest revenue.

### Lookalike Model
- Successfully identified top-3 similar customers for each user using transaction and profile data.

### Customer Segmentation
- Cluster 1: High-value customers with high transaction volume.
- Cluster 2: Low-value customers with frequent purchases.
- Cluster 3: Mid-range customers with consistent buying patterns.
- Cluster 4: Customers from underperforming regions with low transactions.

---

## Dependencies
This project requires the following Python libraries:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
