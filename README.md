# Power-BI-AdventureWorksReport

## **Overview of the Adventure Works Bike Shop Power BI Project**

![image alt](https://github.com/nidhigupta3/Power-BI-AdventureWorksReport/blob/293490584cdb85be23a8ae9b0fe2d31d367936d6/Screenshots/AdventureWorks_Logo.png)

This Power BI project is a comprehensive analysis and visualization of Adventure Works, a fictional global manufacturing company producing cycling equipment and accessories.

The **brief** is that the management team needs a way to:<br>
• Track KPIs (sales, revenue, profit, returns)<br>
• Compare regional performance<br>
• Analyze product-level trends, and<br>
• Identify high-value customers<br>

The **dataset** consists of 10 CSV files and was provided with the [Maven Analytics Power BI Desktop course](https://mavenanalytics.io/course/microsoft-power-bi-desktop). 
The customer base is spread across 6 countries on 3 continents: Australia, Canada, France, Germany, the United Kingdom, and the United States. Sales and Return data are available for the period between 01/01/2020 and 06/30/2022. Customer details include Birth Date, Marital Status, Gender, Annual Income, Email ID, Education Level, Number Of Children, Occupation, and Home-owner Status.

The **objective** is to use the Power BI Desktop to:<br>
• Connect and transform the raw data<br>
• Build a relational data model<br>
• Create calculated columns and measures with DAX, and<br>
• Design an interactive dashboard to visualize the data

## **Tools and Technologies**

• Power BI Desktop: For dashboard creation <br>
• Power Query: Data transformation and data cleaning <br>
• DAX (Data Analysis Expressions): Creation of calculated columns and measures <br>
• Excel: Initial data exploration and validation <br>

## **Project Highlights**
The project involved the following steps:

**1. Data Transformation: Cleaned and transformed raw data using Power Query** <br><br>
• The data was provided in CSV files for Customer Details, Product Categories, Product Sub-categories, Territories, Sales, and Returns. <br>
• It was checked and cleaned for duplicates, errors, and transformations were performed to create calculated columns and measures with common functions and formulas. <br>
• It is ensured that all columns have clear titles, appropriate data types, and no missing values. <br>
• This process also involved identifying potential relationships between different data tables. <br>
• A rolling calendar is created using M code in Power Query Editor. <br>

**2. Data Modeling: Created relationships and calculated columns for effective analysis** <br><br>
• Built a relational data model by creating active relations between tables and understanding cardinality and filter flow.<br>
• This involved establishing the 'Sales Data' and 'Returns Data' tables as the foundation. One-to-many connections between tables were used for analysis. <br>

![image alt](https://github.com/nidhigupta3/Power-BI-AdventureWorksReport/blob/293490584cdb85be23a8ae9b0fe2d31d367936d6/Screenshots/Data%20Modeling.png)

**3. Calculated fields with DAX: Created calculated columns and measures using DAX**<br><br> 
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
_(For example, RELATE seamlessly pull data from different tables for a more comprehensive analysis, similar in logic to VLOOKUP)_  <br>
 
**4. Dashboard Development: Built interactive dashboards tailored to stakeholder needs** <br><br>
• Designed an interactive dashboard to visualize data using visuals like KPI cards, Slicers, Tooltips, and a range of visualizations, including bar charts, line graphs, pie charts, and maps, line and clustered column charts, gauge chart, map etc., offering intuitive data interpretations. <br>
• Created bookmarks, drill-through filters, page-level and report-level filters, slicer panel, and custom navigation buttons. <br>

This project serves as a showcase of advanced Power BI techniques and offers a deep dive into the business analytics of a retail bike shop. <br>

## **Data Visualizations for Adventure Works Analysis**

The dashboard has four pages to unlock insights from the data - (1) one for the executive team, (2) one containing the geographical data, (3) one that analyzes the products, and (4) one for the customers' analysis: <br>

**Executive Dashboard:**
<br>
• The Executive Dashboard page provides an overall view of key performance indicators (KPIs) like total revenue, profit, and orders, and top-selling product lists for easy comprehension of overall performance.<br>
• It is equipped with a slicer panel to filter data by year and continent for a more granular view.<br>
<br>
![image alt](https://github.com/nidhigupta3/Power-BI-AdventureWorksReport/blob/293490584cdb85be23a8ae9b0fe2d31d367936d6/Screenshots/Executive%20Dashboard.png)  <br>

**Maps**
<br>
• The Maps page shows a dynamic visualization of Adventure Works’ global order distribution, segmented by continents.<br>
• It highlights dominant regions (e.g., US) and potential new markets (e.g., Asia, Africa, South America).<br>
<br>
![image alt](https://github.com/nidhigupta3/Power-BI-AdventureWorksReport/blob/293490584cdb85be23a8ae9b0fe2d31d367936d6/Screenshots/Map.png)  <br>
<br>
**Product Detail**
<br>
• The Product Detail page enables a granular exploration of individual products.<br>
• It shows details for the Patch Kit/8 Patches currently. For that product, we can see the monthly KPI versus their targets, and that not all KPIs have been fully accomplished against their targets.<br>
• It also shows graphs for the total profit and returns, which automatically adjust with the time-period on the X-axis.<br>
<br>
![image alt](https://github.com/nidhigupta3/Power-BI-AdventureWorksReport/blob/293490584cdb85be23a8ae9b0fe2d31d367936d6/Screenshots/Product%20Details.png)  <br>
<br>
**Customer Detail**
<br>
• The Customer Detail page delves into customer demographics and their impact on business metrics.<br>
• It utilizes doughnut charts to illustrate customer breakdown by occupation and income.<br>
• It shows a surge in total customers during July 2021, aligning with the peak cycling season.<br>
• Employs a “Top 100 Customers” table to reveal customer purchase insights. (For example, revenue generated and orders placed by Mr. Maurice Shan’s versus those of Mrs. Janet Munoz's).<br>
<br>
![image alt](https://github.com/nidhigupta3/Power-BI-AdventureWorksReport/blob/293490584cdb85be23a8ae9b0fe2d31d367936d6/Screenshots/Customer%20Detail.png)  <br>
<br>
Further analysis can be conducted with artificial intelligence visuals like Decomposition Trees and Key Influencers, as seen in the snippets below.<br>
We can see that for the Product Categories 'Bikes', leading by returns rate in the Subcategory are the 'Touring Bikes', with the leading Product being the 'Touring-2000 Blue,46' bike with 8.33% Return Rate.<br>

**Decomposition Tree**
<br>
![image alt](https://github.com/nidhigupta3/Power-BI-AdventureWorksReport/blob/293490584cdb85be23a8ae9b0fe2d31d367936d6/Screenshots/Decomposition%20Tree.png)

<br>
The Key Influencers can be used to further analyze the data. In the instance shown below, one can find out what could lead a customer to be a homeowner, and by how much. For example, a parent is 1.58 times more likely to be a homeowner compared to non-parents, or a person is 1.06 times more likely to be a homeowner if their education level is 'Bachelors' compared to other levels of education in the data.<br><br>

**Key Influencers**
<br>
![image alt](https://github.com/nidhigupta3/Power-BI-AdventureWorksReport/blob/293490584cdb85be23a8ae9b0fe2d31d367936d6/Screenshots/Key%20Influencers.png)


## **Key Learnings & Skills**
• DAX & Data Modeling: DAX language for calculated columns and measures.
• Interactive Visuals: Utilized bookmarks, dynamic titles, and tooltips to enhance user experience.
• KPI Implementation: Applied conditional formatting and KPI indicators for quick insights.
