# Prosper Loan Data Exploration
### by Chinonso Okonkwo

## Domain
This analytics is focused on Loan/Lending Analytics.

## Objectives
1. Supplement statistics with visualizations to build understanding of data.
2. Choose appropriate plots, limits, transformations, and aesthetics to explore a dataset, allowing you to understand distributions of variables and relationships between features.
3. Use design principles to create effective visualizations for communicating findings to an audience.
4. Create Univariate, Bivariate and Multivariate plots to get understanding of data.
5. Generate at least 15 insights in exploration.

## Installation
The following libraries are used in this project:
1. NumPy
2. Pandas
3. Matplotlib
4. Seaborn

## Dataset

The dataset consists of information 114,000 rows of loan data, and 81 variables including Loan amount, Borrower Income( Stated Monthly Income), Debt-Income-Ratio, Loan Term, Prosper Score and many others. The dataset can be found [here](https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv), with feature documentation available [here](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0)


## Data Wrangling
1. A subset of dataframe was created with 20 columns.
2. Dataframe was assessed for Data Quality and Tidiness Issues.
2. Rows with missing Prosper Score were dropped.
3. Categorical variables that are ordinal, are converted using pandas Categorical Dtype.
4. True in Is Borrower a Homeoner column, was replaced with HomeOWner and False with, Not Homeowner.
74,035 Prosper Loan listings information remained in the dataset with 20 variable.


## Summary of Findings
In the exploration process, I found that there was a Positive Relationship/Correlation 
between Loan Amount and Borrower's Monthly Income. I discovered that with borrowers 
with a relatively low Monthly Income, the probabilities of getting a Low or High 
Loan Amount is slightly similar. However, with a High Monthly Income, the Loan Amount received is Higher.

A strong relationship exists between the Monthly Payments and the Loan amount with 
modifying effect from the Loan Term. On encoding a bivariate plot, with a third variable Loan Term, the Visualization shows that Borrowers with longer Loan Term (36 or 60 months) receives larger Loan amounts.

There was also an interesting relationship between Loan Amount and the Categorical features. 
More Loans are associated with Borrowers with a Longer loan Term, Low risk involved
(high Prosper Score), Owning a Home and being successfully employed.



## Key Insights for Presentation

For the presentation, I focus on the influence of the Borrowers Income (Stated Monthly Income), Monthly Loan Payment, Loan term, Debt to Income ratio on Loan Amount and leave out most of the intermediate derivations. I start by intoducing the Loan Amount variable, followed by the distributions of the other variables, then I plot scatter plots showing correlations.

Scatter plots showing the correlation between Loan Amount and Predictor variable, Stated Monthly income was plotted. The plot showed that When a borrower has relatively low Monthly Income (<8,000 dollars) the probabilities of getting low and high Loan Amount are similar. However, when the borrower’s Monthly Income is high (>8,000 dollars), he/she is more likely to get a Large Loan Amount.

Then, I delved further creating multivariate scatter and point plots, to show that Loan Term plays a part in determining the amount of loan to be given out. It is also influenced by the Prosper score (risk score).That is, The Longer the Loan Term, and the better the risk score(Prosper Score), the larger the Loan Amount to be given out. This could be because Lenders are more open to giving out loans to borrowers who they don't assess as risks(for defaulting), and providing a long term to pay back the large Loan amount as an assurance.

