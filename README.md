# Exploring-Food-Kiosk-Data-Trends-and-Analysis
## Author: Manjusha Motamarry

## Introduction

This report presents an exploratory data analysis (EDA) of the Food Kiosk dataset. The analysis includes data preprocessing, univariate and multivariate analyses, and key insights derived from the dataset.

---

## Data Overview

The datasets include information on sold items, transactions, and date-specific attributes. A brief summary of these datasets and their structure is provided.

---

## Data Preprocessing

Data preprocessing involved merging the datasets and handling missing values. Feature engineering was also performed to add new variables, such as days from the beginning of the dataset and indicators for holidays.

### Include Image: Merged Data Structure
![image](https://github.com/Manjusha-26/Exploring-Food-Kiosk-Data-Trends-and-Analysis/blob/main/Visualizations/Data.jpeg)

---

## Univariate Analysis

### Quantity Distribution

The histogram of quantities sold shows the distribution of sales, highlighting the frequency of popular item quantities.

**Image Placeholder: Quantity Distribution**
![image](https://github.com/Manjusha-26/Exploring-Food-Kiosk-Data-Trends-and-Analysis/blob/main/Visualizations/DensityPlotQuantity.jpeg)

---

### Price Distribution

The density plot of prices provides insights into the range and skewness of the price distribution.

**Image Placeholder: Price Distribution**
![image](https://github.com/Manjusha-26/Exploring-Food-Kiosk-Data-Trends-and-Analysis/blob/main/Visualizations/PrinceDensity.jpeg)

---

## Multivariate Analysis

### Price vs Quantity

A scatter plot with a LOESS curve demonstrates the relationship between price and quantity, indicating price elasticity and trends in consumer demand.

**Image Placeholder: Price vs Quantity**
![image](https://github.com/Manjusha-26/Exploring-Food-Kiosk-Data-Trends-and-Analysis/blob/main/Visualizations/PriceVsQuantity.jpeg)

---

### Sales During Holidays

Boxplots comparing sales on holidays and non-holidays reveal significant differences in sales patterns, with lower sales during holiday periods.

**Image Placeholder: Holiday Sales**
![image](https://github.com/Manjusha-26/Exploring-Food-Kiosk-Data-Trends-and-Analysis/blob/main/Visualizations/holidayvsquantity.jpeg)

---

### Temperature vs Quantity

Scatter plots and trendlines highlight how weather conditions influence sales, showing a correlation between temperature and quantity sold.

**Image Placeholder: Temperature vs Quantity**
![image](https://github.com/Manjusha-26/Exploring-Food-Kiosk-Data-Trends-and-Analysis/blob/main/Visualizations/QuantityvsTemp.jpeg)

---

### Monthly Sales Trends

Bar plots of monthly sales volumes highlight seasonal trends, with peaks and troughs reflecting consumer behavior across different times of the year.

**Image Placeholder: Monthly Sales Trends**
![image](https://github.com/Manjusha-26/Exploring-Food-Kiosk-Data-Trends-and-Analysis/blob/main/Visualizations/MonthTransaction.jpeg)

---

## Key Insights

1. Sales are generally higher during non-holiday periods.
2. Warmer weather conditions correlate with increased sales volumes.
3. Monthly sales trends suggest seasonality in consumer purchasing behavior.
4. Prices and quantities sold exhibit a non-linear relationship.

---

## Conclusion

This analysis provided valuable insights into the Food Kiosk dataset. These findings can inform pricing strategies, inventory management, and targeted marketing efforts. Further analysis may involve predictive modeling or detailed segmentation of consumer behavior.

---

## Appendix

### Data Summary

A detailed summary of all datasets is provided for reference.

### Sold dataset - Datasets/Cafe+-+Sell+Meta+Data.csv

Information about Sold df: 

SELL_ID: a categorical variable, identifier of the combination of items that is contained in the product.

SELL_CATEGORY: “0” identifies single products; the category “2” identifies the combo ones.

ITEM_ID: a categorical variable, identifier of the item that is contained in the product 1-to-1 relation with item_name.

ITEM_NAME: a categorical variable, identifying the name of the item

### Transaction dataset - Datasets/Cafe+-+Transaction+-+Store.csv

Information about Transaction df: Important: It’s supposed the PRICE for that product in that day will not vary.

In details: CALENDAR_DATE: a date/time variable, having the time always set to 00:00 AM.

PRICE: a numeric variable, associated with the price of the product identified by the SELL_ID.

QUANTITY: a numeric variable, associated with the quantity of the product sold, identified by the SELL_ID.

SELL_ID: a categorical variable, identifier of the product sold.

SELL_CATEGORY: a categorical variable, category of the product sold.

### Dates dataset - Datasets/Cafe+-+DateInfo.csv
Information about Dates df:
CALENDAR_DATE: a date variable, associated with the date of the transaction

YEAR: a numeric variable, associated with year of the trasaction

HOLIDAY: a string variable, associated with the name of the Holiday, if it is not a holiday then N/A

IS_WEEKEND: 1: Yes, 0 : No

IS_SCHOOLBREAK: 1 : Yes, 0 : No

AVERAGE_TEMPERATURE: a numeric variable, associated with the average temperature of the day

IS_OUTDOOR: 1 : Yes, 0 : No
