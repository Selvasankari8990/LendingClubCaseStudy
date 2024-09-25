## Lending Club Case Study

## About the Company: 
	This company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface. Like most other lending companies, lending loans to risky applicants is the largest source of financial loss (called credit loss). **Credit loss** is the amount of money lost by the lender **when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'


## Table of Contents
* General Info
* Technologies Used
* Conclusions
* Acknowledgements


## Business Understanding: 

When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile.

**Two types of risks** are associated with the bank’s decision: 
       - If the applicant is **likely to repay** the loan, then **not approving the loan results in a loss of business** to the company 
       - If the applicant is **not likely to repay** the loan, i.e. he/she is likely to default, then **approving the loan may lead to a financial loss** for the company
       .
## Business Requirements (Objective of this Case Study): 
       The company wants to understand the **driving factors (or driver variables) behind loan default**, i.e. the variables which are strong indicators of default. 
       The company can **utilise this knowledge for its portfolio and risk assessment**. If risky loan applicants can be identified early, then **such loans can be reduced thereby cutting down the amount of credit loss**. Therefore, the need is to Perform a Detailed Exploratory Data
       
## Analysis on the Lending Club Loans Data: 
- To identify patterns which indicate if a person is likely to default. 
- To understand how consumer attributes and loan attributes influence the tendency of default.
- Recommend actions such as denying the loan, reducing the loan amount, lending at a higher interest rate, etc.

** Approach followed for Exploratory Data Analysis:**
 Below are the steps that would followed for performing this EDA:

1. Importing necessary libraries & Loading Data for Analysis
2. Data Understanding
	2.1   Exploring the Data Dictionary
	2.2   Exploring Data Structure, Data Shape and Size
	2.3   Null Values & Unique Values Analysis
3. Data Wrangling
	3.1   Remove Unwanted Columns and Rows
	3.2   Missing Values Treatment
	3.3   Derived Metrics Columns
	3.4   Data Segmentation
	3.5   Outliers Treatment
4. Data Analysis
	4.1   Univariate Analysis
	4.2   Bivariate Analysis
	4.3   Multivariate Analysis
5. Summarising Observations



