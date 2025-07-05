# Amazon Product Review Analysis

## Project Objective

Amazon product review helps identify the factors that influence purchasing decisions, provides strategies to boost sales, and offers valuable insights into customer perceptions of the products.

## Dataset Used
' <a href="https://github.com/Marryah007/Amazon_Data_Analysis_Dashboard/blob/main/Amazon%20Product%20Review.xlsx">Dataset</a>

## Questions (KPIs)

•	What is the average discount percentage by product category?

•	How many products are listed under each category?

•	What is the total number of reviews per category? 

•	Which products have the highest average ratings?

•	What is the average actual price vs the discounted price by category? 

•	Which products have the highest number of reviews? 

•	How many products have a discount of 50% or more?

•	What is the distribution of product ratings (e.g., how many products are rated 3.0, 4.0, etc.)? 

•	What is the total potential revenue (actual price × rating count) by category? 

•	What is the number of unique products per price range bucket (e.g., <₹200, ₹200–₹500, >₹500)?

•	How does the rating relate to the level of discount?

•	How many products have fewer than 1,000 reviews?

•	Which categories have products with the highest discounts?

•	Identify the top 5 products in terms of rating and number of reviews combined.

' <a href="https://github.com/Marryah007/Amazon_Data_Analysis_Dashboard/blob/main/Screenshot%202025-07-04%20010641.png">'Dashboard <a/>

## Methodology

This encompasses the systematic approach or techniques used to manage, analyze, and visualize data using Excel

Here's a more detailed breakdown:

Calculations & Formulas

•	1.Potential Revenue:
=IF(AND(ISNUMBER(E2),ISNUMBER(H2)),E2*H2,0)

•	2.Review Count
=LEN(I2)-LEN(SUBSTITUTE(I2,",",""))+1

•	3.Price Range Bucket
=IF(E2<20000," <£20000 ",IF(E2<=39999," £20000-£39999 ",IF(E2<=59999, " £40000-£59999 ", IF(E2<=79999, "£ 60000-£79999 ", ">£80000 "))))



4.High Discount
=IF(F2>=50%, " Yes ", " No ")

5. Combined Score
=SUM(G2,L2)

Data Organization & Manipulation:

1.Pivot Tables:
Summarize and analyze datasets by creating interactive tables that can be easily rearranged and filtered. 

2. Sorting and Filtering:
Organize data in ascending or descending order based on specific criteria and filter data to display only relevant information. 

3. Conditional Formatting:
Apply formatting (e.g., color, icons) to cells based on specific conditions, making it easier to identify trends and outliers. 

4. Data Validation:
Restrict the type of data that can be entered into a cell, ensuring data accuracy. 

5.Named Ranges:
Assign meaningful names to cells or ranges of cells, making formulas easier to read and understand (e.g., naming cell K1 as "Potential Revenue").


## Process

•	Verify data for any missing values and anomalies, and sort out the same.

•	Made sure data is consistent and clean with respect to data type, data format and values used.

•	Created pivot tables according to the questions asked.

•	Merge all pivot tables into one dashboard and apply slicers to make dynamic interactive filters for reports, allowing users to easily filter data and explore different views of the information.

## Dashboard
![Screenshot 2025-07-04 010641](https://github.com/user-attachments/assets/91377832-5cfb-4103-9a7a-bf6e2f4477ac)


## Project Insight

•	Products with 50% or more discount influences Customers’ decisions.

•	A good review with a positive rating help others to make informed decisions.

•	The maximum number of products customer orders from Amazon.

## Conclusion

To effectively guide product improvement, marketing strategy, and customer engagement, focus on understanding the customers deeply, personalizing interactions, leveraging data and feedback, and providing a seamless omnichannel experience. Continuously iterate based on customer feedback and adapt approach to stay ahead of evolving needs and preferences. 
