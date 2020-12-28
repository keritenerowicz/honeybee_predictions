# honeybee_predictions
A dataset of honey production was analyzed to predict the value of production (linear regression) and the state from which data came (kNN). After a review of the data, the year from which data was collected was also predicted (kNN).
___

#### Problem
The first problem is "What is the value of honey production for each state?". This is a regression problem which aims to clarify a relationship between environmental factors (location, honey producing colonies, yield per colony, production, year) and financial factors (stocks on December 15th, average price per pound). I will build a supervised machine learning model (linear regression) to predict this using data from all columns except the 'Value of production' column. 

The second problem is "How does honey production vary by each state?". The second model will be a classification model (kNN classifier) that determines what state each set of values (row) the data was taken from. It will predict this based on the same set of columns + 'Value of production' - 'State'.

#### Hypothesis
For the regression model, I believe that the following columns will be useful because they all influence the value of production based from either an envionmental or financial standpoint:

Environmental:
- State
- Honey producing colonies
- Yield per colony
- Production
- Year

Financial:
- Stocks December 15
- Average price per pound

For the classification model, I expect all columns except 'State' will be useful because that is as much data as possible for the predictions to include without the corresponding states.
