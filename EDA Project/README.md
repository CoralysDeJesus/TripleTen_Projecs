# TripleTen EDA Project

### Instacart Orders

The goal of the project was to clean the data and prepare a report that gives insight into the shopping habits of Instacart customers, featuring data visualization to help communicate results.

#### The Data

The data was spread across five files:

- `instacart_orders.csv`: each row corresponds to one order on the Instacart app
    - `'order_id'`: ID number that uniquely identifies each order
    - `'user_id'`: ID number that uniquely identifies each customer account
    - `'order_number'`: the number of times this customer has placed an order
    - `'order_dow'`: day of the week that the order placed (which day is 0 is uncertain)
    - `'order_hour_of_day'`: hour of the day that the order was placed
    - `'days_since_prior_order'`: number of days since this customer placed their previous order
- `products.csv`: each row corresponds to a unique product that customers can buy
    - `'product_id'`: ID number that uniquely identifies each product
    - `'product_name'`: name of the product
    - `'aisle_id'`: ID number that uniquely identifies each grocery aisle category
    - `'department_id'`: ID number that uniquely identifies each grocery department category
- `order_products.csv`: each row corresponds to one item placed in an order
    - `'order_id'`: ID number that uniquely identifies each order
    - `'product_id'`: ID number that uniquely identifies each product
    - `'add_to_cart_order'`: the sequential order in which each item was placed in the cart
    - `'reordered'`: 0 if the customer has never ordered this product before, 1 if they have
- `aisles.csv`
    - `'aisle_id'`: ID number that uniquely identifies each grocery aisle category
    - `'aisle'`: name of the aisle
- `departments.csv`
    - `'department_id'`: ID number that uniquely identifies each grocery department category
    - `'department'`: name of the department

The data was taken from Kaggle, modified, and provided by TripleTen.

#### The Process
The initial phase of the project involved pre-processing the data, where the initial data impression is obtained and cleaned up. This was done by identifying and addressing duplicate and missing values and their context, which in turn allowed for determining their relevance to the data. The second part featured data analysis through the use of descriptive statistical methods. Pivot tables, merging and slicing of DataFrames, application of aggregate functions, and libraries **pandas** and **matplotlib** were all utilized in this analysis.
    
The project’s current progress status is: complete.

### Results

For a summary of findings, please scroll to the bottom of the Jupyter Notebook or see below:

-----------

> The project started with assessing for missing and duplicate values and taking the proper action necessary (i.e., dropping or replacing missing and duplicate values) to proceed with data analysis. I addressed several key questions and discovered ideal times, days, and products to center due to the frequency of purchases made.
> 
> To summarize our findings, we found:
> 
> The top 5 hours for shopping are 10AM, 11AM, 3PM, 2PM, and 1PM, respectively. The average hour of the day when orders were placed is approximately 13.45 which suggests that, on average, orders are placed around mid-afternoon (i.e. between 1PM - 2PM).
> Functioning under the assumption that the Day of Week scale corresponds to Sunday = 0 and Saturday = 6, the top 3 days for shopping are Sunday, Monday, & Tuesday. The average day of the week when orders were placed is approximately 2.78 which suggests orders are, on average, placed between Tuesday and Wednesday.
>
> The two most common waiting periods observed before customers place another order are approximately one month and one week. The average time people wait between orders is approximately 10 days.
> 
> When examining the distributions of the time of day for when orders were placed on Wednesday versus Friday, a difference in the number of orders placed on the two days was seen. That is, Fridays see more orders placed between 10AM and 3PM compared to Wednesdays. But, for the most part, both days have a similar distribution.
> 
> When examining the distributions of the number of orders placed per customer, it was found that of the 157k+ customers who have placed orders through Instacart, on average, each customer placed approximately 17 orders.
> 
> When searching for the top 20 popular products sold through the Instacart app, it was found that the number one item sold were bananas (non-organic and organic, respectively) followed by organic strawberries, organic baby spinach, and organic hass avocados. The number of organic items among the top 5 products could reveal some information on the preferences of customers who place orders in the Instacart app.
> 
> When investigating how many items people typically buy in one order, it was found that on average, customers typically buy 10 or so items in one order. 25% of customers buy approximately 5 items or fewer; 50% of customers buy approximately 8 items or fewer; and 75% of customers buy approximately 14 items or fewer.
> 
> Finally, when asking about the top 20 items that were reordered most frequently, it was found that top 5 items were the same top 5 among the top 20 popular products.



