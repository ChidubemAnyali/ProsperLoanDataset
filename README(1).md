# (Dataset Exploration Title)
## by (Chidubem Anyali)


## Dataset

The prosper loan is a company that specializes in giving out low interest loans to their customers. They have made their dataset available for this analysis. The dataset contains 81 columns and 113937 rows/ observations. This dataset is financial dataset and this is related to the loan, borrowers, lenders and interest rates. For this analysis, I didnt use all the columns in the dataset. I didnt have to clean the dataset, also. I only changed data type of Prosper Rating from an object to a categorical data type, to fit into the chart i created, properly. The columns that i ended up using for this analysis are:
1. Income Verifiable: The borrower indicated they have the required documentation to support their income.
2. Listing Category (numeric): The category of the listing that the borrower selected when posting their listing: 0 - Not Available, 1 - Debt Consolidation, 2 - Home Improvement, 3 - Business, 4 - Personal Loan, 5 - Student Use, 6 - Auto, 7- Other, 8 - Baby&Adoption, 9 - Boat, 10 - Cosmetic Procedure, 11 - Engagement Ring, 12 - Green Loans, 13 - Household Expenses, 14 - Large Purchases, 15 - Medical/Dental, 16 - Motorcycle, 17 - RV, 18 - Taxes, 19 - Vacation, 20 - Wedding Loans
3. Income Range: The income range of the borrower at the time the listing was created.
4. Prosper Rating (Alpha): The Prosper Rating assigned at the time the listing was created between AA - HR.  Applicable for loans originated after July 2009.
5. Term: The length of the loan expressed in months.
6. Borrower APR: The Borrower's Annual Percentage Rate (APR) for the loan.
7. Loan Status: The current status of the loan: Cancelled,  Chargedoff, Completed, Current, Defaulted, FinalPaymentInProgress, PastDue. The PastDue status will be accompanied by a delinquency bucket.
8. Monthly Loan Payment: The scheduled monthly loan payment.
9. Loan Original Amount: The origination amount of the loan.
10. Estimated Effective Yield: Effective yield is equal to the borrower interest rate (i) minus the servicing fee rate, (ii) minus estimated uncollected interest on charge-offs, (iii) plus estimated collected late fees.  Applicable for loans originated after July 2009.
**To get the visualization done, i had to import 2 libraries: seaborn and matplotlib. 
**I had quite a number of count plot charts, so i had to create a function in order to reduce code repetiions and also saved my time.
**For the pie chart, I had to get the proportion by dividing the length of the true/false values by the length of the entire column, multiplied by 100.
**For the histogram charts, i used he sb(which is the alias for seaborn).histplot function.
** For the violin and box plot for one categorical and one quantative variable, I used the sb.violinplot and sb.boxplot funtion.
** For the scatter chart, i used the sb.regplot function.
** For the scatter chart used for the multivariate visualization, I used the plt.scatter function, sb.barplot function and sb.facetgrid function.
** I also made sure i attached a title to each chart, an x and a y label and  i used ticks where needed



## Summary of Findings

I was able to come up with 15 visualizaions for this analysis. They are 7 univariate visulalizations, 7 bivariate visualizations and 1 multivariate visualization.
Chart 1: Proportion of True to False Income Verifiable- This pie chart depicts the proportion of borrowers with verifiable income. This chart shows that over 92.39% of the borrowers income has been verified. This is a good outlook on the business and this practice should continue.
Chart 2: Count of Listing Category- This chart shows that 58308(51%) of the total borrowers, take the loan for Debt consolidation which means they use the amount borrowed to offset other liabilites. Only a small fraction of the borrowers take loans for engagement ring, baby & adoption, cosmetic procedure, boat, green loan and RV. 
Chart 3: 'Count of Income Range- From this chart it is evident that we have most of our borrowers within the income range of $25,000-49,999. And for those that earn no money they are have the least number of borrowers.
Chart 4: Count of Prosper Rating-From this chart we would see that majority of the borrowers has the proper rating C, while the least number of borrowers fall within the proper rating- AA
Chart 5: Distribution of Term of Loan- This chart shows that most loans are taking for 36 months which is 3 years.
Chart 6: Distribution of Borrower Annual Percentage Rate- This chart shows that the Borrowers Annual Percentage is rightly skewwed and the highest percentage falls within 0.36
Chart 7: Count of Loan Status- This chart shows that there we has over 5000 loans in the status "Current" and about 4000 loans that are in the "completed status". No loan was canceled or past 120 days. Less than 1000 loans were defaulted and a small portion of them are over due by some number of days
Chart 8: Realtionship between Loan Original Amount and Monthly Loan Payment- From this chart we can see that the higher the loan original amount, the higher the monthly loan payment to be remitted by the borrower. Which means that there is a positive correlation between the loan original amount and the monthly loan payment.
Chart 9: Relationsip between Loan Original Amount and Borrower Annual Percentage Rate- This chart shows that the higher the loan original amount, the lower the borrower annual percentage rate. It shows that the annual percentage rate is higher is smaller loan amount. Which also tells us that there is a negative relationship between both variables.
Chart 10 and 11: Relationship between Prosper Rating and Estimated Effecive Yield- From this chart, it shows that prosper loan company charges according to how risky a loan a loan is. For those that have a rating of AA their interest is the lowest, it progresses like that until the rating HR that has the highest interest attached to it. In the really sense, it is meant to be so, as the higer the risk, the higher the return for the investor/lender.
Chart 12 and 13: This chart has further buttressed our observation in the last chart. It is seen here that those with the highest rating "AA", have the lowest Borrower Annual Percentage Rate. It progresses like that until it gets to those with the lowest rating "HR", paying the highest Borrower Annual Percentage Rate.
Chart 14: Relationship between Prosper Rating and Income Verifiable- This chart shows that generally all borrowers that cut across all the ratings has a high margin of those with verifiable income. But, those that fall in the E and HR ratings, have a larger number of unverifiable income.
Chart 15: Relationship between Borrower Annual Percentage Rate, Estimated Effective Yield and Term of Loan- This charts sums it all up, it shows that the higher the borrower annual percentage rate on the borrower, the higher the estimated effecive yield for prosper loan. The chart also shows that most of the loans were taken on a 36 months term and the higher the term of the loan, the higher the yield for prosper loan and the percentage rate for the borrower.

## Key Insights for Presentation
The key insights from the data visualizations are:
1. We have a larger number of borrowers with verifiable income
2. The higher the risk for giving out loans, the higher the income of the company.
3. A greater portion of borrowers take loan for debt consolidation
4. The higher the money borrowed, the higher the monthly loan payment made by the borrower.
5. A larger proportion of borrowers earn between $25,000 and $74,999.
6. A greater portion of the loans are taken on a 36 months term