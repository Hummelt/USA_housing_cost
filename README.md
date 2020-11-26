# USA housing cost
![city_image](https://images.unsplash.com/photo-1601332071777-583f25aa864d?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1422&q=80)

1. [The US house market](#business)
2. [Task and motivation](#motivation)
4. [Approach](#aproach)
4. [The Data](#data)
3. [Data preparation](#preparation)
4. [Modelling](#modelling)
5. [Evaluation](#evaluation)

## The US house market <a name="business"></a>
Real estate economics applies economic techniques to describe, explain and predict patterns of prices, supply an demand for the US real estate market. A detailed article can be found in [Wikipedia](https://en.wikipedia.org/wiki/Real_estate_economics). Especially in the light of the ups and donwns of the house prices there is a interest to get a good oversight and grip on the cost situation.

## Task and motivation <a name="motivation"></a>
This analysis has the aim to develop a method to predict the cost of a house based on a range of input heatures. Initially, a range of features will be reviewed and compared with the aim to find patterns and correlations.
Questions to clarify in detail:
1) What is the main contributor to the house cost?
2) How is the cost for houses distributed?
3) How accurate can predictions for house prices be made with linear regression?

## Approach <a name="approach"></a>
Success criteria for this analysis stage is to answer the above questions with the available data and information. To archive this the following steps and techniques are applied:
- Data import and wrangling
- Exploratory data analysis
- Linear regression

Analysis software and libraries:
- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- scikit-learn

## The data <a name="data"></a>
The data stems from Kaggle and can be found [here](https://www.kaggle.com/aariyan101/usa-housingcsv).

**The dataset:**
| #   |Column                       | Non-Null Count | Dtype  |
|---  |:------------------------:   |:--------------:|-----:  |
| 0   |Avg. Area Income             | 5000 non-null  | float64|
| 1   |Avg. Area House Age          | 5000 non-null  | float64|
| 2   |Avg. Area Number of Rooms    | 5000 non-null  | float64|
| 3   |Avg. Area Number of Bedrooms | 5000 non-null  | float64|
| 4   |Area Population              | 5000 non-null  | float64|
| 5   |Price                        | 5000 non-null  | float64|
| 6   |Address                      | 5000 non-null  | object |

## Data preparation <a name="preparation"></a>
The notebook "Linear Regression.ipynb" contains a complete procedure of data checks and cleaning. Applied verification methods:
- Missing data check
- Duplicate records

## Modelling <a name="modelling"></a>
For the predictive analysis part linear regression was applied. Input variable were 'Avg. Area Income', 'Avg. Area House Age', 'Avg. Area Number of Rooms', 'Avg. Area Number of Bedrooms', 'Area Population', 'Price', 'Address'. The output (the predicted value) was the 'Price'.

## Evaluation
