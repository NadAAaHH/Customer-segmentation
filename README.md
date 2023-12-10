# `Customer Segmentation`: Can We Use Credit Card Habits to Create Effective Customer Segments?

<img src="https://i.ibb.co/BtFJ8LR/68747470733a2f2f7461707461706372656469742e636f6d2f77702d636f6e74656e742f75706c6f6164732f323032302f30.gif" width="200"/>

➽ Divide Customers into Segments with a Clustering Model.  

![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dwyl/imgup/ci.yml?label=build&style=flat-square&branch=main)
[![codecov.io](https://img.shields.io/codecov/c/github/dwyl/imgup/main.svg?style=flat-square)](https://codecov.io/github/dwyl/imgup?branch=main)
[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat-square)](https://github.com/dwyl/imgup/issues)
[![contributions welcome](https://img.shields.io/badge/feedback-welcome-brightgreen.svg?style=flat-square)](https://github.com/dwyl/app-mvp/issues)

&nbsp;
### Table of Contents
1. [Problem Definition & Objectives](#header-1)
2. [Data Statistics & Exploratory Data Analysis (EDA)](#data)
3. [Model Development](#model-development)
4. [Cluster Analysis](#cluster-analysis)

&nbsp;
# <a id="header-1"></a> Problem Definition & Objectives
### What's the Problem & Why is it Important?
Understanding customers is essential for any business's success. Instead of using a cookie-cutter marketing strategy, segmenting customers into groups based on common characteristics enables marketers to gain in-depth insights, and develop personalized marketing such as campaigns, products, and offers that are relevant to each group. Rather than relying on assumptions about their preferences and needs.

&nbsp;
### What's the Goal of This Project?
This project aims to develop a clustering model that can divide customers into segments based on their regular patterns and behaviors associated with their credit card usage, while also providing potential marketing strategies for each segment.
   
&nbsp;
# Data
### Data Statistics
* **Source:** [Credit Card Dataset for Clustering](https://www.kaggle.com/datasets/arjunbhasin2013/ccdata)
* **Dataset Structure:** 8950 samples (rows), 18 features (variables)
* **Data Types:** 1 categorical, 17 numeric
* **Missing cells:** 314
* **Missing cells (%):**	0.2%
* **Total size in memory:**	1.7 MiB
* **Average record size in memory:**	199.0 B


&nbsp;
### Exploratory Data Analysis (EDA) 

#### ➤ Purchases vs One-off Purchases
<img src="Screenshots/PURCHASES vs ONEOFF_PURCHASES.png"/>

The plotted data points is forming an upward pattern from left to right, which refers to a high correlation between the two features as indicated by the heatmap. This correlation could imply that most purchases were one-off purchases.  
The distant datapoints may be due to the large number of outliers in the dataset or other factors.

&nbsp;
#### ➤ Credit Limit vs Balance
<img src="Screenshots/CREDIT_LIMIT vs BALANCE.png"/>

The scatter plot is somewhat forming an angeld triangle, where the hypotenuse of the triangle is hinting for a correlation between the two features.

&nbsp;
#### ➤ Balance vs Minimum Payments
<img src="Screenshots/BALANCE vs MINIMUM_PAYMENTS.png"/>  
Typically, the <code>MINIMUM_PAYMENTS</code> is often depends on the current <code>BALANCE</code> amount. But it appears that there's a very low correlation between them. Again, it may be due to outliers or other factors.

&nbsp;
#### ➤ Features That Changes Over Time
<img src="Screenshots/Features That Changes Over Time.png"/>
In general, all the plotted features against <code>TENURE</code> have an upward trend. Indicating that they are increasing over time.

&nbsp;&nbsp;
# Model Development
Since this is an **unsupervised clustering problem** , a K-means model was developed for the clustering.

### K-means
<img src="Screenshots/vlaue of k.png"/>  
Based on the above figure, the elbow is located at <b>k=4</b> Therefore, the model will be created with 4 clusters.

&nbsp;
<div style="display: flex;">
    <img src="Screenshots/Customer Segmentation Using K-Means Clustering.png" width="600" />
    <img src="Screenshots/Size of Clusters in Percentages.png" width="400" />
</div>

The above figures illustrates the clusters distribution in the scatter plot, and the size of clusters in percentages. As indicated by both figures, The clusters are very close in size, with the exception of **Cluster 4**, which is the smallest cluster.


&nbsp;
# Cluster Analysis
After the examination of the clusters' statistical data and visualizations, the characteristics of each cluster were identified. The following section outlines each segment and potential marketing strategies for each one:

### ➤ Customers Who Prefer to Pay in Advance
1. Offer attractive discounts, incentives, or early access to the product to encourage customers to pay in advance. 
2. Build trust by highlighting your secure payment methods and privacy protections. 
3. If applicable, emphasize the advantages of outright ownership that come with making advance payments. This can be particularly effective for big-ticket items.
4. Reward loyal customers who consistently make upfront payments with exclusive benefits or discounts.

&nbsp;
### ➤ Customers Who Prefer to Pay in Installments
1. Highlight the convenience and flexibility of paying in installments.
2. Provide clear and transparent information about the terms and conditions of installment plans, including the total cost, interest rates, and payment schedule.
3. If applicable, offer competitive interest rates and terms.

&nbsp;
### ➤ Customers Who Prefer to Make One-Off Payments & Have High Balances
1. Highlight the exclusivity and quality of your product.
2. Create a VIP loyalty program that offer them exclusive discounts, promotions, and early access to new products.
3. If applicable, partner with luxury brands and retailers.
4. Invest in high-quality branding and marketing materials to convey a sense of luxury and sophistication.
5. If applicable, highlight how your product can be seen as an investment or a store of value. This is especially relevant for products like jewelry or art.

&nbsp;
### ➤ Low Spenders Customers
1. Offer discounts, promotions, and coupons to make your product even more affordable for low spenders.
2. Low spenders are careful about where they spend their money, so make sure to clearly communicate the value that your product brings to them.
3. If applicable, offer samples and free trials. This is a great way for low spenders to try your product before they buy it.
4. Run social media contests and giveaways. 
5. Offer referral bonuses to customers who refer their friends and family.

&nbsp;   
Overall, considering the different types of payments across segments, make sure that customers are aware of the payment options available. Highlight these options in your marketing materials, website, and checkout process.

Additionally, it might be effective to promote limited-time offers or exclusive discounts for each payment method to create a sense of urgency and encourage customers to act quickly. 

&nbsp;
#### &nbsp;&nbsp;&nbsp; ▶️ For more details, please check the notebook file [here](Customer_Segmentation.ipynb). 
 
&nbsp;

### ░░░░░  Thank you for your interest in this project! I hope you find it helpful😄 ░░░░░  

