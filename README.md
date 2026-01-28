## PROJECT OVERVIEW

This project analyzes sales performance and discount strategies in a retail Superstore dataset,
with the objective of **increasing product consumption and sales volume while maintaining positive profitability**. 

The analysis includes **exploratory data analysis (EDA), machine learning (CatBoostRegressor) and statiscal hypothesis testing** to derive business insights.


## BUSINESS OBJECTIVE

Given the business's need to:

- Reach more customers
- Increase sales volume and product consumption
- Maintain a positive profit rate

This project aims to identify **which factors drive sales** and how **discount strategies** can be optimized across product sub-categories to achieve these gooals.


## KEY STEPS

***1. Data Quality Assessment & EDA***
- Assessed missing values, data consistency and outliers
- Analyzed distributions and skewness
- Visualized trends and patterns across products, sales and customer profiles to establish the initial understanding of business dynamics

***2. Machine Learning***

- **Outliers handling**: quantile-based clipping is intentionally kept minimal to preserve informative business signals, even at the expense of model performance gains
- **Tuned hyperparameters** using Optuna
- Estimated the relative **importance of features** to identify key contributors to sales, highlighting the role of product-related features and discount rates

***3. Discount and Quantity Interaction Analysis***

- Conducted sub-category-level **comparisons** between discounted and non-discounted orders
- Analyzed **purchase quantity** across different **discount ranges**
- Applied **Mann–Whitney U test** to validate whether observed differences are statistically significant

***4. Findings***

- Phones:
  + Statistically significant increase in quality under **15-20% discount**
  + **61%** increase in quantity sold
  + **17%** increase in large orders (orders with more than 4 units)

- Chairs and Binders:
  + Higher purchase quantities are observed
  + No statistically significant evidence 

***5. Recommendations***
 - Promote **a 15-20% discount strategy** for Phones
 - Adopt **a controlled experimental approach** for Chairs and Binders before a large-scale discount deployment


## TOOLS
- Python (Pandas, Scikit-learn, Optuna, Plotly,...)
- Jupyter Notebook

## DATA

Kaggle: vivek468/superstore-dataset-final





