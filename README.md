# Performance Report

- [1. Introduction](#1-introduction)
- [2. PowerBI](#2-powerbi)
  * [2.1 Exploratory Data Analysis](#21-exploratory-data-analysis)
  * [2.2 Data Cleaning](#22-data-cleaning)
  * [2.3 Visualization](#23-visualization)
      + [2.3.1 Measures](#231-measures)
      + [2.3.2 Cards](#232-cards)
      + [2.3.3 Tree Maps](#233-tree-maps)
      + [2.3.4 Waterfall Chart](#234-waterfall-chart)
      + [2.3.5 Line and Bar Chart](#235-line-and-bar-chart)
      + [2.3.6 Scatter Chart](#236-scatter-chart)
- [3. Conclusion](#3-conclusion)


### 1. Introduction

The project shown is a PowerBI report of a fictional company named Plant Co. The report uses various charts and graphs to visualize the company's performance during the YTD and PYTD. The report dives into the sales, gross profit and quantity of products sold. The data can be accessed [here](https://github.com/jidafan/Performance-Report/blob/main/Plant_DTS.xls).

### 2. PowerBI

The report for the project can be viewed [here](https://github.com/jidafan/Performance-Report/blob/main/Performance%20Report.pbix)

#### 2.1 Exploratory Data Analysis

Before we begin working on the dataset, we must understand the data. In this step of the code, we look through each table and each column within to understand the data and see the changes that need to be made.

#### 2.2 Data Cleaning

In this step, we clean the data in the Excel sheet using the PowerQuery editor in PowerBI. To clean the data, we changed the datatypes of some columns to align with what they needed to be. The date column in the file was listed as a text column in PowerBI, so we needed to make changes to change it to a date-type column. In the product ID column, we removed duplicated and blank values as well.

#### 2.3 Visualization

In the next step of this project, we begin the visualization of the company data in PowerBI

#### 2.3.1 Measures

Before we begin creating charts and graphs, we will create the custom measures and tables that will be used in the analysis. To organize the custom measures, I created a measures table to hold them and put an "_" at the front to move it to the top of the tables. The measures they were created were grouped into 4 groups: PYTD, YTD, Switch, and Base Measures.

1. Previous Year To Date (PYTD)

The measures in this category measure the Previous year's Sales, Quantity, and Gross Profit.

2. Year To Date (YTD)

The measures in this category measure the Current year's Sales, Quantity, and Gross Profit.

3. Switch

The measures in this category hold variables for the filter that allows users to parse through the information on the dashboard. It also contains the comparison between YTD and PYTD which is marked as YTD vs PYTD.

4. Base Measures

The measures in this category hold the basic measures that do not fall under the previous categories such as Cost of Goods and Gross Profit%

#### 2.3.2 Cards

The first visualizations that I created were cards that show the YTD, YTD vs PYTD, PYTD and GP%. These cards changed based on what was selected in the filters. There is a filter for years, and a filter for Gross Profit, Quantity or Sales. 

#### 2.3.3 Tree Map

The first chart that was created was a tree map, the tree map was selected so that the performance of the company in various countries could easily be seen. The map shows the name of the country and the YTD vs PYTD.

#### 2.3.4 Waterfall Chart

This chart provides an in-depth view of the data, providing an opportunity to drill down. This chart follows the same pattern of changing based on the selection of the filter. At the top level, it shows the performance over a year. upon clicking on the graph a user can drill down and see country-specific information and then even go a step further and see the performance of each product.

#### 2.3.5 Line and Bar Chart

This chart provides a view of the YTD and PYTD of products over a year's time. The graph features the ability to drill down and show information about each quarter.

#### 2.3.6 Scatter Chart

The last chart featured in this report is a scatterplot that plots the profitability of each customer account, there are bars on the sides of the chart that allow users to filter the data to certain percentages. It features red lines to mark the averages of GP% and YTD, and it is dynamic and changes based on the filter.

