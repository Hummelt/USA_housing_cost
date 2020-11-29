# USA housing cost
![housing](https://static.wixstatic.com/media/7090dd_ba53ce486fda4a8683d525b577bc4ab9~mv2.gif)

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
**What is the main contributor to the house cost?**

![Heatmap](https://github.com/LarsTinnefeld/USA_housing_cost/blob/main/Correlation%20heatmap.png?raw=true)

The correlation heatmap shows that the income area plays the biggest role when it comes to price. "Location! Location! Location!"

**How is the cost for houses distributed?**

![Distplot](https://github.com/LarsTinnefeld/USA_housing_cost/blob/main/Price%20distribution.png?raw=true)

The mean house price is round about 1.25M dollars. The chart shows an evenly distribtuted Gauss distribution.

**How accurate can predictions for house prices be made with linear regression?**

![Coefftable](https://github.com/LarsTinnefeld/USA_housing_cost/blob/main/Coeff%20table.PNG?raw=true)

The above table reflects the coefficents as the result of the analysis output.
