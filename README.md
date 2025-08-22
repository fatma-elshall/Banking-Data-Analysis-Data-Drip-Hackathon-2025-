### 1. Project Objective

The purpose of this project is to analyze customer, card, and transaction data from a bank in order to provide actionable insights that support decision-making in three key areas:

* Customer profiling – understanding demographics and behavior.

* Risk management – evaluating creditworthiness and card security.

* Loan eligibility – identifying customers with high potential for loan approval.

## The ultimate goal is to enable the bank to reduce risk, improve credit policies, and increase customer engagement and profitability.

## Dashboard link in Tableau puplic: 

https://public.tableau.com/views/BankdataanalysisHackathonDatadrip/Transactions?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

## Dataset link :

https://drive.google.com/drive/folders/1D6g7s_HsD2TpgVbJc6K1QjT3q4xRv0pv?usp=drive_link

### 3. Tools used: 
* Python : for Data cleaning and Exploration .
* Tableau : for data visualization and Dashboard design
  
### 4. Data Sources

The dataset is composed of three main tables:

* Users Table

Contains demographic and financial information about customers such as age, gender, income, state, and account open date.

* Cards Table

Provides details about issued cards, including card type (debit/credit), brand (Visa/Mastercard), credit limit, chip availability, and year of last PIN change.

* Transactions Table

Includes transaction-level data such as transaction amount, merchant details, transaction type (swipe, chip, online), and error flags.

These three tables were connected inside Tableau using appropriate relationships to allow integrated analysis across customers, cards, and transactions.

### 5. Key Calculated Fields

Several calculated fields were developed in Tableau to enable deeper insights:

* Debt to Income Ratio (DTI):

[Total Debt] / [Yearly Income]


* Measures the proportion of debt relative to income.

Key indicator for loan repayment capacity.

* Credit Score Segment:

Categorized customers into groups such as Poor, Fair, Good, Excellent.

Helps in evaluating customer eligibility for credit products.

* Age Generations:

Segmented customers into generations (Gen Z, Millennials, Gen X, Baby Boomers) based on age.

Useful for marketing and product targeting.

* PIN Risk Category:

Calculated the number of years between Account Open Date and Last PIN Change Year( as the data was historical data not real time data).

Classified customers as:

Safe (<2 years),

need alarm (2–5 years),

High Risk (>5 years).

This metric is critical for security risk management.

* Loan Eligibility:

Combined Credit Score Segment and DTI Risk Category into a single rule to classify customers as:

Eligible (High Score + Low DTI),

Not Eligible (others).

Provides a framework for identifying customers suitable for loan offers.

### 6. Dashboards

## A. Customer Overview Dashboard

Objective:

Provide a demographic and financial overview of the customer base.

Show insights by age, gender, location, and card ownership.

* Key Findings:

* Majority of customers fall into Gen X and Gen Y.

* Debit cards dominate (85%), indicating potential to expand credit card products.

* Geographic analysis shows income and debt variation across states.


## B. Card & Risk Analysis Dashboard

Objective:

Assess card distribution, PIN security, and customer risk segmentation.

Identify vulnerabilities and opportunities for improvement.

* Key Findings:

* Loan Eligibility: Only ~22% of customers are currently eligible.

* PIN Security: ~22% are at high risk due to outdated PIN changes.

* Chip Adoption: 11% of cards still lack a chip, exposing the bank to fraud risks.

* Credit Score: 42% of customers fall into Fair/Poor categories, representing both risk and opportunity.

* Card Brands: Mastercard (52%) and Visa (38%) dominate the portfolio, opening room for stronger co-branded partnerships.

## C. Transactions Dashboard

Objective:

Analyze transaction volumes, types, errors, and merchant distribution.

Identify trends in customer spending behavior.

* Key Findings:

* Transaction Types: Majority are swipe-based (52%), with low online adoption (12%).

* Errors: Error rate of 3.44%, mostly from insufficient balance and incorrect PIN.

* Merchant Insights: Online transactions lead by total value (89M), with CA, TX, and NY being top-performing states.

* Credit Utilization: Average credit limit is $14.3K, but average transaction amount is only $43 → significant unused capacity.

## 7. Business Recommendations

Based on the analysis across the three dashboards, the following recommendations are proposed:

* Expand Credit Card Adoption:

Cross-sell credit cards to existing debit customers to increase revenue from interest.

* Strengthen Security:

Implement mandatory PIN resets every 2–3 years.

* Accelerate chip card migration to reduce fraud exposure.

* Optimize Loan Policies:

Target High Score + Low DTI customers for loan offers.

Provide financial education or debt restructuring for medium-risk customers to move them into the eligible segment.

* Promote Digital Payments:

Incentivize online transactions through rewards, cashback, and partnerships with e-commerce platforms.

Enhance Customer Segmentation:

Use demographic and geographic insights to design targeted marketing campaigns (e.g., Millennials → digital services, Gen X → housing/mortgage loans).

* Improve Operational Efficiency:

Reduce transaction error rates by enabling balance alerts and strengthening fraud detection algorithms.

##  Conclusion

This project successfully integrates data from users, cards, and transactions to build actionable dashboards in Tableau. The analysis provides the bank with clear strategies to:

* Grow revenue (through cross-selling and digital adoption),

* Reduce risk (via improved security and credit assessment), and

* Enhance customer engagement (by offering tailored financial products).
