# E-commerce Analysis 
## About Data 
The dataset used in this project contains records of all transactions made between December 1, 2010 and December 9, 2011 by a UK-based online retail company. The company specializes in selling gift items for various occasions, with a customer base that includes both individual consumers and wholesale distributors. 

You can find the dataset on the UCI Machine Learning Repository: [Link](https://archive.ics.uci.edu/dataset/352/online+retail)

## Data Preprocessing
Conducted simple data cleaning:

- Converted `InvoiceDate` to datetime format and created a new column InvoiceDateOnly containing only the date part.
- Removed missing values in `CustomerID` and `Description`.
- Dropped duplicated rows.
- Removed invalid transactions with `UnitPrice` < 0. Negative `Quantity` values were kept as they represent cancellations or returns (`InvoiceNo` starting with "C").
- Removed abnormal `StockCode` values and irrelevant `Description` entries. Standardize `Description` text to uppercase.
- Added a new column `TotalPrice` calculated as `Quantity` x `UnitPrice`.

## Visualization
