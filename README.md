---
### Table of Contents
1. [Define the Problem and Objectives](#what's-the-problem-&-why-it's-important?)
2. [Data Statistics & Exploratory Data Analysis (EDA)](#data)
3. [Model Development](#model-development)
4. [Cluster Analysis](#cluster-analysis)
---


<img src="https://taptapcredit.com/wp-content/uploads/2020/01/credit-card.gif" alt="drawing" width="200"/>

# Customer Segmentation: Can Analyzing Credit Card Habits Create an Effective Segmentation?

&nbsp;

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
Based on the above findings, the following factors were found to have the most impact on employee attrition:
1. Newly recruited employees 
2. At late 20's and early 30's 
3. Living far from work 

&nbsp;
# Model Development
Since this is an **unsupervised clustering problem** , a K-means model was developed for the clustering.

&nbsp;
# Cluster Analysis
After conducting the results of the models, we can conclude the top Reasons why employees leave the organization:
* No Overtime: This was a surpirse, employees who don't have overtime are most likely to leave the organization. This could be that employees would like to have a higher amount of income or employees could feel that they are underused.
* Monthly Income: As expected, Income is a huge factor as why employees leave the organization in search for a better salary.
* Age: This could also be expected, since people who are aiming to retire will leave the organization.
  
Knowing the most likely reasons why employees leave the organization, can help the organization take action and reduce the level of Attrition inside the organization.
