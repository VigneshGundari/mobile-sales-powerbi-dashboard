# 📐 DAX Measures Used

## Total Sales
Total Sales = SUM(Mobile_Sales_Data[Sales])

## Total Quantity
Total Quantity = SUM(Mobile_Sales_Data[Quantity])

## Total Transactions
Total Transactions =
DISTINCTCOUNT(Mobile_Sales_Data[Transaction_ID])

## Average Sales
Average Sales =
DIVIDE([Total Sales], [Total Transactions])