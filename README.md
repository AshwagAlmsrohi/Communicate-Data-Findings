# Communicate-Data-Findings
# Introduction
This project is part of the Udacity Data Analyst Nano Degree Program and serves as practice for data visualization. This document explores a dataset containing information about Prosper's loan data. Prosper is America’s first marketplace lending platform, with over $9 billion in funded loans. This dataset contains 113,937 loans with 81 variables on each loan.
# Data source
Loan Data from Prosper
https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv

# Summary and Conclusion
It seems that there are a lot of nulls for most of the variables in the dataset since I'm only interested to investigate some of the features from this dataset, I will subset the dataframe to extract the features of interest for my analysis and remove the nulls for this subset dataframe only
After reading through the descriptions and definitions, I chose ['Term', 'LoanStatus', 'BorrowerRate', 'ProsperRating (Alpha)', 'ListingCategory (numeric)',
              'EmploymentStatus','DelinquenciesLast7Years', 'StatedMonthlyIncome', 'TotalProsperLoans',
              'LoanOriginalAmount','LoanOriginationDate', 'Recommendations', 'Investors','BorrowerAPR','ProsperScore',
            'Occupation','IncomeRange' ]
However by combining these variables I think we should be able to gather some interesting insights and better understanding our borrowers.

# Variable Defintions
Taken from our Prosper Loan Data - Columns Definitions.csv that was provided with the dataset I will now define the individual variables i have selected for my analysis:
Term: The length of the loan expressed in months.
LoanStatus:The current status of the loan: Cancelled,  Chargedoff, Completed, Current, Defaulted, FinalPaymentInProgress, PastDue. The PastDue status will be accompanied by a delinquency bucket.
BorrowerRate:The Borrower's interest rate for this loan. 
ProsperRating (Alpha):The Prosper Rating assigned at the time the listing was created between AA - HR.  Applicable for loans originated after July 2009.
ListingCategory (numeric):The category of the listing that the borrower selected when posting their listing: 0 - Not Available, 1 - Debt Consolidation, 2 - Home Improvement, 3 - Business, 4 - Personal Loan, 5 - Student Use, 6 - Auto, 7- Other, 8 - Baby&Adoption, 9 - Boat, 10 - Cosmetic Procedure, 11 - Engagement Ring, 12 - Green Loans, 13 - Household Expenses, 14 - Large Purchases, 15 - Medical/Dental, 16 - Motorcycle, 17 - RV, 18 - Taxes, 19 - Vacation, 20 - Wedding Loans
EmploymentStatus:The employment status of the borrower at the time they posted the listing.
DelinquenciesLast7Years:Number of delinquencies in the past 7 years at the time the credit profile was pulled.
StatedMonthlyIncome:The monthly income the borrower stated at the time the listing was created.
TotalProsperLoans:Number of Prosper loans the borrower at the time they created this listing. This value will be null if the borrower had no prior loans. 
LoanOriginalAmount:The origination amount of the loan.
LoanOriginationDate:The date the loan was originated.
Recommendations:Number of recommendations the borrower had at the time the listing was created.
Investors:The number of investors that funded the loan.
BorrowerAPR:The Borrower's Annual Percentage Rate (APR) for the loan.
ProsperScore:A custom risk score built using historical Prosper data. The score ranges from 1-10, with 10 being the best, or lowest risk score.  Applicable for loans originated after July 2009.
Occupation:The Occupation selected by the Borrower at the time they created the listing.
EmploymentStatusDuration:The length in months of the employment status at the time the listing was created.
IncomeRange:The income range of the borrower at the time the listing was created.

# Key Insights for Presentation

Insights from the multivariate exploration data
For Applicants with prosper ratings from AA to D have the higher loan amount with increased salary
Employed and full time employees have their mean salaries in higher range
Majority of the borrowers are falling under prosper rating of B , irrespective of the income range
The monthly income of borrowers are having higher values for employed, other and full time employment status
with the prosper rating of AA, A and B
We can also clearly observe that HR prosper rating applicants have higher interest rates
To conclude this analysis , I say that the loan approval status is heavily dependent on the applicant's information on IncomeRange, and employment status.
