# Communicate-Data-Findings
# Introduction
This project is part of the Udacity Data Analyst Nano Degree Program and serves as practice for data visualization. This document explores a dataset containing information about Prosper's loan data. Prosper is America’s first marketplace lending platform, with over $9 billion in funded loans. This dataset contains 113,937 loans with 81 variables on each loan.
# Data source
Loan Data from Prosper
https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv

# Summary and Conclusion
In the exploration, I found that the borrower APR is negatively correlated with original loan amount. At different size of the loan amount, the APR has a large range, but the range of APR decrease with the increase of loan amount. The borrower APR also decreases with the increasingly better rating. Borrowers with the best Prosper ratings have the lowest APR. It means that the Prosper rating has a strong effect on borrower APR. Interestingly, the relationship between borrower APR and loan amount turns from negative to slightly positive when the Prosper ratings are increased from HR to A or better. This is may because people with A or AA ratings tend to borrow more money, increasting APR could prevent them borrow even more and maximize the profit. But people with lower ratings tend to borrow less money, decreasing APR could encourage them to borrow more. I also found that the borrower APR decrease with the increase of borrow term for people with HR-C raings. But for people with B-AA ratings, the APR increase with the increase of borrow term.

Outside of the main variables of interest, I found that the loan amount is positively correlated with the stated monthly income, it makes sense since borrowers with more monthly income could loan more money. The loan amount is also increased with the increase of loan term. I also found that borrowers with better ratings have larger monthly income and loan amount. Employed, self-employed and full time borrowers have more monthly income and loan amount than part-time, retired and not employed borrowers. There is a interaction between categorical term and Prosper rating features.  For loan amount, there is a interaction between term and rating. With better Prosper rating, the loan amount of all  terms increases, the increase amplitude of loan amount between terms also becomes larger.

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

For the presentation, I just focus on features that could affect the borrower APR, which are original loan amount, Prosper rating. I started by showing the distribution of borrower APR and loan amount variable. Then, I showed the relationship between APR vs. loan amount, as well as APR vs. rating. I also investigated the effect of rating on ralationship between APR and loan amount, as well as the effect of rating on relationship between borrower APR and term.
We can also clearly observe that HR prosper rating applicants have higher interest rates


To conclude this analysis , I say that the loan approval status is heavily dependent on the applicant's information on IncomeRange, and employment status.
