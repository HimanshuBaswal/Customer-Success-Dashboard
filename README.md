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
- **Technique:** Pivot Chart with Years and Date as Rows & Revenue for Values
- **Data:** Revenue over the Years (Months)
- **Chart:** Line Chart

### Visual 2: Sales Map
- **Technique:** Pivot Chart with State as Columns & Revenue for Values
- **Data:** Revenue by each State
- **Chart:** Map Chart

### Visual 3: Delivery Performance Doughnut
- **Technique:** Pivot Chart with Delivery Performance as Rows & Revenue (Count) for Values & Percentage of delayed orders
- **Data:** Delivery Performance Ratio (on-time and delayed)
- **Chart:** Doughnut Chart & Percent of on-time delivered orders 

### Visual 4: Return Rate Doughnut
- **Technique:** Pivot Chart with Return as Rows & Revenue (Count) for Values & Percentage of returned orders
- **Data:** Return Rate (no and yes)
- **Chart:** Doughnut Chart & Percent of returned (yes) orders 

### Visual 5: Customer Acquisition Waterfall
- **Technique:** Pivot Chart with Customer Acquisition Type as Columns & Revenue (Count) for Values
- **Data:** Customer Acquisition Type by Count
- **Chart:** Waterfall Chart (Total is gray)

### Visual 6: Customer Satisfaction Bar
- **Technique:** Pivot Chart with Customer Satisfaction as Columns, Product as Rows & Revenue (Count) for Values
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
  - Return rate was ideal at 8%, with on-time deliveries at 64% (9% below the standard).
  - On-time delivery was lowest at 60% for customers acquired from Ads.
  - Sales dipped in February and March, fluctuating between 80k-125k throughout the year.
  - All customer acquisition types had nearly the same count.
  - Customer satisfaction was 28% in the low and very low categories.
  - North Carolina was the best performing state (178K) and Mississippi was the lowest (142K).
  - For orders from customers acquired by "Ads", Alabama generated the most sales (92K), with a customer satisfaction rate of 36% in the lower region.
  - Florida had a 38% lower customer satisfaction rate, followed by Mississippi at 36%.

#### 2018
  - High return rate at 11%, with on-time deliveries at 68% (3% below the standard).
  - High return rate for customers from ads at 13%.
  - June and September saw the lowest sales around 66K.
  - Customer satisfaction was 23% in the lower region overall.
  - Alabama was the best performing state (170K) and Georgia was the lowest (147K).
  - For orders from customers acquired by "Ads", Mississippi generated the most sales (60K), with a customer satisfaction rate of 15% in the lower region.
  - For the same acquisition type, Florida had the highest satisfaction rate at 38% in the lower region.
  - The State of Tennessee saw 16% returns while South Carolina saw 2% returns.

#### 2019
  - Highest return rate at 13%, with on-time deliveries falling to 65%.
  - Customers from ads and returning ones had high product return rates around 14%.
  - Sales fell to a low range during February and remained slightly low for the next two months.
  - Customer satisfaction was 23% in the lower region overall.
  - Georgia was the best performing state (170K) and Tennessee was the lowest (108K).
  - Tennessee customers had the highest customer satisfaction rate at 42% in the lower region, followed by Mississippi at 36% in the lower region.
  - Alabama saw the highest returns at 20%.
  - Florida had 56% on-time deliveries, followed by Alabama at 60%.
  - There was a dip in customers compared to the previous two years, around 11%.

### Product 2
#### 2017
  - Return rate was high at 11%, with on-time deliveries at 70%.
  - Only customers acquired from ads saw 67% on-time deliveries, whereas Organic and Returning customers saw on-time deliveries above the target.
  - The first half of the year saw low sales around 35K, while the rest of the year saw around 45K.
  - Returning customers were low (123) due to low numbers in Mississippi, North Carolina, and Tennessee.
  - South Carolina had a bad customer satisfaction rate at 44%, but 20% in the good region.
  - Alabama saw only 40% on-time deliveries for customers acquired through Ads and had a return rate of 20%.
  - For all customers, Alabama saw 63% on-time deliveries and a return rate of 19%.
  - Florida had the most sales at 82K, and Tennessee was the lowest at 47K.
  - Alabama and Georgia both followed South Carolina with a bad customer satisfaction rate at 38%.

