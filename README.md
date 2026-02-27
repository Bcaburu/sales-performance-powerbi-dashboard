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
# 🧮 DAX Calculations

DAX measures were created to evaluate performance, growth, and efficiency across multiple business dimensions.  
The calculations focused on profitability analysis, year-over-year comparison, performance ranking, and product segmentation.

**Profitability Metrics**

- Profit  
- Profit Margin  
- Total Cost  

Core financial measures were created to evaluate business health beyond revenue, focusing on margin sustainability and operational efficiency.  
These metrics helped identify loss-making products, inefficient markets, and declining profitability trends.

**Time Intelligence**

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

![Executive Overview](https://github.com/Bcaburu/sales-performance-powerbi-dashboard/blob/main/images/ExecutiveOverview.JPG?raw=true)

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

## Page 3: Trend & Growth Analysis

![Trend & Growth](images/trend.png)

### Key Insights

- Every month of 2020 shows higher **revenue** than the same month in 2019, indicating strong sales growth.
- However, the opposite occurs with **profit**. Monthly profit decreased significantly year-over-year, ranging from a 77% decline to a 170% decline.
- January and May recorded operating losses, with May reaching approximately **–4.4K profit**.
- Year-to-date results (January–May) reinforce the same pattern:
  - **Revenue increased by +43.96%**
  - **Profit decreased by –117.15%**
- The company is selling more products but earning less money from those sales, indicating severe margin compression.

### Interpretation

- Business growth is currently volume-driven rather than efficiency-driven.
- The increasing gap between revenue and profit suggests rising costs, heavier discounting, or a shift toward lower-margin products.
- Without intervention, continued growth may worsen financial performance instead of improving it.

### Recommendations

- Investigate cost structure changes, especially within high-volume product categories.
- Review pricing and discount strategies to prevent margin erosion.
- Monitor profit margin as a primary performance KPI rather than relying solely on revenue growth.
- Prioritize sustainable growth by balancing sales expansion with profitability control.

## Page 4: Geographic Performance

![Geographic Performance](images/geographic.png)

### Key Insights

- The **United States is the dominant market**, generating more than double the revenue and profit of the second largest country (Canada).
- **France shows the highest efficiency**, presenting the best profit margin at approximately 2.59%.
- **Australia and Germany operate with negative margins**, contributing to overall profitability deterioration.
- Category analysis reveals that **Bikes are the primary driver of losses in both Australia and Germany**.

### Interpretation

- Market size does not necessarily correlate with operational efficiency.
- The business relies heavily on the U.S. market for profitability, creating geographic concentration risk.
- Poor performance in specific countries appears to be product-driven rather than demand-driven.

### Recommendations

- Reevaluate product strategy in Australia and Germany, particularly within the Bikes category.
- Align product offerings with regional profitability performance instead of applying a uniform global strategy.
- Expand focus on high-margin products in efficient markets such as France.
- Reduce dependence on a single market by improving profitability in secondary regions.

## Page 5: Sales Performance Analysis

![Sales Performance](images/sales-performance.png)

### Key Insights

- Sales performance varies significantly across representatives, showing large differences in profitability contribution.
- Some representatives generate high revenue but comparatively low profit, indicating heavy discounting or inefficient product mix.
- Other representatives achieve strong profit margins despite lower sales volume, demonstrating higher sales efficiency.
- Performance differences are not fully explained by territory size alone, suggesting that individual selling strategies influence results.

### Interpretation

- Revenue alone is not an accurate measure of sales success.
- Some sales representatives are volume-oriented while others are margin-oriented.
- Incentive structures based purely on sales volume may unintentionally encourage low-margin transactions.

### Recommendations

- Introduce performance evaluation metrics based on **profitability in addition to revenue**.
- Provide targeted training focused on selling higher-margin products and improving negotiation practices.
- Adjust compensation or bonus structures to reward profitable sales instead of only sales volume.
- Share best practices from high-efficiency representatives across the sales team.
# 📈 Final Conclusion

The company is experiencing **revenue growth but declining profitability**.  
Although sales volume continues to expand, **margin compression indicates that operational efficiency is deteriorating over time**.

The analysis shows that the core problem is not demand, but **business structure**. The company is **highly dependent on the Bikes category**, which concentrates most revenue while generating weak or negative profitability. In particular, **Road and Touring Bikes consistently operate at a loss**, while **Mountain Bikes show volatile margins** that strongly affect overall financial results.

At the same time, **higher-margin categories such as Clothing and Accessories represent a small share of total revenue**, limiting their positive impact on company performance. Geographic analysis also reveals that losses are amplified in specific markets where low-margin products dominate sales.

To achieve **sustainable growth**, the company should shift focus from **volume to profitability**. Strategic actions should include reviewing pricing and cost structure within the Bikes category, reducing exposure to persistently unprofitable subcategories, and increasing sales of high-margin complementary products such as Clothing and Accessories through cross-selling and targeted commercial strategies.

By **optimizing product mix, improving margin management, and aligning regional strategy with profitability performance**, the business can convert revenue growth into long-term financial sustainability.
