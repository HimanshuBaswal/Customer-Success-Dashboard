# Customer-Success-Dashboard

## Problem Statement:
The Customer Success team currently lacks a centralized view of key customer health metrics, making it difficult to proactively identify and address potential issues that could lead to churn. How can we leverage customer success data to gain insights into sales performance, customer acquisition channels, delivery efficiency, customer satisfaction, and product trends to optimize business strategies and improve overall customer experience?

## About the Data:
This dataset represents sales transactions from a business over a period of six days, starting from January 1, 2017, to January 6, 2017. The data includes information about customer acquisition, product details, sales performance, delivery performance, returns, and customer satisfaction.

| Fields | Description |
| ------| -------| 
| 1) Date: | The date of the sales transaction.|
| 2) Customer Acquisition Type: | Indicates how the customer was acquired, categorized as "Ad" (through advertisements), "Returning" (returning customers), and "Organic" (organic means, such as search engines or word-of-mouth).| 
| 3) State: | The U.S. state where the sales transaction occurred.|
| 4) Product: | The product involved in the transaction, labeled as Product 1, Product 2, etc.| 
| 5) Price: | The price of a single unit of the product.| 
| 6) Units: | The number of units sold in the transaction.| 
| 7) Revenue: | The total revenue generated from the transaction, calculated as Price x Units.| 
| 8) Delivery Performance: | Indicates whether the delivery was on-time or delayed.| 
| 9) Return: | Indicates whether the product was returned by the customer (yes or no).| 
| 10) Customer Satisfaction: | A measure of customer satisfaction on a scale, represented by both a numeric value and a descriptive label (e.g., (2) low, (5) very high).| 

## Approach:

### Visual 1: Sales Line
- **Technique:** Pivot Chart: Years and Date as Rows & Revenue for Values
- **Data:** Revenue over the Years (Months)
- **Chart:** Line Chart

### Visual 2: Sales Map
- **Technique:** Pivot Chart: State as Columns & Revenue for Values
- **Data:** Revenue by each State
- **Chart:** Map Chart

### Visual 3: Delivery Performance Doughnut
- **Technique:** Pivot Chart: Delivery Performance as Rows & Revenue (Count) for Values & Percentage of delayed orders
- **Data:** Delivery Performance Ratio (on-time and delayed)
- **Chart:** Doughnut Chart & Percent of on-time delivered orders 

### Visual 4: Return Rate Doughnut
- **Technique:** Pivot Chart: Return as Rows & Revenue (Count) for Values & Percentage of returned orders
- **Data:** Return Rate (no and yes)
- **Chart:** Doughnut Chart & Percent of returned (yes) orders 

### Visual 5: Customer Acquisition Waterfall
- **Technique:** Pivot Chart: Customer Acquisition Type as Columns & Revenue (Count) for Values
- **Data:** Customer Acquisition Type by Count
- **Chart:** Waterfall Chart (Total is gray)

### Visual 6: Customer Satisfaction Bar
- **Technique:** Pivot Chart: Customer Satisfaction as Columns, Product as Rows & Revenue (Count) for Values
- **Data:** Customer Satifaction levels (ordinal) by product (sorted descending)
- **Chart:** Horizontal Stacked Bar Chart

## Dashboard:
### Sales: 
  -  Sales over time
  -  Sales by State
### Deliveries: 
  -  Orders delivered on time (%)
  -  Orders return rate (%)
### Customer Acquistion: 
  - Waterfall Chart of Customer Aquisition type and their revenue
### Customer Satisfaction: 
  - Customr Satisfaction Stacked Bar Chart by each product
### Slicers: 
  - Slicer 1: Customer Acquistion Type
  - Slicer 2: State
  - Slicer 3: Product
  - Slicer 4: Years

## Insights:
### Product 1
#### 2017
  - Return rate was ideal at 8%, On-time deliveries were 64% (9% below the standard).
  - On-time delivery was lowest at 60% for Customer acquired from Ads.
  - There was a dip in sales in Feb and Mar and then it fluctuated between 80k-125k throughout the year.
  - All the customer acquistion types were nearly the same count.
  - Customer satisfaction was 28% in low and very low.
  - North Carolina was the best performing state (178K) and Mississippi was the lowest (142K).
  - For orders from customers who were acquired by "Ads", Alabama generated the most sales (92K), and the customer satisfaction was 36% in the lower region.
  - Florida had 38% lower customer satisfaction rate followed by Mississippi at 36%.

