# Unsupervised Customer Segmentation

This project performs unsupervised customer segmentation using various clustering techniques. The primary aim is to group customers into segments based on purchasing behavior to enable targeted marketing strategies.

## Findings
The clustering analysis identified 4 distinct customer segments:
1. **High-Value Customers**: These customers have a high frequency of purchases and high average order values.
2. **Occasional Shoppers**: Customers in this group make infrequent purchases but tend to buy high-ticket items when they do.
3. **Regular Buyers**: This segment consists of customers who buy consistently over time, with moderate order values.
4. **Bargain Hunters**: Customers looking for discounts, usually purchasing lower-ticket items.

## Metrics
- **Silhouette Score**: Measures how similar an object is to its own cluster compared to other clusters (average score: 0.58).
- **Inertia**: Sum of squared distances of samples to their closest cluster center (common value found: 2100).

## Libraries Used
- **NumPy**: For numerical calculations.
- **Pandas**: For data manipulation and analysis.
- **Scikit-learn**: For clustering algorithms and metrics.
- **Matplotlib** and **Seaborn**: For visualization of clusters and metrics.

## Code Outputs
- The clustering visualization shows distinct separations between customer segments:
  ![Clustering Output](outputs/clustering_visualization.png)

- Further analysis on metrics: 
```python
from sklearn.metrics import silhouette_score
silhouette_avg = silhouette_score(data, labels)
print("Silhouette Score: ", silhouette_avg)
```

## Conclusion
This project demonstrates how unsupervised learning techniques can effectively be leveraged for customer segmentation, providing insights into buying behaviors that can help businesses improve marketing strategies.