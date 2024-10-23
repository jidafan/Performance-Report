# Performance Report

- [1. Introduction](#1-introduction)
- [2. PowerBI](#2-powerbi)
  * [2.1 Exploratory Data Analysis](#21-exploratory-data-analysis)
  * [2.2 Data Cleaning](#22-data-cleaning)
  * [2.3 Visualization](#25-visualization)
      + [2.3.1 Measures](#231-measures)
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

In the next step of this project, we begin the visualization of the company data.

#### 2.31 Measures

Before we begin creating charts and graphs. We will create the custom measures and tables will be used in the analysis. To organize the custom measures, I created a measures table to hold them and put an "_" at the front to move it to the top of the tables. The measures they were created were grouped into 4 groups: PYTD, YTD, Switch, and Base Measures.

1. Previous Year To Date (PYTD)

The measures in this category measure the Previous year's Sales, Quantity, and Gross Profit.

2. Year To Date (YTD)

The measures in this category measure the Current year's Sales, Quantity, and Gross Profit.

3. Switch

The measures in this category hold variables for the filter that allows users to parse through the information on the dashboard. It also contains the comparison between YTD and PYTD.

4. Base Measures

The measures in this category hold the basic measures that do not fall under the under category's such as Cost of Goods and Gross Profit%
