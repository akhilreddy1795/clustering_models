# Data Science Clustering Models: project Overview
---
* performed **data cleaning** operation 
* Outlier and missing value treatments
* Finding no'of clusters using **Silhoutte Score** 
* Built model with both **K-means clustering and heirarchical clustering** and compared both the results

## Code and Resources Used
---
**Python Version:** 3.7
**Packages:** Pandas, numpy, sklearn, matplotlib, seaborn, sklearn, scipy

## Data Cleaning
---
* Data Quality checks on columns like `exports` and `imports`
* Rounding of the numbers to 2 decimal points for ease of analysis

## EDA
---
* Checking for missing values
* `Outlier identification and capping` the upper quartile to 99th percentile
* Univariate and bivariate analysis
<br>![clustering bar grapg github](https://user-images.githubusercontent.com/69252134/130758880-a99c3f7d-5b0e-4292-b486-6127bbdbde65.png)
* **burundi** has the **low income** as per primary analysis and can be a country in desire need of aid

## Model Building
---
* Before starting clustering the data first i have started with **hopkins score** to see the cluster tendensy
* Acheived result of **hopkins score:** **0.96**
* Scaled data by importing `StandardScalar` from **sklearn**

Started building the model with **K means clustering** and to determine no'of clusters i have used **Silhoutte Score** 
![silhoutte score clustering github](https://user-images.githubusercontent.com/69252134/130760602-80e62d28-782f-4e34-8cb5-ec026d4d3c84.png)
* From the above elbow curve i have concluded to use **k = 4** for my model

## Model Performance
---
* Plotted the clusters for **GDPP vs Child_mortality** and noted the cluters which have high mortality rate as these countries which needs immediate aid
* ![clustering git hub](https://user-images.githubusercontent.com/69252134/130761219-bf28abc7-96e4-4d78-8b7f-2341539dea4b.png)
* differentiated clusters based on `child_mortality, income, gdpp`
* ![clusters subplots github](https://user-images.githubusercontent.com/69252134/130761944-3841a0a3-9ec4-4dab-83b7-680341620244.png)
* **Cluster 3** having the list of countries which we need to focus on funding on priority.


