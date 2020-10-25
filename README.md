# Customer-Lifetime-Value-Prediction
In this project, I have used data analytics to determine the Customer Lifetime Value, an upper limit on spending to acquire new customers.

In marketing, customer lifetime value (CLV or often CLTV), lifetime customer value (LCV), or life-time value (LTV) is a prediction of the net profit attributed to the entire future relationship with a customer. Customer lifetime value can also be defined as the dollar value of a customer relationship, based on the present value of the projected future cash flows from the customer relationship. Customer lifetime value is an important concept in that it encourages firms to shift their focus from quarterly profits to the long-term health of their customer relationships. Customer lifetime value is an important number because it represents an upper limit on spending to acquire new customers. For this reason it is an important element in calculating payback of advertising spent in marketing mix modeling.

# Dataset
The dataset is provided in CSV format and contains roughly 4,200 transactions records. Each row in the dataset represent a single transaction.

# Steps performed:

Step 1: Understanding the dataset
  1. Are there any missing values in the dataset?
  2. What is the range of dates in the dataset?
  3. How many unique customers are there in the dataset?
  4. Profile the data to give the standard descriptive statistics for the Amount field. What is the min, max, variance, and standard deviations?
  5. Do transaction amounts in general increase over time (perhaps due to inflation)?

Step 2: Explore the dataset 
  Outlier Detection, Null Value Handling

Step 3: Determine origin year of customers
  Some of the underlying customers are brand new and others have been customers for almost five years. Obviously the newer customers will have (generally) spent less on average than the old ones. So, we need to separate the customers into groups based on how long ago they were acquired (e.g. customers acquired in 2010, vs customers acquired in 2011, ...).

Step 4: Calculate cumulative transaction amounts
  calculate the cumulative transaction amounts for customers in each group of origin year.
  
Step 5: Calculate cumulative transaction amounts
  calculate the number of new customers by origin year in each year
  
Step 6: Historic CLV
  Dividing the Amount.cmltv triangle by the NewCustomers.cmltv triangle will give us annual measurements of the cumulative amount spent per customer in each group of annually acquired customers. This is also known as Historic CLV.
