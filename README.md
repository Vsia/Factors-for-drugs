# Factors-for-pharmaceutical-drugs
![1000001646](https://github.com/user-attachments/assets/edc8da91-b4cd-4fbb-82fb-4ebc8f474354)


**Motivation**
![motivation_vallesia_pierre_louis](https://github.com/user-attachments/assets/d4447f98-20bf-4539-b44e-46212ad0ac73)

The use of medication to diagnose, cure, treat or prevent diseases is something almost
certain that every person in their life will take part in, whether it be a prescription from a doctor
or over the counter. The pharmaceutical industry is one of the biggest industries in the world.
With the mass distribution of medicine this industry does daily, it is important that people choose
and take the correct form of medication. In this project, we will find which factors contribute
most to user satisfaction from drug performance. We chose The Drug Performance Evaluation
dataset to best help us complete our goal. With the results, we will be able to help the customers
understand which factors or information to look for that will result in higher customer
satisfaction when selecting medication. This can also highlight to the pharmaceutical businesses
which factors to include with their products when selling to consumers to achieve the highest
customer satisfaction possible

**Data Description**

The dataset is from Kaggle and was scrapped from WebMD.

**Basic Data Analysis and Model Diagostic**

The obvious outliers were the drugs over $5000. Those drugs were not removed as there are many patients whose medications costs are at those prices. For example, Paclitaxel-Protein Bound is used by breast and pancreatic cancer patients. At $10362.19 , the patients satisfaction are improtant. 
![vallesia_pierre_louis_outliers](https://github.com/user-attachments/assets/67f600ed-c222-494f-925c-d4e5f393db77)

To determine the remaining outliers, logistic regression was performed on the full model, along with Cook's distance. Cook's showed no outliers as the values were greater than one. 
![vallesia_pierre_louis_outliers_2](https://github.com/user-attachments/assets/a70bea1e-b82b-476d-95c4-49363f4f5a03)

When followed with the leverage and Jackknife residual, there were 34 observations that exceeded that value. Followed by correcelation plots that gace an idea on which variables could be removed. And a VIF test was performed showing no collinearity was violated. The outliers were not removed in the end. 


The model was transformed. After transformation, there was not much difference to justify the need. Therefore, it was ommited. 
![vallesia_pierre_louis_transformed modl](https://github.com/user-attachments/assets/17abc0b0-b875-495d-a059-5705a4d15dff)

To find the final model, backwards elimination was perfomed using F-Statistic and p-value. Through that, the final model was selected. 
![vallesia_pierre_louis_final_model](https://github.com/user-attachments/assets/e2a1db11-9191-492e-8617-2fae9cd4da49)

The full report is available here on [Github](https://github.com/Vsia/Factors-for-drugs/blob/main/Final_Project_Report_Group_14.pdf). 

The R markdown code is also included on [Github](https://github.com/Vsia/Factors-for-drugs/blob/main/factors_for_drugs_r_markdown.Rmd). 



