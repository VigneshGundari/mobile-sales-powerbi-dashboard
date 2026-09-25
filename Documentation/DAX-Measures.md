# 📐 DAX Measures Used in the Dashboard

This dashboard uses DAX measures to calculate key business KPIs from the mobile sales dataset.

## 1. Total Transactions

```DAX id="peu8e7"
Total Transaction =
COUNT(Mobile_Sales_Data[Transaction ID])
```

**Purpose:** Counts the total number of transactions recorded in the dataset.

---

## 2. Total Sales

```DAX id="sylp1l"
Total Sales =
SUMX(
    'Mobile_Sales_Data',
    'Mobile_Sales_Data'[Units Sold] *
    'Mobile_Sales_Data'[Price Per Unit]
)
```

**Purpose:** Calculates total revenue by multiplying units sold with price per unit for every transaction and summing the results.

---

## 3. Average Price

```DAX id="ws1wti"
Average =
AVERAGE(Mobile_Sales_Data[Price Per Unit])
```

**Purpose:** Calculates the average selling price of mobile phones across all transactions.