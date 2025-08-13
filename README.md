# Portuguese-Banking
Subscription Rate Modeling
Findings
Business Problem
As it is costly to execute phone campaigns to get customers to sign up for new products, the business is trying to understand which types of customers may be likely to subscribe to a bank term deposit after receiving a phone call, and if this can be modeled effectively
Historically, 12.5% of all campaign calls have led to a customer subscribing to the bank term deposit. Ideally, if the business was to run this again on a new set of customers they would want to target customers more likely to sign-up (higher accuracy) but they would also not want to miss (not call) customers that would have signed if they had been call (high recall). Depending on the cost of the calls and the incremental profits received when a customer subriscbes to a bank term deposit will help us shape us how well our model needs to perform for it to be profitable to execute. 

Results and Next Steps
Logistic Regression & Decision Trees catch most of the subscribers (>86%) vs KNN & SVM (~38%), which given the business objective is most important. They have a lower precision than KNN&SVM, which means that false positives will be slightly higher, but depending on the calls of making these campaigns, could be a worthwhile investment nonetheless
The results of the Logistic Regression are also very interpretable (vs some of the other models) so if the business were to encounter another group of customers where they knew some of these same data (but maybe not all) it could likely make more informed decisions on how to target to cross sell another banking product. 
One issue is that variables like Month and Call Duration are strong predictors of subscription but it may be likely that longer calls lead to subscription because the customer is interested in the product already. The month timing may something to look deeper into and if it correlates with when the consumer price index was higher which shows a strong correlation with subscription rate.
Next steps would be to use the findings from the Logistic Regression to target a new set of customers for the same banking product or target a subset of these customers with a different banking product.
