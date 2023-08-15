# Housing-in-Colombia

![](colombia.jpg)

## Intrduction
Our objective for this project was to develop a machine learning model that accurately predicts house prices under $400,000 in Bogotá, Colombia. We utilized Linear Regression and Ridge Regression models to achieve this and evaluated our results using the Mean Square Error (MSE) metric.

## Dataset and Data Preprocessing 

The dataset we used was scrapped from the real estate website [Properati.com](https://properati.com/).

In the data preprocessing phase, We used the SimpleImputer transformer to deal with the missing values. And to deal with categorical feature encoding, we used the OneHotEncoder transformer.

We took several steps to optimize our dataset. We clipped the outliers and split the lat-lon feature into separate columns for latitude and longitude, converting their data type from object to float. Additionally, we removed features with high cardinality, leakage concerns, and multicollinearity. The whole process is written in a wrangle function.

## Exploratory Data Analysis

Our focus was on studying the correlation between the price of a house and three specific characteristics.

### House Size
It is clear that size and price are closely linked, as demonstrated in this plot:
![](area_price.png)