## Conclusions
1.	Out of the Total Loans approved and issued, only 14% have defaulted.
2.	We can observe that only 56% of the Charged Off loans get recovered. However, in the Fully Paid loans recoveries are made more than the issued amount. This might be due to interests and other fees. This shows that the Fully Paid loans generate a profit of around 17%.
3.	We can observe that the number of loans issued has been exponentially increasing year after year. It is also clearly seen that most of the loans are applied during the Q4 (Quarter 4) of every year. The Default rate is even spread across the years and the months and hence no significant observation can be made there.
4.	Loan Amounts vary from 500 to 35000. Loans of 10k are the most commonly sought loan. 78% of the loans are under 15k and only 10% of the loans are greater than 20k. We can also observe that as the Loan Amount increases the Charge off % also increases. This shows that the higher loans, substantially carry a higher risk of default.
5.	There are only 2 Loan Tenures - 36 months (3 yrs) and 60 months (5 yrs). 36 months is the most preferred choice for almost 76% of loan applicants. It is also the beneficial option for the business, since only 10% of this group ends in default. Whereas, the 60 months tenure has a default rate of 25%. This means that 1 out of every 4 60 month tenured loans has not been paid back.
6.	Almost 75% of the loans have 15% of lesser interest rates.
7.	Grades A and B together account for 57% of the total loans. The Sub-Grades spread also confirms the same thing, that larger proportion of loans fall within higher grades or sub-grades. This indicates a good shift toward higher-quality borrowers, it suggests a healthier loan portfolio with potential for better financial performance, lower risk, and stronger investor confidence. This positive trend should be monitored and leveraged in strategic planning. We can also observe that the Default Rate has an inverse proportion against the grades i.e., Higher the Grade, Lower the Default Rate. This clearly indicates that the existing Grade System is beneficial to the business.
8.	The highest percentage of loan applicants (22%) have been employed for â€˜10+ years, indicating that a significant portion of applicants have stable, long-term employment. This clearly indicates that business should prioritize applicants with longer employment histories, as they are often seen as lower risk. However, there is still a notable percentage of applicants with shorter tenures, indicating a diverse applicant pool.
9.	Almost 92% of the applicants are either in a rental home or have a mortgage on their homes. This means that there is a high risk of loan repayment from these types of applicants. This can also be confirmed by analysing the spread against the loan status. There is a clear indication that the Default Rate is minimal in-Home Owned Applicants when compared to the Applicants who do not own a house.
10.	The verification status reveals that 44% of borrowers are unverified, indicating potential risk. While 31% have verified status, suggesting creditworthiness, the low verification rates highlight opportunities for improved processes. Enhanced verification could reduce default rates, ensure compliance, and inform targeted lending strategies for better portfolio performance.
11.	The income distribution shows that 34% of borrowers earn 25k-50k, with 65% in the 25k-75k range, indicating a focus on middle-income earners. Only 6% earn 0-25k, suggesting higher risk. There is potential to tailor loan products for these demographics while engaging higher-income borrowers effectively. Analysing the Income Spread against the Loan Statuses, we can see that mostly fully paid loans are concentrated around lower annual incomes; higher incomes have fewer defaults (charged off). Currently loans are evenly distributed across all income levels. Applicants with an annual income of 50k or lesser are most likely to default and applicants with higher annual income are less likely to default.
12.	The most popular loan purpose is "debt consolidation" with 47% contribution followed by the "credit cards" with 13% contribution. Together they form 60% of the loans, indicating that the loan applicants predominantly use the loans for debt management and handling personal expenses. On analysing the spread against the loan status, we can see that 27% of loans for small business are Charged off making them the riskiest.
13.	We can observe that California has the highest number of loans with 18%, followed by New York at 10% and Florida at 7%. Most states have a higher proportion of Fully Paid loans compared to Charged Off loans. However, there are notable exceptions, such as Nevada (60% Default Rate) and Arkansas (21% Default Rate), which have a relatively high proportion of Charged Off loans. This suggests that while some states may have higher overall lending activity, the risk of loan default varies across different regions.
14.	Most loans are fully paid across all debt-to-income ratios, peaking around 17.5. Higher ratios correlate with more defaults (charged off), indicating increased risk. Lower ratios suggest better financial health and higher repayment likelihood. Currently loans are evenly distributed across all ratios.
15.	Almost 96% of the applicants do not have a bankruptcy record. This is very beneficial to the business and indicates that our loan approval processes is very strong. While analysing bankruptcies against the loan status, we see that the Default Rate is Directly Proportional and Positively Correlated with the Bankruptcies. That is, Higher the Bankruptcy, Higher the Chance of Default Rate.
16.	Interest Rates are directly proportional to the loan tenure. Earlier we saw that the Loan Amounts were also high for higher tenure. Hence, we can understand that higher the amount, higher the tenure and hence higher the interest rate as well, which is beneficial to business since it will yield more revenue.
17.	Interest Rates are inversely proportional to the Grades or Sub-Grades. There is a negative correlation between them. This means that Higher the Grades, Lower the Interest Rate. Earlier, we saw that the Default Rates are quite high in the lower grades. Hence, we say that the current interest rate slabs are perfectly aligned, since for Lower Grades, the Risk is higher and hence the Interest Rates are also higher ensuring loss compensation.
18.	Strong Correlation Between Total Payment and Loan Amount: As expected, there's a strong positive correlation between the total payment and the loan amount, indicating that larger loans generally result in higher total payments.
Business Benefit / Impact:
- Will be helpful to estimate the total amount of revenue that can be expected from loans.
- It can also help in setting appropriate interest rates and repayment terms based on loan amounts.
19.	Positive Correlation Between Installment and Loan Amount: Loans with higher installments tend to have larger loan amounts, suggesting a direct relationship between monthly payments and the total loan value.
Business Benefit / Impact:
- Helps to Tailor loan offerings to different borrower preferences by offering varying installment plans.
- This can also help in managing cash flow and risk by ensuring that borrowers can afford their monthly payments.
20.	Negative Correlation Between Interest Rate and Total Payment: Annual Income and Debt to Income Ratio also are negatively correlated with each other. This indicates that borrowers with higher incomes tend to have lower debt burdens relative to their income, possibly reflecting better financial management or more favorable lending terms.
Business Benefit / Impact:
- This finding suggests that a higher interest rate might not necessarily lead to higher total payments. Company should carefully consider the impact of interest rates on borrower behavior and repayment patterns.
- Lending Club should explore alternative pricing strategies or incentives to encourage early repayment or refinancing.
21.	Negative Correlation Between Annual Income and Debt to Income Ratio: Surprisingly, there's a negative correlation between interest rate and total payment. This might suggest that borrowers with higher interest rates are more likely to make larger payments, potentially due to early repayment or refinancing strategies.
Business Benefit / Impact:
- This insight suggests that higher-income borrowers may be more creditworthy, allowing the company to refine its lending criteria to attract this demographic.
- Lending Club could develop targeted products or services for higher-income clients to optimize portfolio performance and minimize risk.
22.	Weak Correlation Between Loan Term and Total Payment: The correlation between loan term and total payment is relatively weak, indicating that the length of the loan doesn't have a strong impact on the total amount paid.
Business Benefit / Impact:
- Lending Club can offer flexible loan terms without significantly affecting the total revenue generated.
- However, they should carefully evaluate the risk associated with longer loan terms and implement appropriate risk management strategies.
23.	No Significant Correlation Between Credit History and Loan Performance: Variables like public record bankruptcies, open accounts, and earliest credit line year show weak or no correlation with the target variable (loan status defined in Data Segmentation section), suggesting that these factors may not be as influential in predicting loan outcomes.
Business Benefit / Impact:
- While credit history can still be a valuable factor in assessing risk, Lending Club might need to explore additional factors to improve their creditworthiness evaluation models.
- They could consider alternative data sources or risk assessment techniques to enhance their underwriting process.
24.	The analysis reveals that as loan amounts increase, so do the number of installments and interest rates. Borrowers classified as "Not-Verified" typically receive loans under 25k, while those labeled "Verified" often secure loans over 25k. Additionally, borrowers with shorter loan terms face higher installment amounts. These insights can guide lending strategies and risk assessments.


## Technologies Used
    * Pandas
    * NumPy
    * Seaborn
    * MatplotLib 

## Acknowledgements
Give credit here.
- This project was inspired by...
- References if any...
- This project was based on [this tutorial] (https://www.example.com).


## Contact Created by [@Selvasankari8990/LendingClubCaseStudy] - feel free to contact me!



