# LoanDataFromProsper

## Dataset
[Dataset Download](https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv)<br>
[Dataset Description](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0)

This data set contains `113,937 rows` and `81 columns`.
each row has information on the borrow's APR, status, borrowed amount, debt, etc. Variables with many missing values will be dropped to make the Dataset more accurate. Outliers were also will be removed to provide more reliable Data.


<br>

## Questions
I will try to answer these questions: <br>
- What factors affect a loan’s outcome status?<br>
- What affects the borrower’s APR or interest rate?<br>
- What affects the original loan amount?


<br>

## Visualization Stage
I will choose only `17 columns` to use in the visualization of this project.<br> These columns are:
- LoanKey
- Term
- LoanStatus
- BorrowerAPR
- BorrowerRate
- ListingCategory (numeric)
- BorrowerState
- Occupation
- EmploymentStatus
- LoanOriginalAmount
- CreditScoreRangeLower
- CreditScoreRangeUpper
- DebtToIncomeRatio
- Investors
- StatedMonthlyIncome
- MonthlyLoanPayment
- IncomeVerifiable

I used some types of graphs such as:
- countplot
- histogram
- choropleth
- heatmap
- regplot
- scatter
- boxplot
- FacetGrid
- pointplot
- errorbar
- PairGrid
- violinplot
- scatterplot


<br>

## Summary of findings:

- many borrowers already have existing debts which is why they take debt consolidation loans in order to reduce the burden of existing debts and offer a new loan every month at low interest.
- maximum number of borrowers are Employed and the minimum number are Not employed
- the length of the loan (in months) is maximum for 36 months and minimum for 12 months.
- Loan status "Current" has the most number of counts
- Loan status "Completed" have second most number of counts.
- If **Borrower Rate** **increases Borrower APR will also increase** and vice-versa.
- Their is **moderate negative correlation** between **loan original amount** and **Borrower APR**, **Borrower Rate** variables.
- **Borrower APR** is **highly** correlated with **Borrower Rate**.
- Their seem to be some outliers present in credit score range upper and credit score range lower variables.
- There is a **moderate correlation** between **investors** and **Loan original amount.**
- We can see the moderate negative correlation between investors and Borrower APR, Rate variable **more clearly.**<br>
- we can see the moderate negative correlation of credit score lower and upper range with both Borrower APR, Rate variables **more clearly.**<br>
- We can clearly see the **moderate positive correlation** between **loan original amount** and **Credit score** lower and upper.<br>
- Debt to income ratio is moderately negatively correlated with stated **monthly income.**
- Many borrowers having **'self employed'** as employment status, have had **loan original amount close to 25000.**<br>
- Borrowers with **'not employed'** as employment staus are very less in our data and also most of them have **loan amount close to 2500** only with APR cloase to 0.20.


<br>

## Key Insights for Presentation
First, histogram plots were created to visualize the distribution of the borrower's APR percentages. After exploring all possible variables related to BorrowerAPR. ProsperScore has the strongest relationship with Borrower's APR (negatively correlated). 

Second, Scatter plots and Heatmap were also created to find out that ProsperScore and BorrowerAPR were negatively correlated. 

The third plot created multiple scatter plots (BorrowerAPR vs ProsperScore) on different letter ratings. The plots showed the lowerest rating(HR) of borrowers received the highest APR percentage, and borrowers with the highest rating (AA) received the lowest APR percentage.

<br>


## Resources 
- [Exploratory Visual Anatomy of Prosper Loan Dataset Using Tableau for 
P2P Lending](https://sersc.org/journals/index.php/IJFGCN/article/download/28201/15600/)
- [Loan_Data_Analysis](https://github.com/MarcCampmanyGar/Loan_Data_Analysis)
- [Prosper-Loan-Data-Exploration](https://github.com/RaniaHasan/Prosper-Loan-Data-Exploration)
- [LoanDataFromProsper](https://github.com/chikitabajaj/LoanDataFromProsper)