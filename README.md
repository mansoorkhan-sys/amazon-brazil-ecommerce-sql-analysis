# amazon-brazil-ecommerce-sql-analysis
End-to-end SQL analysis of Brazilian e-commerce data, exploring revenue trends, customer behavior, seller performance, delivery efficiency, and business insights using MySQL.

Amazon Brazil is scaling rapidly in Latin America's largest e-commerce market. The operations and strategy team needs a clearer picture of how the platform is performing — which customers are driving revenue, which sellers are delivering, which product categories are growing, and where fulfillment is breaking down. 
It contains transactional data across customers, sellers, products, orders, payments, and reviews. MY job was to write SQL queries that turn this raw data into decisions. 

🛠️ Technologies Used
My Sql
GITHUB
WSCUBE -LLM (For Data Set)

Database Structure

TABLE: customers
TABLE: geolocation
TABLE: leads_closed
TABLE: leads_qualified
TABLE: order_items
TABLE: order_payments
TABLE: order_reviews
TABLE: orders
TABLE: product_category_name_translation
TABLE: products
TABLE: sellers

SQL Concepts Covered

CREATE DATABASE
CREATE  TEMPORARY TABLE
PRIMARY KEY
FOREIGN KEY
DATA IMPORT
SELECT
WHERE
ORDER BY
GROUP BY
HAVING
DISTINCT
COUNT()
SUM()
AVG()
RIGHT JOIN
SUBQUERY
JOINS
Aggregate Functions

QUESTIONS & BUSINESS CONTEXT 
Q1. Find the total number of orders fulfilled by each seller state. 

Amazon Brazil's logistics team is planning its next round of regional fulfillment center investments. Before committing budget, they need to know which states are generating the most order volume on the seller side — so infrastructure goes where the actual demand is. 

Q2. For each product category, calculate the cumulative revenue generated as orders come in over time. 

The growth team wants to see how revenue builds up within each category across the order timeline. This running total helps them spot which categories hit their revenue targets early in the month versus which ones pick up only toward the end — useful for planning flash sales and push notifications. 

Q3. Which payment method do customers use the most, and what is the average order value for each payment type? 

The finance and partnerships team is renegotiating contracts with payment providers. Before those talks, they need to know which payment method — credit card, boleto, voucher, or debit card — dominates the platform, and whether high-value orders cluster around a specific payment type. 

Q4. Find the customer who has spent the most money across all their orders. 

The CRM team is launching Amazon Brazil's first premium loyalty tier. The first step is identifying the single highest-spending customer on the platform — both to personally onboard them into the program and to understand what a top-tier customer profile looks like. 

Q5. Find the average review score for each product category. 

The customer experience team tracks satisfaction at the category level. A low average review score in a category often signals a fulfillment issue, a product quality problem, or a mismatch between listing description and actual product. This query helps them prioritize which categories need intervention first. 

Q6. Find the total number of orders placed by each customer, broken down by the state they live in. 

The regional marketing team is planning state-level campaigns in Brazil. They want to know how order frequency varies by customer location — so they can target low-frequency states with acquisition offers and reward high-frequency states with loyalty perks. 

Q7. Identify sellers who registered on the platform but have never fulfilled a single order. 

The seller growth team runs quarterly re-engagement campaigns targeting dormant sellers. To build that list, they need to find every seller account that exists in the system but has zero fulfilled orders — these are the accounts that need a nudge or need to be reviewed for removal. 

Q8. Find the top 5 product categories by total revenue. 

Before every major sales event — Black Friday Brazil, Dia das Mães, Cyber Monday — the merchandising team decides which categories get homepage real estate and promotional budget. Total revenue by category is the primary input for that decision. 

Q9. Find the median delivery time (in days) between order placement and actual delivery. 

The logistics director wants to know the true middle ground of how long customers wait for their orders. The median is preferred over the average here because a handful of extremely delayed orders (due to remote delivery locations in Brazil's interior) would skew the average and make performance look worse than it is for most customers. 

Q10. Find all products that have never been ordered. 

The catalogue operations team does a quarterly clean-up of dead listings. Products that have never received a single order waste search index space, confuse customers, and inflate category browse pages. This query gives them the exact list to review, reprice, or remove. 

Q11. Find sellers who have fulfilled more orders than the average seller on the platform. 

The seller success team is building an invite list for Amazon Brazil's "Top Seller" badge program. Only sellers who perform above the platform average qualify. This query identifies exactly who clears that bar — and gives the team a baseline for what above-average performance actually means numerically. 

Q12. Find which Brazilian states have the highest average customer review score for orders delivered there. 

The last-mile delivery experience varies significantly across Brazil — deliveries to São Paulo and Rio are generally faster and smoother than to states in the North and Northeast. This query helps the CX team correlate delivery destination with satisfaction, so they can push logistics partners to improve in underperforming states. 

Q13. Identify customers who have placed orders but never left a review. 

The post-purchase engagement team wants to grow the volume of reviews on the platform — more reviews mean better product discoverability and buyer trust. The first step is identifying customers who buy regularly but never review, so the team can target them with review reminder emails and in-app nudges. 

Q14. Find the month with the highest number of orders placed across the entire platform. 

The demand forecasting team needs to know Amazon Brazil's peak order month historically. This drives decisions about how much warehouse capacity to reserve, how many temporary delivery staff to hire, and when to start marketing campaigns for the next peak season. 

Learning Outcomes

Through this project, I gained practical experience in:

Designing relational databases
Creating and managing SQL tables
Importing  datasets into PostgreSQL
Writing SQL queries for business analysis
Performing joins across multiple tables
Using aggregate functions for reporting
Extracting insights from structured data


