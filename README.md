# Power-BI-AdventureWorksReport

## **Overview of the Adventure Works Bike Shop Power BI Project**

![image alt](https://github.com/nidhigupta3/Power-BI-AdventureWorksReport/blob/293490584cdb85be23a8ae9b0fe2d31d367936d6/Screenshots/AdventureWorks_Logo.png)

This Power BI project is a comprehensive analysis and visualization of Adventure Works, a fictional global manufacturing company producing cycling equipment and accessories.

The **brief** is that the management team needs a way to:
1. Track KPIs (sales, revenue, profit, returns)
2. Compare regional performance
3. Analyze product-level trends, and
4. Identify high-value customers

The **dataset** consists of 10 CSV files and was provided with the [Maven Analytics Power BI Desktop course](https://mavenanalytics.io/course/microsoft-power-bi-desktop). 
The customer base is spread across 6 countries on 3 continents: Australia, Canada, France, Germany, the United Kingdom, and the United States. Sales and Return data are available for the period between 01/01/2020 and 06/30/2022. Customer details include Birth Date, Marital Status, Gender, Annual Income, Email ID, Education Level, Number Of Children, Occupation, and Home-owner Status.

The **objective** is to use the Power BI Desktop to:
1. Connect and transform the raw data
2. Build a relational data model
3. Create calculated columns and measures with DAX, and
4. Design an interactive dashboard to visualize the data

## **Tools and Technologies**
 
1. Power BI Desktop: For dashboard creation
2. Power Query: Data transformation and data cleaning
3. DAX (Data Analysis Expressions): Creation of calculated columns and measures
4. Excel: Initial data exploration and validation

## **Project Highlights**
The project involved the following steps:

**1. Data Transformation: Cleaned and transformed raw data using Power Query**
1. The data was provided in CSV files for Customer Details, Product Categories, Product Sub-categories, Territories, Sales, and Returns.
2. It was checked and cleaned for duplicates, errors, and transformations were performed to create calculated columns and measures with common functions and formulas.
3. It is ensured that all columns have clear titles, appropriate data types, and no missing values.
4. This process also involved identifying potential relationships between different data tables.
5. A rolling calendar is created using M code in Power Query Editor.

**2. Data Modeling: Created relationships and calculated columns for effective analysis**
1. Built a relational data model by creating active relations between tables and understanding cardinality and filter flow.
2. This involved establishing the 'Sales Data' and 'Returns Data' tables as the foundation. One-to-many connections between tables were used for analysis.

![image alt](https://github.com/nidhigupta3/Power-BI-AdventureWorksReport/blob/293490584cdb85be23a8ae9b0fe2d31d367936d6/Screenshots/Data%20Modeling.png)

**3. Calculated fields with DAX: Created calculated columns and measures using DAX**
Leveraged DAX functions to unlock deeper insights from the Adventure Works dataset. Here are some key functions used:

1. Math Functions: For example, SUM, AVERAGE, MAX/MIN, COUNT, DISTINCTCOUNT
   
2. Logical Functions: For example, IF, AND, OR, NOT
 
3. Text Functions: For example, CONCATENATE, REPLACE, UPPER/LOWER
 
4. Filter Functions: For example, CALCULATE, FILTER, ALL
_(For example, CALCULATE helped as a filter override, enabling me to create new filter contexts. It proved invaluable for analyzing trends over time, such as previous month’s orders, revenue, profit, returns, and overall average price)_

5. Date, Time, Time Intelligence: For example, DATE, YEAR/MONTH, DATEDIFF, DATESYTD
_(For example, DATESINPERIOD and DATESYTD helped in calculating metrics like 90-day rolling profit, along with comparing current data points to previous months in terms of orders, profit, revenue, and returns)_

6. Iterator Functions: For example, SUMX, AVERAGEX
_(For example, SUMX helped in calculating metrics like revenue, profit, and total orders for each data point, which then became the building blocks for further analysis)_

7. Relationship Functions: For example, RELATED
_(For example, RELATE seamlessly pull data from different tables for a more comprehensive analysis, similar in logic to VLOOKUP)_
 
**4. Dashboard Development: Built interactive dashboards tailored to stakeholder needs**
Visualizing data with reports
 • Building an interactive dashboard: Customized dashboards providing insightful metrics and KPIs relevant to the bike shop's operations.
 • Visualizations: A range of visualizations, including bar charts, line graphs, pie charts, and maps, offering intuitive data interpretations.
 Designed an interactive dashboard to visualize data using charts and visuals: KPI cards, Matrix, Slicers, Bar chart, Line and clustered column chart, Gauge, Map etc.
Created Bookmarks, drill-through filters and page level, report level filters.

This project serves as a showcase of advanced Power BI techniques and offers a deep dive into the business analytics of a retail bike shop.

## **Data Visualizations for Adventure Works Analysis**

My Power BI report utilized four key dashboards to unlock insights from the data:
The dashboard had four pages, one for the executive team, one that had the geographical data, one that analyzed the products and finally a page for the customers.

**Executive Dashboard:**

![image alt](https://github.com/nidhigupta3/Power-BI-AdventureWorksReport/blob/293490584cdb85be23a8ae9b0fe2d31d367936d6/Screenshots/Executive%20Dashboard.png)

**Maps**
The Maps page shows the geographical distribution of the company’s orders.

![image alt](https://github.com/nidhigupta3/Power-BI-AdventureWorksReport/blob/293490584cdb85be23a8ae9b0fe2d31d367936d6/Screenshots/Map.png)

**Product Detail**
The products page shows details for the All-Purpose bike stand. For that product, we can see the monthly KPI vs their targets, and that all KPIs had not been fully accomplished against their targets. We can also see graphs for the total profit and returns, which automatically adjust with the time-period on the x-axis.

![image alt](https://github.com/nidhigupta3/Power-BI-AdventureWorksReport/blob/293490584cdb85be23a8ae9b0fe2d31d367936d6/Screenshots/Product%20Details.png)

**Customer Detail**

![image alt](https://github.com/nidhigupta3/Power-BI-AdventureWorksReport/blob/293490584cdb85be23a8ae9b0fe2d31d367936d6/Screenshots/Customer%20Detail.png)

**Decomposition Tree**

![image alt](https://github.com/nidhigupta3/Power-BI-AdventureWorksReport/blob/293490584cdb85be23a8ae9b0fe2d31d367936d6/Screenshots/Decomposition%20Tree.png)

**Key Influencers and Top Segments**

![image alt](https://github.com/nidhigupta3/Power-BI-AdventureWorksReport/blob/293490584cdb85be23a8ae9b0fe2d31d367936d6/Screenshots/Key%20Influencers.png)
![image alt](https://github.com/nidhigupta3/Power-BI-AdventureWorksReport/blob/293490584cdb85be23a8ae9b0fe2d31d367936d6/Screenshots/Top%20Segments.png)

## **Key Learnings & Skills**
• DAX & Data Modeling: DAX language for calculated columns and measures.
• Interactive Visuals: Utilized bookmarks, dynamic titles, and tooltips to enhance user experience.
• KPI Implementation: Applied conditional formatting and KPI indicators for quick insights.
