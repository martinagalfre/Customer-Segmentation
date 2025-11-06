# Customer Segmentation

## Project Overview
A superstore is launching a new pastry section selling artisanal cakes, doughnuts, cookies, and other pastries. This project segments customers based on their purchasing behavior and demographics to identify target groups for **personalized marketing campaigns**, increasing engagement and sales.

## Dataset
The dataset contains 2,240 customer records with demographic and purchase information. Key features for this analysis include:
- `TotalChildren` (sum of kids and teens at home)
- `Marital_Status` (encoded as couples vs singles)
- `NumStorePurchases`
- `MntSweetProducts`

## Methods
1. **Data Cleaning & Feature Engineering**  
   - Removed missing values and outliers  
   - Combined `Kidhome` and `Teenhome` into `TotalChildren`  
   - Simplified `Marital_Status` into couples vs singles  

2. **Feature Scaling**  
   - Standardized features using `StandardScaler`

3. **Clustering**  
   - Applied KMeans  
   - Determined optimal number of clusters using the **Elbow Method** and **Silhouette Score**

4. **Visualization & Dimensionality Reduction**  
   - Used PCA to reduce dimensions for 2D and 3D cluster visualization  
   - Heatmap of cluster centers to interpret customer behavior

## Key Insights

* Focus marketing efforts on customers with **high sweet product spending** and **frequent store visits**.
* Use **personalized campaigns** for singles or those living alone, emphasizing indulgence and premium offerings.
* Promote **in-store combo deals or family-oriented offers** for couples and households with children.
* Allocate **broad awareness campaigns** for low-engagement customers rather than targeted ads.


**Takeaway:** Marketing should focus on clusters with higher sweet product spending and purchase frequency, using targeted campaigns tailored to family/living situation and buying behavior.
