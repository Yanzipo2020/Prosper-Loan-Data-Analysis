# Loan Data from Prosper
## by Yan Li


## Dataset

This project is on a data set from Prosper, which is America’s first marketplace lending platform, with over $23 billion in funded loans to more than 1,370,000 people. This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, borrower employment status, borrower credit history, and the latest payment information, etc. By investigating this dataset, I hope to answer these three questions:
1. Who borrow money through Prosper? Why do they want a loan?
2. What affects the borrower’s APR or interest rate?

## Summary of Findings

This notebook tries to answer the questions about who and why borrows through Prosper and what affect the borrowers' APR or interest rates.

In univariate exploration, we find out most borrowers' listings are under "Debt Consolidation" category whose number outweighs the sum of all other categories. This shows the borrowers have already got debts and Prosper can provide better APR than other loan companies. Top 5 occupations in the borrrowers are "Computer Programmer", "Executive", "Teacher", "Administrative Assistant", and "Analyst". The median of the borrowers' monthly income is 4667 dollars. And most borrowers' monthly loan payment is in the range between 150-175 dollars. Nearly half of all loans were in progress when Prosper Loan dataset was done. But in the loans which are finished, nearly 2/3 are completed. The failed loans (Changed Off, Defaulted, Past Due, Cancelled) account for 1/3 of all finished loans.

In bivariate exploration, we find monthly loan payment has strong correlation with loan's original amount. But the scatter plot of these features shows a few straight line patterns with different slopes. This has been explained by multivariate exploration and the different line patterns are caused by different length of the loan ("Term" feature).

We also find the borrowers' APR are significantly affected by their Prosper ratings. The higher the rating, the lower the APR. And the borrowers' employment status play a part in APR as well. For unemployed people, they have to afford higher APR.

## Key Insights for Presentation

The main reason of people using Prosper is debt consolidation. This shows the borrowers have already got debts and Prosper can provide better APR than other loan companies. Top 5 occupations in the borrrowers are "Computer Programmer", "Executive", "Teacher", "Administrative Assistant", and "Analyst". Nearly half of all loans were in progress when Prosper Loan dataset was done. But in the loans which are finished, nearly 2/3 are completed. The failed loans (Changed Off, Defaulted, Past Due, Cancelled) account for 1/3 of all finished loans.

Prosper rating affects the borrower's APR strongly. So to get a good rating can reduce the APR which in turn reduce the monthly and overall payments.