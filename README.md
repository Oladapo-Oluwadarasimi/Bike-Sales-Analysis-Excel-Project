# Bike Sales Analysis Project

## Introduction

This project analyzes the demographic and regional factors that influence consumer's decisions to buy bikes. By analyzing data such as region, occupation, number of children, and marital status, we can adjust marketing efforts and enhance business strategy.

## Data Overview

The dataset from the sheet named "bike_buyers" provides detailed information on customers and their bike purchasing decisions. The key fields included in the dataset are:

- **ID**: Unique identifier for each customer.
- **Marital Status**: Indicates whether the customer is married (Married) or single (Single).
- **Gender**: The gender of the customer (Male or Female).
- **Income**: The income level of the customer.
- **Children**: The number of children the customer has.
- **Education**: The highest level of education attained by the customer.
- **Occupation**: The professional field in which the customer is employed.
- **Home Owner**: Indicates whether the customer owns a home (Yes or No).
- **Cars**: The number of cars owned by the customer.
- **Commute Distance**: The distance the customer commutes daily.
- **Region**: The geographic area where the customer resides.
- **Age**: The age of the customer.
- **Purchased Bike**: Indicates whether the customer purchased a bike (Yes or No).

## Screenshot of bike_buyers

![Screenshot (47)](https://github.com/Oladapo-Oluwadarasimi/Global_Layoffs_2020-2023/assets/173706258/e6bd8332-ffa4-4e79-ad71-c0143c5a5587)


## Data Cleaning
- Created a worksheet so as not to mess up the raw data.
- Removed duplicates.
- Standardized categorical variables.
- Created an age bracket using a nested IF statement:
  ```excel
  =IF(L3>54,"Old",IF(L3>=31,"Middle Age",IF(L3<31,"Adolescent","Invalid")))


## Pivot Tables 

### 1. Average Income Per Purchase
**Business Problem**: How does income level affect the likelihood of purchasing a bike?
- **Pivot Table**: Rows: Gender, Columns: Purchased Bike, Values: Average of Income

### 2. Family Structure and Bike Purchases
**Business Problem**: How does family structure impact bike purchases?
- **Pivot Table**: Rows: Marital Status, Columns: Children, Values: Count of Purchased Bike

### 3. Regional Purchasing Behavior
**Business Problem**: Are there significant regional differences in bike purchasing behavior?
- **Pivot Table**: Rows: Region, Columns: Gender, Values: Count of Purchased Bike

### 4. Education Level and Bike Purchases
**Business Problem**: How does education level affect bike purchases?
- **Pivot Table**: Rows: Education, Columns: Marital Status, Values: Count of Purchased Bike

### 5. Age and Bike Purchases
**Business Problem**: How do age brackets influence bike purchasing patterns?
- **Pivot Table**: Rows: Age, Columns: Purchased Bike, Values: Count of Purchased Bike

### 6. Commute Distance and Bike Purchases
**Business Problem**: Does commute distance influence the likelihood of purchasing a bike?
- **Pivot Table**: Rows: Commute Distance, Columns: Purchased Bike, Values: Count of Purchased Bike

  
## Dashboard

![Screenshot (51)](https://github.com/Oladapo-Oluwadarasimi/Global_Layoffs_2020-2023/assets/173706258/40fc283a-13e8-41b3-8743-181583362f7b)


### Slicers
To enhance the usability of the dashboard, the following slicers were added:
- **Marital Status**
- **Region**
- **Education**
- **Home Owner Status**
- **Gender**

These slicers allow users to filter the data dynamically and view the insights based on specific criteria.

## Key Insights

1. **Average Income Per Purchase**
   - Men typically had greater salaries than women, and those with higher incomes were more likely to purchase bikes.
   - **Solution**: Income targeting and gender income analysis.

2. **Family Structure and Bike Purchases**
   - Married people with kids bought more bikes than single individuals with kids.
   - **Solution**: Since married people with children make up a significant percentage of the client base, create family package offers or promotions specifically for them.

3. **Regional Purchasing Behavior**
   - North American women bought more bikes than in Europe and the Pacific.
   - **Solution**: 
   ***Regional Marketing***: Given that women make more purchases than men do, step up the marketing efforts in North America. Campaigns should be customized to emphasize area trends and preferences.

***International Strategy***: Look into the reasons behind the decline in bike sales by women in Europe and the Pacific, and modify the product offers or marketing tactics to better serve these areas.

4. **Education Level and Bike Purchases**

   - Single individuals with graduate degrees purchased more bikes.
   - **Solution**: Education-based campaigns and corporate partnerships.

5. **Age and Bike Purchases**
   - Older individuals bought fewer bikes.
   - **Solution**: Age-specific marketing and senior-friendly options.

6. **Commute Distance and Bike Purchases**
   - Purchases increased for commutes less than 10 miles.
   - **Solution**:
 ***Urban Commuter Focus***: Highlight the economy, environmental advantages, and ease of use of bikes as the best means of transportation for short commutes.

***Long-Distance Solutions***: To attract customers with longer commutes, develop and offer bike models intended for long-distance riding, such as electric bikes or versions with improved comfort features.

## How to Use this Project

1. Clone the repository:
   ```bash
   git clone https://github.com/Oladapo-Oluwadarasimi/Bike_Sales_Analysis.git
