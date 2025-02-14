# Blinkit Grocery Store Data Analysis

This project involves analyzing grocery sales data from Blinkit, a leading quick-commerce platform. The goal is to uncover insights into customer purchasing behavior, product performance, sales trends, and operational efficiency using Python and data analysis techniques.



## Problem Statement

 The goal is to uncover insights into customer purchasing behavior, product performance, sales trends, and operational efficiency using Python and data analysis techniques.

Key Objectives:
1. Perform data cleaning and preprocessing on raw sales data.
2. Conduct Exploratory Data Analysis (EDA) to identify trends, patterns, and outliers.
3. Create a dashboard which analyze sales performance by Itemwise, outlet,Fat content and outlet size.



### Steps followed 

- Step 1 : Get data set from https://www.kaggle.com/datasets/arunkumaroraon/blinkit-grocery-dataset.
- Step 2 : Load data into Power BI Desktop, dataset is a excel file.
- Step 3 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 4 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 5 : It was observed that in none of the columns errors & empty values.
- Step6 : In ItemFat Content column there is 'reg' for regular aprt from 'Regular'. So replace the 'reg' with 'Regular.
- Step7 : In ItemFat Content column there is 'low fat' for regular aprt from 'Low Fat'. So  applied "Capitalize Each Word" option.
- Step7 : Close and apply.
- Step 8 : In report view, created 3 measures, "Average Sales","Average Rating" ,"No.of Items".
- Step 9 :Created a frame and in that add textboxes for heading, and subheading.
- Step 10 : Added a card view and add "Total sales, Average sales,Average Ratings,No.of items. 
- Step 11 : Created a metrics which contain above parameters.
- Step 12 : Added Donut chart for "Total Sales by Fat content".
- Step 13 : Added bar chart for "Total Sales by Outlet Type".
- Step 14 : Added Stalked bar chart for "No.of Items by item type". 
- Step 15 : Added Line chart for "Total sales by Outlet Establishment". 
 - Step 16 : Added donut chart for "Sales by Outlet size". 
 - Step 17 : Added Funnel chart for "Sales by Outlet LOcation". 
 - Step 18 : Added Metrics table for Outlet summary". 
 Following DAX expression was written to find total distance,
 
         Avg Rating = AVERAGE('BlinkIT Grocery Data'[Rating])
         Avg Sales = AVERAGE('BlinkIT Grocery Data'[Sales])
         No.of items = COUNTROWS('BlinkIT Grocery Data')

         Parameter = {
    ("Sales", NAMEOF('BlinkIT Grocery Data'[Sales]), 0),
    ("Avg Sales", NAMEOF('BlinkIT Grocery Data'[Avg Sales]), 1),
    ("Avg Rating", NAMEOF('BlinkIT Grocery Data'[Avg Rating]), 2),
    ("No.of Items", NAMEOF('BlinkIT Grocery Data'[No.of items]), 3)
}
    
 
 # Report Snapshot (Power BI DESKTOP)

 
 ![Image](https://github.com/user-attachments/assets/55f5119c-a3d2-4f24-a793-897d1f112cef)
 
 
