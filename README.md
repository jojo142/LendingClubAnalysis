# LendingClubAnalysis
In this study, I used the historical data of loans issued on LendingClub
between April 2008 and December 2019. It contains over 1.8 million loan listings with
a total value exceeding $15 billion.

### Data Description: 
Our data comes from the Lending Club records. It includes information such as borrower information, loan details, interest rates, loan status, and other financial data from between April 2008 and December 2019. From all of the features and narrowing down to which we find to be the most important when analyzing our loans. We will first visualize each feature and remove any possible outliers that may disrupt our findings. Next, Identify correlations among these features. When initially looking at our data we assumed that the most important features would be Interest Rate, Loan Term, Credit Score, and Loan amount. We decide on these based on prior investment knowledge and decide to visualize these features and see which has a noticeable correlation. 

### Goal: 
Study how business analytics can be used to guide loan investments. The goal of this Case Study is to provide answers to these questions:
- How can I use these data when selecting which loans to invest in?
- What is the benefit of using data-driven tools relative to ad hoc investment strategies?
- What amount of return can I expect from data-driven investments on average?

### The Case Study is divided into three phases:
- Phase 1: I understood the background and the motivation. Constructed a plan for Phase 2.
- Phase 2: In this Phase of the Case Study, I performed data cleaning and data preparation for further analysis e.g. predictive analytics, followed by exploring the data to gain some insights.
- Phase 3: In this Case Study phase, I first employed predictive analytics to understand loan types and lending behavior. Then, you will employ predictive models for developing various investment strategies.

### Problem Motivation:
Our problem motivation is to Investigate the nature of different types of loans and integrate relevant information of various loans. By doing so, it can achieve the goal of maximizing loan return while minimizing risk. Our overall goal is to provide investors with our recommendation on the best distribution of loans for their portfolio. And our recommendations come from performing data analysis on various investment-related factors

<img width="516" alt="ZGq3wzO0DeZWz2HqF8c0HN9ACh9r-qCOW24jgJY8JUhpmKoD3OoPiuPeogBe6eNlCGHQoN9JYVUFI_w1PG3NejGs929fh9TsY33yQguRzXpFYcCnA-FkYPX01mmZ" src="https://github.com/jojo142/LendingClubAnalysis/assets/76130563/eb2f90dc-e144-468e-94b0-710dfdd86435">

### Skills Utilized: 
- Data Cleaning and Wrangling:  filtering and removing  rows [current loans, loans issued before a certain date]
- Data Selection and Subsetting:  selecting specific features for analysis
- Data Visualization:  visualizing data, identifying outliers, and exploring correlations.
- Statistical Analysis: calculating & interpreting default rate, and average interest rate for different loan grades.

<img width="621" alt="VnaRrYffCk2XeMBNkwG4Bhe-AwCuW5AgfhG2jtmTmw3Zom7Wl4wrd0mQPkR_fxzZ5y8ZVWSLgqpS9bd6Knzhr3Kh36ctLo4s29Im1G6PGKjNunNd2Ytu2NLpwcv-" src="https://github.com/jojo142/LendingClubAnalysis/assets/76130563/619bdaa4-0039-4e06-9eda-a59e83e0c9a0">


### The purpose of this table is to give us a deeper understanding of how we can make a well-balanced and effective investment decision.
- If we look at the results we can understand that Grades A and B show the lowest negative average returns meaning that loans in these grades are performing well compared to others essentially suggests that borrowers in these categories are more creditworthy, leading to lower default rates and increased chances of full repayment.

- Grades C and D show a moderate decrease in average returns, potentially indicating slightly higher default rates but also represent a reasonable balance between risk and return.

<img width="610" alt="mTOJmu5rFa19WA0ttdTwBQa_Qupwjn_ARwYEvCsyMTUwos2b_JA1QwuvaoQLbs2vc5tUAICiUeJT_2ByBS3qKhrvrziVznjSBeiurJQ_lc6Izhdw-Rcq6PmlazMj" src="https://github.com/jojo142/LendingClubAnalysis/assets/76130563/def80e3d-258e-4e30-ab83-06742b4c63ba">