#### 2018
  - High return rate at 11%, with on-time deliveries at 68% (3% below the standard).
  - Mid-year saw low sales around 25K-30K, while the rest of the year saw around 35K-40K.
  - Customers acquired were nearly the same for all types.
  - Compared to the previous year, Organic customer acquisition was 23% lower, and Ads were 15% lower.
  - There were 50 fewer customers than the previous year.
  - Customers from Ads had a 14% return rate, 6% more than acceptable.
  - South Carolina generated the most sales at 72K, followed by Tennessee at 68K, whereas Mississippi and Alabama had below 50K sales.
  - Georgia saw a 15% return rate and Tennessee had a 58% on-time delivery rate.
  - Customers acquired through Ads had a 27% return rate in North Carolina, followed by Georgia and Tennessee at 20% each.
  - Only 50% and 55% of the customers in Tennessee saw on-time delivery for Organic and Returning Customers.

#### 2019
  - This year had an 11% return rate and 70% on-time delivery rate.
  - Throughout the year, sales were as low as 25K, and only the third quarter saw decent sales.
  - Mississippi generated 70K in sales, followed by Florida at 66K.
  - There were 10% fewer customers this year.
  - Customers from Ads had a higher return rate at 13%.
  - Alabama, North Carolina, and South Carolina saw around 35% bad customer satisfaction rates.
  - South Carolina had a high return rate at 20%, followed by North Carolina at 16%.
  - Customers from Ads saw only 56% on-time delivery in Florida and a 28% return rate from South Carolina.
  - Mississippi and North Carolina had 58% on-time delivery for Organic customers, and North Carolina had a 25% return rate for the same type.
  - Georgia saw 53% on-time delivery for Returning customers, and Florida had a 21% return rate for the same type.

### Product 3
#### 2017
  - On-time Delivery Rate: 67%
  - Return Rate: 11%
  - Sales Performance: Sales remained low around 45K in the first four months of the year, returned to normal levels in the following months, but saw a dip in September.
  - Top Performing States:
    - South Carolina: 112K
    - Florida: 105K
  - Customer Dissatisfaction Rate: 37%
  - Customer Acquisition Breakdown:
    - Returning Customers: 28%
    - Ads Customers: 33%
    - Organic Customers: 39%
  - Customer Satisfaction (by Acquisition Type):
    - Ads Customers: 45% had a lower satisfaction rate compared to Organic and Returning customers.
  - Return Rates:
    - Tennessee: 19%
    - Florida: 15%
  - On-time Delivery Rates (by Acquisition Type):
    - Ads Customers:
    - North Carolina: 53%
    - South Carolina: 58%
    - Tennessee: 60%
  - Overall Customer Satisfaction:
    - Tennessee: 70% dissatisfaction rate.
    
#### 2018
  - On-time Delivery Rate: 69%
  - Return Rate: 12%
  - Top Performing States:
    - Alabama: 129K
    - Georgia: 124K
  - Return Rates:
    - Tennessee: 18%
    - Georgia: 16%
  - On-time Delivery Rates (by Acquisition Type):
    - Organic Customers: South Carolina had 50% on-time delivery.
    - Ads Customers: North Carolina had a 29% return rate.
  - Overall Customer Satisfaction (by Acquisition Type):
    - Ads Customers: 16% return rate, 60% on-time delivery.
  - State-wise Performance:
    - Georgia: Worst customer satisfaction rate at 25%, 30% return rate.
    - Florida: Least sales, 50% of sales were generated in the first five months.
    
