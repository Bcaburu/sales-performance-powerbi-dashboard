# Sales Performance Analysis: Power BI Project
This project analyzes company sales performance across products, markets, and sales representatives using Power BI.
The goal was to identify profitability drivers, underperforming areas, and growth opportunities.
The analysis focuses not only on revenue generation but also on operational efficiency and margin sustainability.
# 🛠️ Tools & Technologies
- Power BI
- DAX
- Power Query
- Data Modeling (Star Schema)
- Data Visualization
# 🧱 Data Model
A star schema model was implemented to improve performance, simplify filtering behavior, and support scalable analysis.
The Sales table acts as the central fact table, connected to dimension tables such as Products, Region, and Salesperson.
This structure allows consistent aggregations across different business perspectives including product, geography, and sales performance.

*place holder do print*
## 🧮 DAX Calculations

DAX measures were created to evaluate performance, growth, and efficiency across multiple business dimensions.  
The calculations focused on profitability analysis, year-over-year comparison, performance ranking, and product segmentation.

**Profitability Metrics**

- Profit  
- Profit Margin  
- Total Cost  

Core financial measures were created to evaluate business health beyond revenue, focusing on margin sustainability and operational efficiency.  
These metrics helped identify loss-making products, inefficient markets, and declining profitability trends.

**⏳ Time Intelligence**

- Revenue PY  
- Revenue YoY %  
- Profit PY  
- Profit YoY %  

Time intelligence calculations were implemented to compare year-over-year performance and detect growth patterns.  
This analysis revealed that revenue growth does not necessarily translate into profit growth, highlighting margin compression over time.

**Performance Analysis**

- Avg Profit per Rep  
- Top Performer Profit  
- Lowest Performer Profit  
- Top Performer Name  

Ranking and aggregation logic were used to evaluate individual sales representative performance.  
These measures helped identify top contributors, underperforming representatives, and variations in sales efficiency

**Product Segmentation**

- Product Segment  

Products were dynamically classified into performance segments based on profitability and revenue contribution.  
This segmentation enabled strategic portfolio analysis and supported decision-making regarding product optimization and discontinuation.


# 🔎 Analysis & Insights
