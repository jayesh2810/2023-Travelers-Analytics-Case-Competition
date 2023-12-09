# Traveler-s-auto-insurance-model.
For this case competition, the task is to provide a method for predicting the claim cost for each policy.

### <ins>Dataset Description</ins>
The InsNova data set is based on one-year vehicle insurance policies from 2004 to 2005. There are 45,239 policies, of which around 6.8% had at least one claim.

### <ins>Variable Descriptions</ins>:
***id***- Policy key

***veh_value***- Market value of the vehicle in $10,000's

***exposure***- The basic unit of risk underlying an insurance premium

***veh_body***- Type of vehicles

***veh_age***- Age of vehicles (1=youngest, 4=oldest)

***gender***- Gender of driver

***area***- Driving area of residence

***agecat***- Driver’s age category from young (1) to old (6)Driver’s age category from young (1) to old (6)

***engine_type***- Engine type of vehicles

***max_power***- Max horsepower of vehicles

***driving_history_score***- Driving score based on past driving history (higher the better)

***veh_color***- Color of vehicles

***marital_status***- Marital Status of driver (M = married, S = single)

***e_bill***- Indicator for paperless billing (0 = no, 1 = yes)

***time_of_week_driven***- Most frequent driving date of the week (weekdays vs weekend)

***time_driven***- Most frequent driving time of the day

***trm_len***-  term length (6 month vs 12 month policies)

***credit_score***- Credit score

***high_education_ind***- indicator for higher education

***clm***- Indicator of claim (0=no, 1=yes)

***numclaims***- The number of claims

***claimcst0***- Claim amount





### Chosen methodology for claim cost predictions:

***Two-step model:***
The first step uses a count model to predict the frequency of claims.
The second step employs a Regression model to estimate the severity of claims.

For the classification model, we have used GLM with Poisson distribution.\
For the regression model, we have used the GLM with inverse Gaussian distribution.

### Variable selection methodology:
1.) Forward/Backward selection.\
2.) P-value significance.\
3.) Benchmarking trial and error.\
4.) Research and development.
 

### Model evaluation metrics:
1.) Normalized Gini Coefficient\
2.) 10 fold cross validation\
3.) Average gini across all folds\
4.) Bootstrapping for the reliability of model coefficients.
