MADHAV E-COMMERCE SALES DASHBOARD – Power BI

Table of Contents

Introduction

Objective

Skills & Tools

Dataset Overview

Key Insights

Dashboard Highlights

Recommendations

Project Structure

What I Learned

⭐ Final Note

Introduction

This project converts raw e-commerce order data into a clean, interactive Power BI dashboard. It reveals what drives revenue and profit, who your most valuable customers are, which product segments win, and how payment preferences shape fulfillment and cash flow.

Objective

Track core KPIs: Total Sales (Amount), Profit, Quantity, and Average Order Value.

Understand monthly profit seasonality and detect loss-making months.

Compare state-wise performance to focus regional strategy.

Analyze category mix and payment-mode behavior.

Identify top customers and top/low-performing sub-categories for action.

Skills & Tools
Skill	Tools Used
Data Visualization	Power BI (cards, column & bar charts, donut charts, slicers, tooltips)
Data Transformation	Power Query (cleaning, typing, shaping)
Data Modeling	Star schema, Order ↔ Details (1:*), Date table, relationships
DAX & Analysis	KPI measures, AOV, time intelligence (MTD/YTD), ranking, conditional formatting
Dataset Overview

Files

Orders.csv – Order ID, Order Date (DD-MM-YYYY), CustomerName, State, City

Details.csv – Order ID, Category, Sub-Category, Quantity, Amount, Profit, PaymentMode

Relationship
Orders[Order ID] (1) → Details[Order ID] (*)

Key Insights
🧺 Revenue & Category Mix

Total Sales (Amount): 437,771

Total Profit: 36,963

Total Quantity: 5,615

Average Order Value (AOV): ≈ 875.54

Quantity share by Category: Clothing 62.62%, Electronics 20.55%, Furniture 16.83%.

🗺️ Geographic Performance

Top states by sales:

Maharashtra — 102,498

Madhya Pradesh — 87,463

Uttar Pradesh — 38,362
Followed by Delhi and Rajasthan.

⏳ Time Trends

Best months (Profit): Nov 2018, Jan 2018, Feb 2018.

Loss-making months: May 2018, Jul 2018, Dec 2018 (negative profit).

💳 Payment Behavior

Share of Quantity by Payment Mode: COD 43.74%, UPI 20.61%, Debit Card 13.20%, Credit Card 11.97%, EMI 10.49%.

High COD reliance suggests opportunities to nudge digital payments.

🧱 Sub-Category Profitability

Top profitable sub-categories: Printers, Bookcases, Saree, Accessories, Tables.

Under-performers (negative profit): Furnishings, Electronic Games, Kurti, Skirt, Leggings.

👤 Top Customers (by Sales)

Harivansh, Madhav, Madan Mohan, Shiva, Vishakha lead overall spend.

Dashboard Highlights

Features

KPI cards for fast executive read.

Month-wise profit columns with conditional formatting.

State-wise sales bars for regional comparison.

Donuts for Category and Payment Mode mix.

Top Customers and Sub-Category Profit bars.

Interactive slicers (Quarter, State) for drill-downs.

Recommendations

Region focus: Double down on Maharashtra and Madhya Pradesh; investigate drivers in Uttar Pradesh to scale.

Payment optimization: With COD at 43.74%, incentivize UPI/Cards (discounts, cashbacks) to reduce returns and handling cost.

Assortment strategy: Clothing leads volume (62.62%). Keep depth here; grow profitable electronics/furniture with bundles.

Seasonality play: Push campaigns in November; proactively manage pricing and promotions in May/July/December where profit dips.

Merchandising: Scale Printers/Bookcases/Saree; review pricing or sourcing for Furnishings/Electronic Games/Kurti/Skirt/Leggings.

Project Structure
├── MADHAV E-COMMERCE SALES DASHBOARD.pbix   # Power BI report
├── Orders.csv                               # Orders (Order, Date, Customer, State, City)
├── Details.csv                              # Line items (Category, Sub-Category, Qty, Amount, Profit, PaymentMode)
├── assets/
│   └── madhav_dashboard.png                 # Dashboard screenshot (used above)
└── README.md

🔎 What I Learned

Clear storytelling (KPI → trend → mix → deep dive) elevates decision-making.

Payment mode mix materially impacts operations and profitability.

Simple state/city roll-ups surface immediate regional opportunities.

Negative months deserve root-cause: discounting, returns, seasonality, or supply issues.

Clean modeling (Date table + relationships) keeps DAX simple and visuals fast.

⭐ Final Note

If this analysis helped or inspired you, star the repo and share your thoughts. Your feedback makes the next iteration even better!
