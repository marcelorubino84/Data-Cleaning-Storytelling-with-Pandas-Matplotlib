# Data Cleaning & Storytelling with Pandas & Matplotlib Overview:

#### The purpose of this project is to make sense of messy data given in CSV files and extract insight in order to answer some business questions.

* **Data cleaning and quality**: 4 files are cleaned and then transformed in order to answer some business questions
* **Data visualization**: Using matplotlib and seaborn to create plots that convey a clear message.

#### The main question:

* Is it beneficial for the company to discount products?

#### Aspects needed to clarify for business purposes:

* How products should be classified into different categories to simplify reports and analysis
* What is the distribution of product prices across different categories
* How many products are being discounted
* How big are the offered discounts as a percentage of the product prices
* How seasonality and special dates (Christmas, Black Friday) affect sales
* How could data collection be improved

## Code and resources:

**Python Version:** 3.8

**Packages:** pandas, seaborn, matplotlib

**Enviroment:** google colab

**Data:** Obtained from [WBS coding school](https://www.wbscodingschool.com/)

## Data Cleaning

After obtaining the data, I needed to clean it up so that it was usable for my analysis. I made the following changes and created the following variables:

* Deleting missing values from in the 'orders' DataFrame, since they represented only 0.0022% of the rows
* Change the datatype of "created_date" and "date" column in orders and orderlines dfs to datetime.
* Change the datatype "unit_price" to numeric in orderlines df
* Eliminating two dots and commas in "unit_price" and "price" column, for the purpose of having smooth data.
* Change datatype of "price" and "promo_price" in products, to numeric
* Dropped missing values from products column

## Quality assesment of the data

* Changing pandas display format
* Excluding unwanted orders, and only selecting completed orders for this analysis
* Made a list of the order_id's of the Completed orders
* Changing the DataFrames from _qu, so we can distinguish between the data that has been cleaned, and that which has been quality controlled
* Keep only the orders that are present in both orders and orderlines
* Excluding orders with unknown products

## Creating categories for all the products

* There were no categories created in the given data, just products
* 29 product categories were created in order to group all similar products

The graph below shows the average price of all the products in each category:

![out](https://user-images.githubusercontent.com/99658869/215459421-48e1e846-2e62-4c5e-b7a2-678db6bad94e.png)

## Checking the 10 most sold brands:

![out2](https://user-images.githubusercontent.com/99658869/215460715-87f711ec-feca-4ebb-96b0-1f76d4af22d6.png)


## Analysis

The purpose of the analysis is to make sense of the data, onced cleaned and organized, in order to find insights and answer the business question:

* **Is it beneficial for the company to discount products?**


* (This readme is continously updating) Not finished yet!





