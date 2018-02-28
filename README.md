# Prosper Loan Data Analysis
In this analysis, we explore loan data from Prosper. This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, borrower employment status, borrower credit history, and the latest payment information. I used R to do the analysis.

## Summary
### Loan Status vs Borrower APR
![alt text](https://github.com/jasccyang/ProsperLoanAnalysis/blob/master/pics/PlotOne.png?raw=true)
Bad loan statuses are correlated with higher APR. From this graph, we see bad loan statuses (Chargedoff, Defaulted, Past Due) have higher APR than good loan statuses (Completed, Current, FinalPaymentInProgress). Cancelled is a neutral status because the borrower decided not to take out the loan.

### Average Credit Score vs Borrower APR
![alt text](https://github.com/jasccyang/ProsperLoanAnalysis/blob/master/pics/PlotTwo.png?raw=true)
Having a high credit score and homeownership is correlated with lower APR. A majority of users with low credit score does not own a home.

### Original Loan Amount vs Borrower APR
![alt text](https://github.com/jasccyang/ProsperLoanAnalysis/blob/master/pics/PlotThree.png?raw=true)
Small loans are mostly made by non-homeowners and large loans are mostly made by homeowners. The lowest rates are largely given to homeowners regardless of loan amount. Higher APR (0.35) are more common with loans below $10,000.

## Reflection
Prosper Loan Data set is a very detailed dataset with many features to analyze. Not from a finance background, I had to read up on the terminology for quite a few words and descriptions for concepts. Something that should be obvious like lower APR in larger loan amounts was not immediately obvious to me. I think that’s one of the challenges in being a data analyst in that we have to become familiar with the data before we can ask the right questions. <br>
In my analysis, I’ve only explored a small set of features from this dataset. There’s much more to analyze with this dataset. A future work would be to explore Prosper’s own ratings of borrowers. In the multi-variant section, I explored the prosper score feature. We saw borrowers with credit scores below 600 was not given a Prosper rating. I’m curious to see what other methodologies Prosper uses to determine a borrower’s APR.

## Files
PorsperLoanAnalysis.html: html output of ProsperLoanAnalysis.rmd
ProsperLoanAnalysis.rmd: R Studio analysis of the data
prosperLoanData.csv: loan data from Prosper 
