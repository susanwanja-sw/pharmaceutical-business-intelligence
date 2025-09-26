# Pharmacy Sales Dashboard (Jan–Aug)  
An interactive Power BI dashboard analyzing pharmacy sales across 5 countries  

## Table of Contents  
1. [Introduction](#introduction)  
2. [Dataset](#dataset)  
3. [Project Objectives](#project-objectives)  
4. [Data Model](#data-model)  
5. [Methodology](#methodology)  
6. [Key Insights & Findings](#key-insights--findings)  
7. [Dashboard Showcase](#dashboard-showcase)  
8. [Tools & Technologies](#tools--technologies)  
9. [How to Explore](#how-to-explore)  
10. [Business Impact & Recommendations](#business-impact--recommendations)  
11. [Future Improvements](#future-improvements)  
12. [Contact](#contact)  

## 1. Introduction  
This project explores pharmacy sales data from January to August across 5 countries using Power BI.  
The dashboard provides insights into:  
- Total revenue and order volume  
- Top-performing products and salespersons  
- Sales trends over time (monthly analysis)  
- Cross-country comparisons  

The goal was to create a data-driven view of sales performance to support better business decisions.  

## 2. Dataset  
- Period Covered: Jan – Aug  
- Size: ~3,488 orders across 5 countries  
- Key Variables:  
  - `Date` → transaction timeline  
  - `Country` → Australia, Canada, India, UK, [other]  
  - `Product` → e.g., Digestive Enzymes, Antiseptic Cream, Cough Syrup  
  - `Sales Person` → responsible staff  
  - `Amount` → sales value ($)  
  - `Boxes Shipped` → order volume  

## 3. Project Objectives  
- Analyze total sales performance across countries and months  
- Identify top and bottom products by sales  
- Highlight top-performing salespersons  
- Visualize trends in total sales to uncover seasonality  
- Build an interactive dashboard for decision-makers  

## 4. Data Model  
The model follows a Star Schema:  

- Fact Table: Sales Data (`Amount`, `Boxes Shipped`, `Product`, `Sales Person`, `Country`, `Date`)  
- Dimension Table: Date table (`Day`, `Month`, `WeekNo`, `Year`)  

Data Model Screenshot:  
<img width="824" height="442" alt="image" src="https://github.com/user-attachments/assets/65cc5dde-e715-4ec4-bb04-5e000b43a858" />

## 5. Methodology  
1. Data Preparation  
   - Cleaned dataset (removed duplicates, standardized formats)  
   - Created a proper Date Dimension for time intelligence  

2. Data Modeling  
   - Established 1-to-many relationship between Date and Sales data  
   - Defined calculated columns and measures (DAX)  

3. DAX Measures  
   - Total Amount  
   - Total Orders  
   - Top/Bottom N Products  
   - Top/Bottom N Salespersons  
   - Monthly/Year-to-Date Sales  

4. Visualization  
   ### 1. **Overall Business Performance**
   <img width="614" height="97" alt="image" src="https://github.com/user-attachments/assets/dc84f44b-ef93-4673-8997-5e4c3e60d8e3" />

- Total Amount: $58.93K
This represents total revenue generated across all markets during the 8-month period. It's the primary financial health indicator, showing whether the business meets revenue targets and profitability goals. This metric drives investment decisions, budget allocation, and strategic planning for pharmaceutical operations.
- Total Orders: 3,488
Total transaction volume indicates market demand and operational capacity. Combined with revenue, it reveals an average order value of $16.90, suggesting premium pharmaceutical products or bulk transactions. This metric helps determine staffing needs, inventory planning, and customer engagement effectiveness across all markets.
- Total Countries: 5
Geographic diversification reduces market risk and demonstrates international operational capability. Multi-country presence is crucial for pharmaceutical companies, indicating regulatory compliance expertise, supply chain sophistication, and growth potential. This diversification provides revenue stability and competitive advantage in the global healthcare market.
- Sales Person: 7
Sales team size directly impacts revenue generation and operational efficiency. With $8.42K revenue per salesperson, this metric evaluates individual productivity and team optimization. It determines hiring needs, territory coverage effectiveness, and compensation structures while indicating the company's ability to scale operations internationally. 

### 2. **Sales Trend Over Time**
<img width="850" height="473" alt="image" src="https://github.com/user-attachments/assets/16d5f138-611f-4d7b-a3f7-72d53a3028e0" />

1. Chart Overview
The line chart displays monthly sales performance from January to August, showing clear seasonal patterns with steady growth from January's low (5.5K) to May's peak (8.9K), followed by fluctuations through summer months ending at 6.9K in August.

2. Key Patterns Identified
Sales demonstrate strong seasonality with 62% growth from January to May peak. June shows significant dip to 7.0K before recovering to second-highest performance in July (8.8K). August stabilizes at 6.9K, indicating consistent operational performance despite seasonal variations.

3. Business Implications
The pattern reveals predictable seasonal trends crucial for inventory planning and resource allocation. January and June dips present improvement opportunities, while May and July peaks provide templates for successful strategies. Understanding these cycles enables better forecasting and operational planning. 

### 3. **Product & Sales Performance**
<img width="839" height="489" alt="image" src="https://github.com/user-attachments/assets/d409dd4a-6930-477b-93bc-13a2bc105812" />

- Total Amount By Product
The product performance chart reveals Digestive Enzymes as the clear market leader at 11.1K, followed by Antiseptic Cream (9.7K) and Nasal Spray (8.8K). The bottom performers include Allergy Pills (7.8K) and Cough Syrup (7.9K), indicating product portfolio optimization opportunities.

- Amount by Sales Person
<img width="764" height="492" alt="image" src="https://github.com/user-attachments/assets/aa8653e7-7164-4a17-8817-9c688f3690cd" />

Sales performance shows Rajesh Patel leading at 11.0K, closely followed by Nikhil Batra (10.4K) and Priya Singh (9.1K). The consistent performance across top performers suggests effective sales processes, while lower performers like Divya Mehra (6.9K) indicate coaching and development opportunities.
Strategic Insights
Both charts demonstrate concentrated performance with top performers significantly outpacing others. Product concentration in Digestive Enzymes and sales concentration in top three representatives suggest successful strategies that can be replicated. The performance gaps indicate clear opportunities for portfolio optimization and team development.
  

## 6. Key Insights & Findings  
- Revenue: $58.93K generated from 3,488 orders  
- Geographic Reach: Sales across 5 countries  
- Sales Team: 7 active salespersons  
- Top Product: Digestive Enzymes ($11.1K)  
- Top Salesperson: Rajesh Patel ($11.0K)  
- Sales Trend:  
  - Sales peaked in May (8.9K) and July (8.8K)  
  - Lowest sales in January (5.5K)  

## 7. Dashboard Showcase  
Dashboard Screenshot:  

<img width="635" height="507" alt="image" src="https://github.com/user-attachments/assets/1b10ccd5-de40-4b2f-9d80-53d62468bfd3" />


https://github.com/user-attachments/assets/04de5d09-6bae-4adb-b7df-2482e26b2895


## 8. Tools & Technologies  
- Power BI – modeling, DAX measures, interactive dashboards  
- Power Query – data cleaning and transformation  
- Excel – preliminary dataset review  
- DAX – advanced calculations (YTD, Top/Bottom N, KPIs)  

## 9. Business Impact & Recommendations  
### Strategic Recommendations

**Product Strategy**
- **Scale Success:** Increase inventory and marketing focus on **Digestive Enzymes** (top performer).  
- **Opportunity Products:** Develop growth strategies for **Allergy Pills** and **Cough Syrup** (untapped potential).  
- **Portfolio Balance:** Analyze bottom performers for possible **discontinuation or repositioning**.  

**Sales Team Development**
- **Best Practice Sharing:** Leverage **Rajesh Patel** and **Nikhil Batra's** techniques for team training.  
- **Performance Coaching:** Implement **mentorship programs** to develop team members.  
- **Territory Optimization:** Redistribute high-performing sales reps across **key markets**.  

**Market Expansion**
- **Seasonal Planning:** Prepare for **January dips** and capitalize on **May peak patterns**.  
- **Geographic Focus:** Analyze **country-specific preferences** for targeted marketing campaigns.  
- **Inventory Management:** Align **stock levels** with identified seasonal and product trends.  

### Immediate Action Items
- Investigate factors behind **January and June sales declines**.  
- Conduct **win-loss analysis** with top-performing sales representatives.  
- Develop **product bundling strategies** featuring high-performing items.  
- Implement **monthly performance review cycles** based on dashboard insights.  

## 10. Future Improvements

### Phase 1 Enhancements (Next 3 months)
- **Predictive Analytics:** Implement forecasting models using Power BI AI features.  
- **Customer Segmentation:** Add customer demographic data for deeper market insights.  
- **Profitability Analysis:** Include cost data for margin analysis and ROI calculations.  

### Phase 2 Advanced Features (6-12 months)
- **Real-Time Dashboards:** Set up automated data refresh via Power BI Service.  
- **Mobile Optimization:** Design responsive layouts for mobile and tablet access.  
- **Advanced Analytics:** Implement statistical analysis and correlation studies.  
- **Alert System:** Configure automated notifications for performance thresholds.  

### Phase 3 Enterprise Integration (12+ months)
- **API Connectivity:** Direct integration with CRM and ERP systems.  
- **Advanced AI:** Machine learning models for demand forecasting.  
- **Multi-Currency Support:** Enable global expansion with currency conversion.  
- **Compliance Reporting:** Build regulatory reporting capabilities for the pharmaceutical industry.  

### Technical Roadmap
- **Migration to Power BI Premium** for advanced features.  
- **Integration with Azure Data Factory** for ETL automation.  
- **Implementation of row-level security** for data governance.  
- **Development of embedded analytics** for external stakeholders. 
  
[susanwanja347@gmail.com]

[https://www.linkedin.com/in/susan-wanja-1b63a6234/]

© All rights reserved, Susan Wanja portfolio 2025
