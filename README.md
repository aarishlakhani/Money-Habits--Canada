# Canadian Household Spending — Clustering, Dimensionality Reduction & Predictive Modeling

This repository focuses on studying Canadian households and their spending/saving habits.  
For this, two datasets have been provided by Environics Analytics:  
- Household spending per dissemination area  
- Demographic data per dissemination area  

The analysis is divided into two parts: **unsupervised learning** (clustering and dimensionality reduction), and **supervised learning** (regression).  

In the first part, we cleaned the data and used **K-means clustering** to recognize the distinct segments within the merged household spending and demographic dataset.  
The optimal number of clusters was determined using the **Elbow method** and the **Silhouette method**.  
To further explore the structure of the dataset, we implemented **Principal Component Analysis (PCA)** and **Uniform Manifold Approximation and Projection (UMAP)**.  

The second part focuses on developing models to predict a household’s **proportion of income spent on total personal insurance premiums and retirement/pension contributions**.  
We employed two predictive models: **Elastic Net linear regression** and **XGBoost**. Both models were evaluated in terms of **mean squared error (MSE)**, **R-squared (R²)**, and **bootstrapped confidence intervals**.  
XGBoost significantly outperformed Elastic Net.  

Finally, we applied **SHAP (Shapley Additive exPlanations)** values to identify the most important variables contributing to household spending behavior.  
