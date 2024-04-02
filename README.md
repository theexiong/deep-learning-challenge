# deep-learning-challenge

Overview
This assignment's purpose was to create a model that would be able to predict if a charity was successful or not successfful. This consisted of dropping columns, binning values together and using get_dummies() to convert categorical data. 

Results
Data Proprocessing: 
    
    -Target variable was the IS_SUCCESSFUL column
    
    -Features were all other columns (EIN, NAME, APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS and ASK_AMT)
    
    -Variables that should be removed are EIN, NAME, SPECIAL CONSIDERATIONS and STATUS.

    

Compiling, Training, and Evaluating the Model

For the optimized model, I chose four hidden layers.
    
    1. units=40, activation=relu, input_dim=35
    2. units=35, activation=relu
    3. units=25,, activation=relu
    4. units=15, activation=tanh

-At first I had chose three hidden layers but the model was still not reaching 75%, so I upped it to four hidden layers.

-I also tried using all relu activations but it was still predciting only 72%, so I added the tanh to test if it would improve the model.

-I was not able to achieve the target model performance. The max percentage was around 72%. 

-In order to increase my model's performance, I dropped the SPECIAL CONSIDERATIONS and STATUS variables. I also added bins for the INCOME_AMT variable. I increased the number of hidden layers and included different activation functions as well.



Summary

Overall this deep learning model did not achieve the target percentage of 75%. The max percentage this model achieved was 72%. A different model with more layers and epochs may predict this dataset better. If there were more variables included that were more relevant to the outcome of the charity, that would help tremendously. I feel that the data that was supplied just did not really define if a charity would be successful or not. The pattern is not defined enough to predict correctly. 
