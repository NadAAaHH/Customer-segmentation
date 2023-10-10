<img src="https://www.gsam.com/content/gsam/base/en/market-insights/gsam-insights/quantinomics/credit-card-data/_jcr_content/main_content_top_par/public/main_content_top_par/background_e265/background/image_fb85.img.gif/1518447836002.gif" alt="drawing" width="200"/>

# Customer Segmentation: Can credit card habits be used to better understand the customers?


### What's the Problem & Why it's Important?
Segmenting customers is essential for businesses to understand their customers' unique needs and preferences. By grouping customers into segments based on shared characteristics, businesses can develop personalized marketing campaigns, products, and services that are more likely to resonate with each group.  

### What's the Goal of This Project?
This project aims to develop a predictive model that can determine which employees are most likely to leave based on various information about the employee's personal and professional history.

&nbsp;

# Dataset Analysis
#### Data
* **Source:** [Credit Card Dataset for Clustering](https://www.kaggle.com/datasets/arjunbhasin2013/ccdata)
* **Dataset Structure:** 8950 samples (rows), 18 features (variables)
* **Data Types:** 1 categorical, 17 numeric
* **Missing cells:** 314
* **Missing cells (%):**	0.2%
* **Total size in memory:**	1.7 MiB
* **Average record size in memory:**	199.0 B

&nbsp;
### Exploratory Data Analysis
Based on the above findings, the following factors were found to have the most impact on employee attrition:
1. Newly recruited employees 
2. At late 20's and early 30's 
3. Living far from work 

&nbsp;
# Model Development
Since this is an **unsupervised clustering problem** , the K-means to cluster
  
&nbsp;
### Evaluation
To evaluate the models performance, the following measurements were used:
* Confusion matrix
* Precision
* Recall
* Accuracy

&nbsp;
### Performance

| Model | Accuracy    | Precision    | Recall    |
| :---:   | :---: | :---: | :---: |
| Neural Network | 87.96 %   | --   | --   |
| Random Forest | 86.68 %   | --   | --   |
| Logistic Regression | 75.54 %   | --   | --   |

&nbsp;
# Conclusion
After conducting the results of the models, we can conclude the top Reasons why employees leave the organization:
* No Overtime: This was a surpirse, employees who don't have overtime are most likely to leave the organization. This could be that employees would like to have a higher amount of income or employees could feel that they are underused.
* Monthly Income: As expected, Income is a huge factor as why employees leave the organization in search for a better salary.
* Age: This could also be expected, since people who are aiming to retire will leave the organization.
  
Knowing the most likely reasons why employees leave the organization, can help the organization take action and reduce the level of Attrition inside the organization.



