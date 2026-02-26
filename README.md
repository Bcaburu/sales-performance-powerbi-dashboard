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

### Page 1: Executive Overview

![Executive Overview](*place holder do print*)

### Key Insights

- Both **profit and profit margin show a consistent decline over the years**, indicating deterioration in overall business efficiency.
- Accessories and Clothing present the highest margins (37% and 22% respectively), however **Components,despite only an 8% margin, generate nearly five times more total profit than both categories combined**, showing that profitability is strongly driven by volume rather than margin.
- The **Bikes category operates with negative profit and negative margin**, significantly impacting overall company performance.
- The scatterplot segmentation revealed three important product groups:
  - **Growth Opportunity** → low revenue but high margin products that could generate strong returns if sales volume increases.
  - **Underperformers** → negative margin products that should be reworked or potentially discontinued.
  - **High Volume Low Margins** → products with strong sales but low margins, indicating pricing or cost optimization opportunities.
- All **Top 5 best-selling products belong to the Bikes category**, specifically the *Mountain-200* model (different sizes and colors).

### Recommendations

- Increase commercial efforts on high-margin “Growth Opportunity” products.
- Review pricing strategy and production costs for high-volume items to improve margins.
- Perform a deeper product-level analysis within the Bikes category to identify which specific subcategories or models are driving the negative profitability before making strategic decisions.
- Consider discontinuing or restructuring persistent negative-margin products.

### Page 2: Profitability & Product Mix

![Product Profitability](images/product-analysis.png)

### Key Insights

- The **Bikes category represents 89% of total revenue**, yet it operates at an overall negative profit, significantly impacting company performance.
- In 2017, Bikes generated a profit of approximately 19K. However, in 2018 this sharply declined to a loss of 5K.
- The main driver of this decline was **Mountain Bikes**:
  - 2017: 324K revenue with a 6.27% margin.
  - 2018: 503K revenue but margin dropped drastically to 0.3%.
- Although revenue increased substantially in 2018, the severe margin compression led to overall category losses. Margin recovery is observed again in 2019 and 2020.
- Across the full period, **Mountain Bikes are the only subcategory generating positive profit**, while Road Bikes and Touring Bikes consistently generate losses.
- Components generate 555K in revenue, while Clothing (31K) and Accessories (7K) generate significantly less revenue but maintain substantially higher margins.

### Strategic Interpretation

- The company is highly dependent on Bikes for revenue, but this dependency exposes the business to margin volatility.
- The 2018 performance suggests either pricing pressure, cost increases, or aggressive discounting within Mountain Bikes.
- Product mix strongly influences profitability: high-volume categories do not necessarily drive financial sustainability.

### Recommendations

- Conduct a detailed cost and pricing review for Road and Touring Bikes to determine whether restructuring or discontinuation is necessary.
- Stabilize Mountain Bike margins through pricing optimization or cost control initiatives.
- Reduce revenue concentration risk by gradually expanding sales of higher-margin categories.
- Develop cross-selling strategies to increase Clothing and Accessories sales, leveraging their strong margins.
- Consider targeted marketing campaigns and sales training programs to promote higher-margin complementary products during the bike purchase journey.
