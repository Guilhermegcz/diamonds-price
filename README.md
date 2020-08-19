# diamonds-price
Using a diamonds dataset with price and other variables to predict the price of new diamonds types.  

# tools
- Python, Jupyter Notebook, Pandas, Scikit-learn, Seaborn, Matplotlib

# data source
https://www.kaggle.com/shivam2503/diamonds

# data cleaning
Check nan values  and droped outliers

# first analysis
The model is structured initially  analyzing the price based in carats.   
From that, categories such as clarity, color and cut are analyzed together to identify any relationship.  
![alt text](https://github.com/Guilhermegcz/diamonds-price/blob/master/images/price_carat.png)

It was noted that the diamond's  clarity  contribute for a variation in prices.  
![alt text](https://github.com/Guilhermegcz/diamonds-price/blob/master/images/price_carat_clarity.png)

![alt text](https://github.com/Guilhermegcz/diamonds-price/blob/master/images/price_carat_color.png)

![alt text](https://github.com/Guilhermegcz/diamonds-price/blob/master/images/price_carat_cut.png)


# linear regression model
For the final model, the database was separated by clarity.   
It was used a linear regression for each type of clarity.  
Finally for the smaller diamonds, it was noticed some values resulted in negative values. As a solution for that question, a new model was proposed for diamonds with a price below than 300.   
This new model brought greater precision to the lower values.  
![alt text](https://github.com/Guilhermegcz/diamonds-price/blob/master/images/price_carat_reg.png)

![alt text](https://github.com/Guilhermegcz/diamonds-price/blob/master/images/linear_reg_clarity.png)


# Issues
The projection does not follow the data curvature.

# Future resolutions
Transform carat and price values applying log.




