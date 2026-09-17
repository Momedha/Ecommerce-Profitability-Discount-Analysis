Profit Leakage Analysis — Power BI Dashboard

A single-page Power BI dashboard that uncovers how discount policy silently erodes profit, and simulates the optimal discount cap to fix it.

Business Problem

Retail companies often apply the same discount percentage across all products without measuring its real effect on profit. Sales volume can keep growing while a significant share of orders are actually sold at a loss — and without a dedicated analysis, this stays invisible to management.

This project analyzes ~51,000 orders from a retail dataset to answer three questions:

How much of the business is actually losing money, and why?
Is the problem concentrated in specific product categories, or is it systemic?
What is the ideal maximum discount cap that protects profit without sacrificing sales volume?
Key Findings
Metric	Value
Total Sales	$12.64M
Total Profit	$1.47M
Profit Margin	11.6%
Overall Loss Rate	24.5% of orders are sold at a loss
Break-even point	Loss rate jumps sharply once discount exceeds ~20%
High-discount zone	Orders with discount above 30% have a 92% loss rate
Category-level finding	Only 1 out of 17 sub-categories is loss-making overall (Tables — 29% avg. discount, 57.6% of its orders lose money)
The Solution

Instead of removing discounts (which would also reduce order volume), the dashboard includes an interactive What-If simulation to test different maximum discount caps and their impact on total profit. Capping the discount at ~20-30% is projected to raise total profit from $1.47M to approximately $1.9M, without changing a single product price.

Dashboard Highlights
KPI row: Total Sales, Loss Order Rate, Profit Margin, Total Profit, Top Risk Sub-Category
Total Sales & Profit by Year trend
Discount Range breakdown table (orders, avg profit, loss rate per discount band)
Scatter plot: Avg Discount % vs Profit Ratio by Sub-Category
Interactive discount cap slider with simulated profit outcome
High Discount Loss Rate gauge, isolating the highest-risk order segment
Tools & Techniques
Power BI — data modeling, DAX measures, interactive What-If parameters
DAX — custom measures for Profit Ratio, Loss Rate %, Discount Band segmentation, and dynamic risk detection
Data source: Global Superstore dataset (Orders, Returns, Date dimension tables)
