# Prosper Loan Exploration
## by Dorothy Nguyen


## Dataset

> This project is conducted as a part of Udacity Data Analyst Nanodegree. The purpose of this project is to perform exploratory data analysis, then create a presentation with explanatory charts that conveys findings and insights from the data set provided.

> The studied data set contains 113,937 loans with 81 variables on each loan provided by Prosper Marketplace, California-based pioneering company in the peer-to-peer lending industry in the U.S. Since its establishment in 2005, Prosper has helped more than 1.3 million customers get access to over $21 billion in affordable loans ([source](https://www.prosper.com))

> The dataset can be found in the [here](https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv) with feature documentation available in this [data dictionary](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0) contains specific details on every single dataset's variable.

> In the preliminary wrangling, I transformed some variables into their proper data types, for example, Income Range and Prosper Rating (Alpha) being converted to be ordinal types since they have intrinsic ranking order in their natures. 

> Out of 81 columns, I selected about 15 columns that are relevant to this loan exploration project. These columns are related to loan interest rates, the amount of loan, loan status and the characteristics of the borrowers such as their incomes and credit scores. I am interested to discover what are the major features for predicting the borrower interest rate of loan. My presumption is that customer risk score and income will have the most significant influences on each loan interest rate.

## Summary of Findings

> Over the course of various level of explorations, I found out somewhat significant patterns and relationships between variable of interest and other features. First of all, the borrower annual interest rate took a normal distribution with the peak around 20% and is highly negatively correlated with Prosper score. This means the lower prosper score borrowers are assessed, the more expensive interest rate they are supposed to obtain for their loans.

> Secondly, the scatter plot strongly indicates that the relationship is approximately linearly negative between borrower APR and loan original amount when loan amount is transformed to be on a logarithmic scale. Prosper customers who get a bigger loan amount are associated with decreasing annual interest rate. This relationship was discovered further in the multivariate exploration with modifying effects from Prosper rating grades and monthly loan payment magnitudes given to the loan. The findings restated the clear interactions between loan amount and annual interest rate among customers across Proper rating and monthly payment.

> Additionally, the finding reveals that across all level of incomes, except for income range of 0, past due, chargedoff, and defaulted loans generally have higher interest rates. On the contrary, completed loans seem to be the ones that have the lowest interest rate in all income ranges.

> Furthermore, out of 21 listing categories, half of borrowers listed the purpose of their loan applications to be debt consolidation. Besides, cosmestic procedure and household expenses have experienced the most expensive loans on average. On the contrary, personal loan and not available categories seem to get cheaper borrowing rates. Other than that, listing category does not seem to deliver any clear trend or relationship to the numeric variable of interest. Hence, I rather not conducting any further analyses with this categorical variable.

> Ouf of the main variable of interest, I detected the noticeably positive relationships between loan original amount, monthly loan payment, and term. Mean of monthly loan payment increases gradually as loan original amount is getting more considerable. The monthly payment amount appears to be proportionally greater for the length of 3 years compared to that amount for the length of 5 years. 

## Key Insights for Presentation

> For the presentation, I dig into the influences of the original loan amount, monthly loan payment and the characteristics of the borrowers including their income ranges and credit scores on Borrower APR. I start with univariate exploration by introducing the Borrower APR variable, followed by the patterns in loan original amount and monthly loan payment distributions. Afterwards, the distributions of three categorical variables including loan status, income range and Prosper rating are plotted.

> To continue, I use the box plots to depict the interactions between Borrower APR and loan original amount across Income Range and Prosper Rating. The bivariate relationship between Borrower APR and loan original amount is mentioned afterwards using scatter plot. 

> Moving on with the multivariate exploration, I cover the relationship between Borrower APR and loan original amount across various magnitudes of Prosper rating grades and monthly loan payment quantities with strip plot and scatter plot respectively. The presentation is finished with the dodged point plot of income range and Borrower APR accross loan status.
