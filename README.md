<h1>Diwali Sales Analysis</h1>

In the following Diwali Sales Analysis project, we aim to analyze the Diwali Sales Data to improve customer experience and Sales. For the Diwali Sales Analysis project,the focus is on examining the sales data to get actionable insights into customer behavior, purchasing patterns and product preferences during the festive season. By exploring trends and identifying key drivers of sales,the project aims to optimize marketing strategies, enhance customer experience, and boost overall sales performance.

## Dataset

Our dataset is a csv files comprising of the following columns:

- user_id
- cust_name
- product_id
- gender
- age
- name
- marital_status
- state
- zone
- occupation
- product_category
- orders
- amount
- status
- unnamed

## Data cleaning and Processing

First step was to get a deeper understanding of the data we are dealing with. Our data contained some important attributes such as gender, age, marital_status, occupation, state, zone on which insights could be gained.

Then we found number of non-null values present in each columns and we found that some columns like `status` and `unnamed` had zero non-null values so we removed them.

In `amount` column we found 12 null values. So to deal with these null values, we first found the mean amount for each product category and then replaced the `NA` values with mean for that category.

Then we renamed column `Marital_Status` to `Married`.

Then we designed a function to categorize the age and then applied the function to the `Age` column to create a new column called `Age_Group`.

## Exploratory Data Analysis

### The following charts were created during our EDA :

- Plotting a bar chart for gender and it's count.
- Bar chart for Total Amount spent based on Gender.

_From the first 2 visualizations we inferred that most of the buyers are females and even the purchasing power of females are greater than men_

- Plotting a bar chart for `Age_Group` and it's count and dividing each `Age_Group` based on it's `Gender`
- Plotting a bar chart `Total_Amount` spent based on each `Age_Group`.

_From the next 2 visuals we conclude that the most of the buyers are of age group between 26-35 yrs and this age group has higher purchasing power as well_

### _For State_

- Plotted a bar chart for Total Number of Orders from top 10 states and Total Amount/Sales From top 10 states.

_From above graphs we can see that most of the orders & total sales/amount are from Uttar Pradesh, Maharashtra and Karnataka respectively_

### _For Marital Status_

- Plotted a bar chart for Total Number of Orders by `Gender` and Total Amount/Sales by `Gender` dividing each of the marital status into Male and Female.

_From above graphs we can see that most of the buyers are married (women) and they have high purchasing power_

### _For Occupation_

- Plotted a bar chart for Total Number of Orders by `Occupation` and Total Amount/Sales by `Occupation` of people.

_From above graphs we can see that most of the buyers are working in IT, Healthcare and Aviation sector_

### _For Product Category_

- Plotted a bar chart for Total Number of Orders by `Product Category` and Total Amount/Sales by `Product Category` of people.

_From above graphs we can see that most of the sold products are from Food, Clothing and Electronics category_

## Conclusion

_Married women age group 26-35 yrs from UP, Maharastra and Karnataka working in IT, Healthcare and Aviation are more likely to buy products from Food, Clothing and Electronics category_
