# READme file for Analysis of Prosper Loan dataset


## by  Henry Ime Mbom


## Dataset

> This dataset contains the customer's data from a loan company known as Prosper. This dataset comprises of 113,937 observation with 81 Features on each loan which includes loan amount, borrower rate, current loan status, borrower income, Prosper score, etc. The dataset was downloaded from : https://www.google.com/urlq=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&ust=1581581520570000

## Summary of Findings.

<b> The following observations were made during the univariate analysis phase:</b>

> The count of BorrowerAPR values between 0.00 and 0.05 appeared to be nearly zero when plotted on a histogram compared to that of BorrowerRate which is above 10000 in the same range.But transforming the count axis to a log scale reveals more about the count of BorrowerAPR in this range. BorrowerAPR variable observed to contain 25 missing value programmatically.

> The hisplot of the StandardMonthlyIncome variable is highly driven to the left of the axis.Using summary statistics I figured out the maximum count value to be 1750000, which could have caused an outlier or error in the plot. So I created a second visualization where the top 1% of the data were dropped from the original dataset inorder to obtained a more reasonable plot.


>The ListingCreationDate variable was converted to a datetime object in the format ‘yyyy-mm-dd’ to indicate the loan listing creation dates; and the column name of the ListingCategory varaible was changed from 'Listing category (numeric)' to a simple and easily accessible name: ListingCategory.

<b> Following the univariate exploration of variables was the bivariate exploration where relationships between the variable of interest and some supported variables were established.The outcome of this phase is summarized as follows:</b>

>There was a high correlation between Borrower's rate and Borrower's APR varaibles in the range 0.1 to 0.2 percent.

> Standard monthly income and borrower's rate are highly negatively correlated between 0.2 to 0.3 borrower's rate at about 100000 standard monthly income.Outliers were observed below the zero line.

> Borrower's rate is highly correlated with Prosper's score for Prosper's score between 3.0 and 8.0.

> When a borrower has relatively low credit amount (< about 25,000) the probabilities of getting low and high interest rates are similar. However, when the borrower’s credit amount is high (>about 50,000), he/she is more likely to get a lower interest.

<b> Lastly, a multivariate exploration was performed on the dataset, and the following observations were made:</b>

> Majority of the borrowers whose available credit falls below 100000 were unemployed,retired and part time workers.Self employed and full time borrowers have credits extending to up to 300000 dollars. Between credit limit 0 to 5000 dollars, borrowers across all employment status are represented.

> Majority of the borrowers whose available credit were below 100000 have their loan status as either being in default or charged off; while borrowers with loan status completed or current have their credit extending to 300000 dollars.

> It was concluded that the employment status of a borrower can be used to predict their loan Status.

## Key Insights for Presentation.

> Borrower's rate is highly correlated with Prosper's score for Prosper's score between 3.0 and 8.0.

> When a borrower has relatively low credit amount (< about 25,000) the probabilities of getting low and high interest rates are similar. However, when the borrower’s credit amount is high (>about 50,000), he/she is more likely to get a lower interest.

> Employment status of a borrower can be used to predict their loan Status and Borrower's rate.





 















> 