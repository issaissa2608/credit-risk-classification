# credit-risk-classification

Through this analysis, I used logical regression models to identify the creditworthiness of borrowers from a peer-to-peer lending service. This dataset included
fields loan size, interest rate borrower income, debt to income, number of accounts, derogatory marks, and total debt. I used this to predict whether a loan was
healthy or high-risk. I started by separating labels and features into x and y variables to analyze this data. Then I used sklearn to split the data into training
and testing datasets using the train_test_split module. Using this I created model 1 (results below). Due to the imbalance in the data, I resampled the data. This
is used to create model 2. Then I was able to compare the two models and analysis which would provide better results.

Machine Learning Model 1 (Description of Model 1)

Accuracy: 99%

  o	Healthy Loans:
	
    o	Precision: 1
		
    o	Recall: 0.99 
		
  o	High-Risk loans:
	
    o	Precision: 0.85
		
    o	Recall: 0.91
		
		
Machine Learning Model 2 (Description of Model 2)

Accuracy: 99% 

  o	Healthy Loans:
	
    o	Precision: 1
		
    o	Recall: 0.99 
		
  o	High-Risk loans:
	
    o	Precision: 0.84
		
    o	Recall: 0.99
		

Overall, both models perform well when predicting healthy loans. Using resample data, the second model increased the recall of high-risk loans. However, this 
precision has not changed. I would recommend the use of the second model as it has a high rate of return for high-risk loans. As miscalculating high-risk loans is
more of a risk it would be better to go with better accuracy for high-risk over healthy loans.



