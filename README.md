## Project Overview

For this project, I will use multiple linear regression modeling to analyze house sales in a northwestern county.

## Business Objective

I was hired by West Seattle Realty (a local real estate agency) to provide insights to better their speciality in helping buyers and sellers navigate the King County residential home market.

Link to local agency: https://westseattlerealty.com/west-seattle-realty

### The Data

This project uses the King County House Sales dataset, which can be found in  `kc_house_data.csv` in the data folder in this assignment's GitHub repository. The description of the column names can be found in `column_names.md` in the same folder. I filtered out the dataset into the following:

* Price: $78,000-$5,570,000
* Bedrooms < 10
* Bathrooms < 4
* Floors < 3
* Square Foot Living: 370 sqft-5990 sqft

And then the rest of the columns are:

* `date`
* `view`
* `sqft_above`
* `sqft_basement`
* `yr_renovated`
* `zipcode`
* `lat`
* `long`
* `sqft_living15`
* `sqft_lot15`

## Modeling
Regression Modeling was used to predict the house prices

# Conclusion

## Findings
**Top Features correlated with price:**

* Zipcodes 98112, 98039, & 98004
* Square foot living
* Grade
* Condition
* View

**Interpretations:**
* The top three coefficients for Zipcodes 98112, 98039, and 98004 are 1.04, 1.27, and 1.1 repsectively. This means that price will increase in that location by 10.4%, 12.7%, and 11%.
* The coefficient for sqft_living is .17 meaning for every 100 sqft added, the price will increase by 1.7%
* The coefficient for the highest grade is .44 meaning if the house is mansion grade, the price will increase by 4.4%
* The coefficient for the top condition is .12 meaning if the house is in very good condition, the price will increase by 1.2%
* The coefficient for the top view is .2 meaning if the view is considered excellent, the price will increase by 2%

## Recommendations
* If you are selling your house or increase the value of it, try and increase the square footage of the house (whether it's adding an addition to the property)
* Target homes in specific areas (such as Zipcodes 98112, 98039, or 98004) to buy and resell since it has proven to be the biggest factor effecting price
* If you are selling, improve the quality of your house by investing in upgrades. Grade has proven to be a huge factor correlating with the price

## Future Work

* Look at location (lat/long) to see how much of a factor it plays into the price of a house.
* Gather data from different school districts in KC to see if there is a relationship with prices of a house and the quality of schools.
* Get before/after stats on renovated houses to see the frequency houses are being renovated and if it has an effect on prices