#### 2019
  - On-time Delivery Rate: 72%
  - Return Rate: 10%
  - Sales Performance: Sales were steady throughout the year.
  - Top Performing States:
    - Mississippi: 125K
    - Florida: 65K (least sales)
  - Customer Satisfaction Rate: 28%
  - Sales Change: 10% decrease compared to last year.
  - On-time Delivery Rates:
    - Florida: 57%
    - North Carolina: 58%
  - State-wise Customer Satisfaction:
    - South Carolina: Highest satisfaction rate at 35%.
  - Customer Acquisition Breakdown:
    - Ads Customers: 67%
    - Organic Customers: 25%
    - Returning Customers: 8%
  - Return Rates:
    - Ads Customers: Tennessee 20%, North Carolina 18%.
  - Overall Satisfaction (by Acquisition Type):
    - Florida: 45% bad satisfaction rate.
    - North Carolina: 35% bad satisfaction rate.

## Summary:

### Sales Performance

#### Overall Trends
  - Revenue Growth: Sales showed fluctuations across the years, with notable dips in mid-2017 and mid-2018, while 2019 saw more stable but lower overall sales.
  - Seasonal Trends: Sales were typically lower in the first quarter and peaked towards the year-end.
  - Top Performing States:
    - South Carolina: Consistently high sales across all years.
    - Florida: Steady performance with high sales in 2017 and 2018.
    - Alabama and Georgia: Significant contributors, especially in 2018.

#### Customer Acquisition Channels
  - Returning Customers: Steady but lower in number compared to new acquisitions.
  - Ads Customers: High acquisition rate but often accompanied by higher return rates.
  - Organic Customers: Showed better satisfaction and retention but lower sales volume compared to Ads Customers.

### Delivery Performance
#### On-time Delivery Rates
  - 2017: 67% overall, with the highest rates in South Carolina and Alabama.
  - 2018: Slight improvement to 69%, but significant variances between states.
  - 2019: Achieved a higher rate of 72%, showing consistent improvement.

#### Delays and Challenges
  - Common Issues: High variability in delivery performance across states, with North Carolina and Florida often underperforming.
  - Top Performers: Mississippi and South Carolina consistently had better on-time delivery rates.

### Return Rates
#### Overall Trends
  - 2017: Return rates were around 11% across all products.
  - 2018: Slight increase to 12%, with notable spikes in Tennessee and Georgia.
  - 2019: Return rates stabilized at 10%, with improvements seen in Mississippi and South Carolina.
#### By Customer Acquisition
  - Ads Customers: Higher return rates across all years, indicating potential issues with product fit or expectations.
  - Organic and Returning Customers: Lower return rates, suggesting better alignment with customer needs.

### Customer Satisfaction
#### Satisfaction Levels
  - 2017: Overall dissatisfaction rate was 37%, with Tennessee having the highest dissatisfaction.
  - 2018: Improved to 27%, with notable reductions in dissatisfaction in Georgia and North Carolina.
  - 2019: Further improvement to 23%, with South Carolina showing the highest satisfaction rates.
#### Key Insights
  - Product Fit: Ads Customers had higher dissatisfaction and return rates, indicating a need for better-targeted marketing and product information.
  - State Performance: States like South Carolina and Alabama consistently performed better in terms of customer satisfaction, while North Carolina and Tennessee often lagged.

### Strategic Insights and Recommendations
   - Focus on High-Performing States: Leverage the success in South Carolina and Alabama to implement best practices across other states.
   - Improve Ads Customer Experience: Address the higher return and dissatisfaction rates among Ads Customers by refining marketing strategies and setting clearer expectations.
   - Enhance Delivery Efficiency: Continue improving on-time delivery rates, particularly in underperforming states like North Carolina and Florida.
   - Boost Organic Acquisition: Invest in organic growth strategies to increase the proportion of satisfied and loyal customers.
   - Monitor Seasonal Trends: Prepare for seasonal dips in sales by implementing targeted promotions and inventory management strategies during low-sales periods.

## A Visual from the dashboard
![image](https://github.com/HimanshuBaswal/Customer-Success-Dashboard/assets/74957804/17944d6d-4c4d-4f64-b8bf-310de7368978)



