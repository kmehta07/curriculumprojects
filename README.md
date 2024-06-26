Executive Summary :

Our research undertook a comprehensive exploration into the dynamics of credit risk
fraud of various customers present in the dataset. We analyzed the behavior patterns of
a large number of individuals that may indicate potential credit risk or fraudulent
activities. This includes monitoring major factors such as income, employment length,
interest rates, home ownership status, whether the person has defaulted on the current
loan, whether the person has defaulted in the past, the number of times the person has
defaulted, etc. Our findings revealed patterns and trends of the defaulters which can be
used extensively for business insights and improving business strategies to enhance
risk management, ensure regulatory compliance, and ultimately fortify the financial
health of lending institutions.


Data Fields and Descriptions:
1. person_id: Unique identifier for each individual.
2. person_age: Age of the individual.
3. person_income: Annual income of the individual.
4. person_home_ownership: Home ownership status (categorical: RENT, OWN,
MORTGAGE).
5. person_emp_length: Employment length in years.
6. loan_intent: Purpose of the loan (categorical: PERSONAL, EDUCATION, MEDICAL,
etc.).
7. loan_grade: Loan grade (categorical: A, B, C, etc.).
8. loan_amnt: Loan amount.
9. loan_int_rate: Loan interest rate.
10. loan_status: Default status on the current Loan (binary: 1 for default, 0 for not default).
11. loan_to_income_ratio: Ratio of loan to income.
12. cb_person_default_on_file: Historical default status (whether the person has defaulted
in the past or not) (binary: Y or N).
13. cb_person_cred_hist_length: Credit history length.
14. credit_score: Credit score.
15. number_of_open_accounts: Number of open bank accounts.
16. past_delinquency_count: Count of past delinquencies.(No of defaults in the past)


Our research seeks to answer the following important concerns about loan default risk and
consumer behavior in the financial lending industry:
● What are the main markers or elements that influence the probability that borrowers may
fail to make loan payments? This entails determining important financial parameters like
credit score and stable income, as well as individual characteristics like work history and
intent of the loan.
● How do these variables work together to affect the likelihood of a loan default? Our goal
is to comprehend the intricate connections among different factors and how they affect
the risk assessment procedure as a whole. For example, does the likelihood of a loan
default increase with a higher loan-to-income ratio?
● Can machine learning algorithms better anticipate loan default by making use of a wide
range of data points? We investigate how advanced analytics methods might be used to
combine data from many sources to produce more accurate risk evaluations. This entails
evaluating how well different models capture subtle trends in consumer behavior.
● What effects on risk management and decision-making do our prediction models have
for lending institutions? We examine how our findings might be used to improve lenders'
capacity to reduce the financial risks brought on by loan defaults.



What techniques did you use and why?
● Data Cleaning and Processing: We took great care to ensure that the financial
information in our dataset was accurate and consistent.
● Exploratory Data Analysis (EDA): By delving into the subtleties of our credit data, we
were able to identify patterns and trends unique to the risk of loan default.
● Spark SQL: We processed massive amounts of credit data quickly and effectively using
Spark SQL, which was essential for our extensive study.
● Graph Frames: We used Graph Frames to map complex linkages between borrower
attributes and loan default outcomes to gain important insights.
● Logistic Regression: Taking into account distinct credit risk characteristics, our logistic
regression models were optimized to forecast the likelihood of a loan default.
● Decision Trees: To better identify the important factors determining the possibility of a
default, we employed decision trees to sort through intricate credit metrics.
● Random Forest Classifier: We used random forest classifiers to combine various
decision trees and improve our predictions, which were then customized for credit risk
evaluation.



Finding 1:
To find the number of defaulted customers with a credit score and average personal income
The data has been grouped based on the loan grade and loan intent
The above analysis tells us about the number of customers who have a credit score above 680
which is a good credit score and a personal income of above 77800 which is an average income
but has still defaulted.


Finding 2:
Number of defaulters between the ages 31-40, who have defaulted in the past more than 3
times, having a credit history length more than 10.
The data has been grouped based on age and past credit history length.
By grouping customers based on both Age and Home Ownership the financial institution gains
insights into specific customer financial particulars more prone to risk. Identifying higher risks
within a certain age or Home Ownership details highlights potential challenges that should be
tackled.
From the above analysis, we can infer that - there doesn't appear to be a clear pattern regarding
age and defaulting, especially when home ownership is also considered. There might be a
relationship between home ownership status and defaulting


Finding 3:
We ran three machine learning models using the necessary feature engineering on the data.
The three models are - Logistic Regression, Decision Tree, and Random Forest Classifier.
We concluded by learning the models, evaluating and finding out the accuracy of three models
that Random forest classification works the best for this use case, generating an accuracy of
approximately 88%
This concludes that the financial particulars/variables are efficient in analyzing how likely the
customer is a risk to the financial institution using those variables or financial details.



Conclusion
In conclusion, our research explored the complex dynamics of credit risk fraud and provided
important information for lenders. Notably, we found a significant correlation between loan goals
and default rates, highlighting the necessity of focused risk assessment techniques, particularly
for student loans and debt consolidation. Furthermore, a nuanced viewpoint is offered by the
association between the state of home ownership and default risk. Because renters are more
likely to default, lenders can create loan products that are specifically suited to their needs and
can adjust risk assessments. By comparing machine learning models like Random Forest
Classifier and Logistic Regression, we were able to identify the best model to predict loan
defaults. This emphasizes how data-driven methods may be used to accurately estimate risk.
Essentially, our research provides financial institutions with useful information to help them
improve lending practices, minimize risk, and make wise choices. The project's integration of
advanced machine learning and classical analytics advances our knowledge of credit risk
dynamics and builds a stronger lending ecosystem.
