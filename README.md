<img src="https://taptapcredit.com/wp-content/uploads/2020/01/credit-card.gif" width="200"/>

# Customer Segmentation: Can We Create Effective Customer Segments by Analyzing Their Credit Card Habits?

### Table of Contents
1. [Problem Definition & Objectives](#header-1)
2. [Data Statistics & Exploratory Data Analysis (EDA)](#data)
3. [Model Development](#model-development)
4. [Cluster Analysis](#cluster-analysis)

&nbsp;
# <a id="header-1"></a> Problem Definition & Objectives
### What's the Problem & Why it's Important?
Understanding customers is essential for any business's success. Instead of using a cookie-cutter marketing strategy, segmenting customers into groups based on common characteristics enables marketers to gain in-depth insights, and develop personalized marketing such as campaigns, products, and offers that are relevant to each group. Rather than relying on assumptions about their preferences and needs.

&nbsp;
### What's the Goal of This Project?
This project aims to develop a clustering model that can divide customers into groups based on their regular pattern and behaviors associated with their credit cards usage.
   
&nbsp;
# Data
#### Data Statistics
* **Source:** [Credit Card Dataset for Clustering](https://www.kaggle.com/datasets/arjunbhasin2013/ccdata)
* **Dataset Structure:** 8950 samples (rows), 18 features (variables)
* **Data Types:** 1 categorical, 17 numeric
* **Missing cells:** 314
* **Missing cells (%):**	0.2%
* **Total size in memory:**	1.7 MiB
* **Average record size in memory:**	199.0 B


&nbsp;
### Exploratory Data Analysis (EDA) 

&nbsp;
#### **Purchases vs One-off Purchases**
<img src="Screenshots/PURCHASES vs ONEOFF_PURCHASES.png"/>

The plotted data points is forming an upward pattern from left to right, which refers to a high correlation between the two features as indicated by the heatmap. This correlation could imply that most purchases were one-off purchases.  
The distant datapoints may be due to the large number of outliers in the dataset or other factors.

&nbsp;
#### **Credit Limit vs Balance**
<img src="Screenshots/CREDIT_LIMIT vs BALANCE.png"/>

The scatter plot is somewhat forming an angeld triangle, where the hypotenuse of the triangle is hinting for a correlation between the two features.

&nbsp;
#### Balance vs Minimum Payments
<img src="Screenshots/BALANCE vs MINIMUM_PAYMENTS.png"/>
Typically, the `MINIMUM_PAYMENTS` is often depends on the current `BALANCE` amount. But it appears that there's a very low correlation between them. Again, it may be due to outliers or other factors.

&nbsp;
#### Features That Changes Over Time
<img src="Screenshots/Features That Changes Over Time.png"/>
In general, all the plotted features against `TENURE` have an upward trend. Indicating that they are increasing over time.

&nbsp;&nbsp;
# Model Development
Since this is an **unsupervised clustering problem** , a K-means model was developed for the clustering.

&nbsp;
### K-means
<img src="Screenshots/vlaue of k.png"/>
Based on the above figure, the elbow is located at **k=4**. Therefore, the model will be created with 4 clusters.

&nbsp;
<div style="display: flex;">
    <img src="Screenshots/Customer Segmentation Using K-Means Clustering.png" width="600" />
    <img src="Screenshots/Size of Clusters in Percentages.png" width="400" />
</div>

The above figures illustrates the clusters distribution in the scatter plot, and the size of clusters in percentages. As indicated by both figures, The clusters are very close in size, with the exception of **Cluster 4**, which is the smallest cluster.


&nbsp;
# Cluster Analysis
After conducting the results of the models, we can conclude the top Reasons why employees leave the organization:
* No Overtime: This was a surpirse, employees who don't have overtime are most likely to leave the organization. This could be that employees would like to have a higher amount of income or employees could feel that they are underused.
* Monthly Income: As expected, Income is a huge factor as why employees leave the organization in search for a better salary.
* Age: This could also be expected, since people who are aiming to retire will leave the organization.
  
Knowing the most likely reasons why employees leave the organization, can help the organization take action and reduce the level of Attrition inside the organization.
