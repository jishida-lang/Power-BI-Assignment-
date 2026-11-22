# Power-BI-Assignment-
This is the first Power BI Assignment 1 – Data Transformation &amp; Data Modeling. This assignment will help you explore e-commerce sales data analysis using Power BI.
## Import Data:
1.Get data,Excel workbook,Browse,data select,load.
2.Home, Tranformdata - get Power Query Editor.
## Data Transformation:
1.Keep rows,keep top row,number of row-500 -"List of orders"
2.Order date column select ,datatype-Date-"List of orders",Order date column select ,datatype-  “Amount” and “Target” columns to ‘Fixed Decimal Number’.
3."CustomerName" column Transform,Format,capitalization for each word. 
4.Merge the "State" and "City" columns-Custom column,name-"location",=(city)&","&(State).
5.Custom column,name-"profit Margin",=(Profit)/(Amount)
6.Add conditional column,name-"Profit Status","Profit-is less than-0-loss","Profit-equals-0-Break-Even","Profit-is greater than-0-Profit".
## Merging Data (Joins):
1.Duplicate the "List of Orders" and "Order Details" -Merge Queries,Right table for merge- Order Details,Inner. Named-"Orders Data"
## Handling Missing Data & Duplicate Data: 
1. Identify missing values- Click a column filter arrow to spot "null"- no missing value found.
2. Remove rows,remove duplicates.
## Sorting and Filtering Data:   
1.In Power Query: Click the dropdown next to Order Date in the data preview and select Sort Descending to order rows during data preparation.
2. In Power Query: Click the filter arrow on the State column header, uncheck Select all, check Kerala, and click OK.
## Grouping and Aggregating Data:
1.Duplicate the “Order Details” table ,Group by- Advanced,"Order ID, New column name-count rows"."Category,Average Profit-Average- profit.
2.Duplicate the “Sales Target” table ,Group by-Basic,Month of order date,Total target-Amount-Sum-Target.
## Data Modeling:
1.“List of Orders” and “Order Details” tables based on the ‘Order ID’ -Model view-‘Order ID’- Drag and drop creat new relationship -cardinality-Many to one,Cross filter direction-single.
2.“Order Details” and “Sales Target” tables based on the ‘Category’. Model view 'Category'- Drag and drop creat new relationship -cardinality-Many to many,Cross filter direction-Both.
3.Manage relationship-Active