#### 2018
  - High Return rate at 11%, On-time deliveries were 68% (3% below the standard).
  - High return rate for customers from ads at 13%.
  - June and Sept saw the lowest sales around 66K.
  - Customer satisfaction was 23% in lower region overall.
  - Alabama was the best performing state (170K) and Georgia was lowest (147K).
  - For orders from customers who were acquired by "Ads", Mississippi generated the most sales (60K), and the customer satisfaction was 15% in the lower region.
  - For the same acquired type, Florida had a highest satisfaction rate at 38% in lower region.
  - The State of Tennessee saw 16% returns while south carolina saw 2% returns.

#### 2019
  - Highest return rate at 13%. on time deliveries fell to 65%.
  - Customer from ads and the returning ones had high product return rate around 14%.
  - Sales fell to low range during february and remained slightly low for the next 2 months.
  - Customer satisfaction was 23% in lower region overall.
  - Georgia was the best performing state (170K) and Tennessee was lowest (108K).
  - Tennessee customer had the highest customer satisfaction rate at 42% in the lower region, followed by Mississippi at 36% in lower region.
  - Alabama saw the highest returns at 20%.
  - Florida had 56% on time deliveries, followed by Alabama at 60%.
  - There was a dip the customers compared the previous two years around 11%.

### Product 2
#### 2017
  - Return rate was high at 11%, On-time deliveries were perfect at 70%.
  - Only customers acquired from ads saw 67% on time delivers whereas Organic and returning customers saw on time deliveries over the target.
  - The first half of the year saw low sales around 35k, rest of the year saw 45K and nearby.
  - Customers Returning (acquisition type) were low (123) which was because of low number in Mississippi, North Carolina, and Tennessee.
  - South Carolina noticed bad customer satisfaction rate at 44%, but had 20% in the good region.
  - Alabama saw only 40% on time deliveries for customers acquired through Ads and had a return rate of 20%.
  - For all customers, Alabama saw 63% on time deliveries and return rate was high at 19%.
  - Flo rida had the most sales at 82K, and Tennessee being the lowest at 47K.
  - Alabama and Georgia both followed South Carolina for bad customer satisfaction rate at 38%

#### 2018
  - High Return rate at 11%, On-time deliveries were 68% (3% below the standard).
  - Mid year saw low sales around 25K-30K, while rest of the year saw around 35K-40K.
  - Customers acquired were nearly the same for all the type. 
  - Comparing to previous year, Customer from Organic type below 23% lower, and from Ads were 15% lower.
  - We had 50 less customer than previous year.
  - Customers from Ads had 14% return rate 6% more than acceptable.
  - South Carolina generated the most sales at 72K followed by Tennessee at 68K, whereasa Mississippi and Alabama had below 50K sales.
  - Georgia saw 15% return rate and Tennessee had 58% on time delivery rate.
  - Customer acquired through Ads had 27% return rate in North Carolina followed by Georgia and Tennessee at 20% each.
  - 50% and 55% of the customers saw on time delivery in Tennessee for Organic and Returning Customers.

#### 2019
  - This year had 11% return date and 70% On-time delivery rate.
  - Throughout the year sales were low as 25K and only 3rd Quarter saw decent sales.
  - Mississippi generated 70K in sales followed by Flo rida at 66K.
  - 10% less customers returned this year.
  - Customers coming from ads type had higher return rate at 13%.
  - Alabama, North Carolina, and South Carolina saw around 35% bad customer satisfaction rate.
  - South Carolina had a high return rate at 20% followed by North Carolina at 16%.
  - Customer from Ads saw only 56% on time delivery in Flo Rida and 28% return rate from South Carolina.
  - Mississippi and North Carolina had 58% on time delivery for customer from Organic reach and North Carolina had 25% return rate for the same type.
  - Georgia saw 53% on time delivery for returning customers and Flo Rida had 21% return rate for the same type/,

### Product 3

### Product 4

### Product 5

## A Visual from the dashboard
![image](https://github.com/HimanshuBaswal/Customer-Success-Dashboard/assets/74957804/16a409cc-4738-4f41-9450-3eea51279671)



