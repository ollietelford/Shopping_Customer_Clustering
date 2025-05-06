# Shopping Customer Clustering
## 🎯 Objective
The goal of this project is to analyze customer shopping behavior and identify patterns that can support the marketing team in developing targeted strategies. By segmenting customers based on income, age, and spending habits using the KMeans clustering algorithm in Python, we can group customers into more manageable and actionable segments for marketing efforts.

-----
## 🔍 Dataset Overview
The dataset contains information on 200 customers, including their age, annual income, and spending score. There are no missing or null values.
From the exploratory data analysis (EDA), we observed:
- Age appears to have little influence on either spending score or annual income.
- Clear differences between genders emerge.
- Notably, distinct clusters are visible when comparing annual income with spending score.
<p align="center">
<img src="https://github.com/user-attachments/assets/692f993f-3f2a-4ae9-b114-a28498514253">

These observations are further supported by the correlation heatmap. Only age and spending score show any meaningful correlation. Additional insights could be gained by knowing the number and type of purchases—for example, younger customers may make fewer but more expensive purchases (e.g., a gaming console or a bicycle).
<p align="center">
<img src="https://github.com/user-attachments/assets/5ae059af-ebfa-41a5-a6e1-0aa65222f332">

-----
## 📊 Clustering
Customer clusters were identified to support more targeted marketing campaigns. To determine the optimal number of clusters, inertia scores were plotted using KMeans for 1 to 11 clusters. The "elbow point" on the graph was used to select the ideal number.
- 3 clusters emerged when considering annual income alone.
- 5 clusters were identified using bivariate clustering on annual income and spending score.
<p align="center">
<img src="https://github.com/user-attachments/assets/3e68c035-f3d1-47a4-b01b-89fee5e1debf" width=500 height=190>


<p align="center">
<img src="https://github.com/user-attachments/assets/58c86fe7-71dc-4bef-b181-97ed61b1e07b">

Further insights could be obtained by analyzing actual purchase data per customer to identify product preferences within each cluster. However, based on current clustering:
Clusters 0 (blue), 2 (green), and 3 (red) are the most viable for marketing focus:
- Clusters 0 and 3: High spending scores.
- Cluster 2: High income but low spending score—suggesting potential for conversion with targeted offers.

<p align="center">
<img src="https://github.com/user-attachments/assets/b6141e92-cbeb-4bbb-9b39-39b782d08cb4" width=400 height=270>

Gender Breakdown:
- Females dominate clusters 0 and 3 (high spenders).
- Males dominate cluster 2 (high income, low spending).

Cluster Summary Statistics
- Below is a breakdown of the mean values for each feature across the identified clusters:
<p align="center">
<img src="https://github.com/user-attachments/assets/0ce5791f-4d0f-40df-9ce5-7bce25f14a93" width=600 height=250>

-----
This dataset was taken from https://absentdata.com/data-analysis/where-to-find-data/