- As we move to lower-grade loans (E to G), there is a trend of decreasing average returns, signifying an increasing risk of default.
Based on these, we understand there’s a trade-off between the potential for higher returns and elevated risk, as indicated by higher default percentages and interest rates. The higher interest rates aim to compensate for this increased risk.

![IrNrbC0dw7WJXgenWZ5Hx5BkjmJMcKZUpVyWtJGKCAb22Q_pYFmuF-EedR0gBE1-1kgyhtcoxQXX9GEXgEpLUxgyNYFQ5kvCxJRb-Jh35FTvp_Q7uqzXaMHQ-4WX](https://github.com/jojo142/LendingClubAnalysis/assets/76130563/90e45fd8-a1f0-4b94-8202-be4c346639e7)
<img width="737" alt="gI2ho0VRcK2Ywj1mCfgj56YwGYWHoN3yZVW4KsIFjq6W2jsVpyWI-iIh-NZKgJaFjKD8SIHajKgQ0QIYFZ_zuRvRBZAhwFGSo-naodhR5m9XIyuFrlByNtM4zY3m" src="https://github.com/jojo142/LendingClubAnalysis/assets/76130563/2334e7c8-06e0-45f7-a1a7-d775da234a9f">


### PCA with 14, 10, and 7 clusters without outliers.

Since our primary concern is to find loans with similar risk profiles and grouped them together, we are prioritizing the WCSS values that are lower. In this case when we do clustering without the outliers we get a lower WCSS value of 88.7 %. It indicates that the loans within each cluster are more similar in terms of their characteristics, which could be valuable for assigning grades based on loan characteristics.

<img width="910" alt="Screenshot 2023-12-30 at 4 24 39 PM" src="https://github.com/jojo142/LendingClubAnalysis/assets/76130563/238fb4b2-8d56-4e60-b117-b53f098661ad">

PCA visualizations help understand the relationship between various loan characteristics and identifying clusters of loans with similar risk profiles or borrower behaviors. 

### Correlation Heat Map: 

<img width="509" alt="bY5d5gdSMKoE1B7IrZi57rrH0EBmmzul9nInquM8Oid8aX9Yi56QhEdNeaJ8LUyhHh1yFR4HT_hih4Lr9v1vCoX8o0SW5SJUwUM1NTRyE5cHqXytjAcoltY5S6ed" src="https://github.com/jojo142/LendingClubAnalysis/assets/76130563/8e60c441-202d-4c29-abb3-c7038cb5aaea">

### Model Summary:
The fitted values represent the model's predictions for the loan amounts based on the input features and the coefficients estimated by the model. The summary shows that the range of fitted values is from 999.7 to 40003.7, indicating a wide range of predicted loan amounts. The residual error represents the average amount that the response variable (loan amount) deviates from the fitted values (predicted values) by the model. We got a value of 43.93, which means that, on average, the actual loan amounts deviate from the predicted values by approximately 43.93 units.

<img width="439" alt="S6FzfZvdxTRJsOLQKxdKApbH_y75y3tfR0YeZdTYoSSWV-WJZhPpsn3gvOXZSlV_6o20yMap0fR2paxGyX7iSf96RJAFFe1zAw_sKzAs3F_ABHugWpcyLqJj42q0" src="https://github.com/jojo142/LendingClubAnalysis/assets/76130563/84058acd-9619-4d59-a8bc-07751ade4709">

# Mean: 

<img width="364" alt="Sy6LAgQL7cS9TrbWrzEZc6tiNrNCLe8XZmtfME7e-VCwScLxp-mkY1Zu6moo2t7kRdUzUVMrc7QPEieQdv5yOHD3LCoKorCMHwAAfPCmrr6OWOrUgUWbf-qzLRij" src="https://github.com/jojo142/LendingClubAnalysis/assets/76130563/887d7627-ff0c-4d2b-a64c-0f746d28ad38">

### Scatterplot: 

<img width="521" alt="FqK9FZOhzpMQpNnxfN9KMIJJQFrDOoFIJd67jg9NWJopM6seSS5x17y9D6tSXuGsKuMjw1j9tCTdOEOtGLhuNber8K9a4Jq7Z3Uo4NQvvy_uBzwe9iqOSOCwbWO5" src="https://github.com/jojo142/LendingClubAnalysis/assets/76130563/8220a341-3eec-4d95-b636-2c9de524d627">

### Model Diagnostic: 
The residuals are the differences between the observed values of the dependent variable (loan_amnt) and the values predicted by the model. They represent the errors of the model. The smallest residual value. In this case, it's -21.170. This indicates that there is at least one data point where the observed value is much lower than the value predicted by the model. In the first quantile the value below which 25% of the residuals fall. It's -0.347, suggesting that most residuals are close to zero or slightly negative. The median is  -0.156, indicating that half of the residuals are below this value and half are above. The average of all the residuals is 0.000, suggesting that, on average, the model's predictions are close to the actual values. 

<img width="524" alt="fOsdjkynJXKQB4hjZeJnhUxMwoYmefWY65QEDWjMtpZc7yNgmDZugZ3qzam3Uq5QYp2u08jUzcO97EFPd1GgT_2K68teykbv_15_LZHnoT12QdBSRqItIfzcEGIg" src="https://github.com/jojo142/LendingClubAnalysis/assets/76130563/4673c7ab-9b63-45f2-8d9d-65df7c1a597b">

We can see in the third quartile that the value below which 75% of the residuals fall and its 0.004, indicating that most residuals are close to zero or slightly positive. The largest residual value is 21149.233, indicating that there is at least one data point where the observed value is much higher than the value predicted by the model.   

### Discussion:
Our findings revealed interesting patterns, some of which matched our expectations, and others we found surprising. The correlation analysis between loan features such as interest rates, loan amounts, credit scores, and loan statuses provided a better understanding of the factors influencing loan performance. While some relationships, such as the negative correlation between credit score and interest rate, were expected, others, like the positive correlation between loan amount and loan status, offered new insights.
While the dataset obtained from Lending Club was abundant with information, it was necessary to clean and wrangle the data to make it effective, useful, and relevant. This process involved handling irregularities, removing outliers, accounting for NAs, and converting variables into appropriate formats, all of which prepared the data for meaningful analysis.
Our analysis highlighted the trade-off between risk and return in P2P lending, as evidenced by the varying default rates and interest rates across different loan grades. While higher-grade loans (e.g., Grade A) had lower default rates, they also offered lower average returns compared to riskier loans. This trade-off presents the complexity behind loan performance and informs our decisions regarding portfolio diversification and risk management.
The evaluation of different investment strategies, including random selection, return-based models, and selecting the best-performing loans was also helpful to consider. While the "Best" strategy resulted in the highest return, it’s important to consider the practicality of this strategy, as nonetheless it brings the highest risk, and may not be always sustainable in ever-changing market and economic environments. The "Return-based" model, despite being based on analytical skills, did not perform as expected, indicating the need for further improvement.
Our analysis also has certain limitations that should be acknowledged. The assumptions made in our models, the quality of the dataset, and the inherent risks associated with P2P lending are factors we should keep in the back of our minds. Future work could focus on improving our predictive modeling, exploring alternative investment strategies, and considering additional variables that could impact loan performance.

### Acknowledgement: 
This Case Study is inspired by and based on the following:
- Provost F, Fawcett T. (2013) Data Science for Business: What you need to know about
data mining and data-analytic thinking. Sebastopol, CA: O’Reilly Media, Inc.
- Cohen MC, Guetta CD, Jiao K, Provost F. (2018) Data-driven investment strategies
for peer-to-peer lending: a case study for teaching data science. Big Data 6:3, 191–213,
DOI: 10.1089/ big.2018.0092.

### Sources:
1. https://www.lendingclub.com/
2. https://www.investmentzen.com/peer-to-peer-lending-for-investors/lendingclub
3. https://www.lendingclub.com/personal-savings/founder-savings
