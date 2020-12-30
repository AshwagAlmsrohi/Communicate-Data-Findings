# Communicate-Data-Findings
# Introduction
This project is part of the Udacity Data Analyst Nano Degree Program and serves as practice for data visualization. This document explores a dataset containing information about Prosper's loan data. Prosper is America’s first marketplace lending platform, with over $9 billion in funded loans. This dataset contains 113,937 loans with 81 variables on each loan.
# Data source
Loan Data from Prosper
https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv

# Summary and Conclusion
In the exploration,
-The borrower APR is negatively correlated with original loan amount.
-LoanStatus of all Borrowers are with current and completed state.
-The range of APR decrease with the increase of loan amount .
- Borrowers with the best Prosper ratings have the lowest APR.
- EmploymentStatus of all Borrowers are with Employed State
Majority of the loan applicants are from 50K to 75K range with emloyeed status.
- Applicants with incomerange of 50K to 75K range have their prosper rating falling under AA, A, B and C.
- With better Prosper rating, the loan amount of all terms increases, the increase amplitude of loan amount between terms also becomes larger.


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

# Key Insights for the Presentation
There are total of 113937 loans entries saved in the dataset and 81 attributes. Each loan contain information on the borrowered's background information and details regarding the loans.This analysis will focus on years between (2010 and 2013) and factors that are related to Prosper loans status (LoanStatus).

For the presentation, I mainly focused on the features that are impactful for approval of loan status. So for this I looked at the distribution of each and every numeric and categorical variables and did all the necessary univariate, bivariate and multivariate analysis on selected variables.


# Key Insights for Presentation
- For Applicants with prosper ratings from AA to D have the higher loan amount with increased salary
Employed and full time employees have their mean salaries in higher range.
- Irrespective of the income range
The monthly income of borrowers are having higher values for employed, other and full time employment status
with the prosper rating of AA, A and B.
- LoanStatus of all Borrowers are with current and completed state.
- Longer term loans have on average lower APR.
- 2013 - 2014 Prosper Score follows a gradual transition from purple to yellow, investors seemed to have really adopted this risk rating.
- 2011 onwards max APR has dropped from above 40% to slightly above 36% .
- Top IncomeRange of all Borrowers are within $25,000-49,999.
- Most of the borrower have a fairly low Prosper Score of 4 (custom risk score) while the majority of the customer have a score between 5-8. You can also see that even customers with the low risks score of 1 or 2 did get a loan from Prosper. Furthermore, not many borrowers received the highest score of 10.
- The Income Range of the borrower seem not to have an impact on the outcome of the loan.
- The majority (~50,000) of people who currenly has a loan are empolyed no matter what is their ProsperScore.
- Plots also show that BorrowerRate has a negative relationship with LoanOriginalAmount and has a postive relationship with ProsperScore.

To conclude this analysis , I say that the loan approval status is heavily dependent on the applicant's information on IncomeRange, and employment status.
