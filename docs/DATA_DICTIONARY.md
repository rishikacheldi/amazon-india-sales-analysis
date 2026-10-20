# Data Dictionary — Amazon India Sales Analysis

## 1. Overview

This document describes the fields in the Amazon India Sales dataset used for the Power BI dashboard.

- **Dataset size:** 10,000 rows and 13 columns
- **Reporting period:** January 1, 2024 – August 30, 2026
- **Unique orders:** 10,000
- **Missing values:** None detected in the supplied dataset
- **Duplicate rows:** None detected in the supplied dataset

## 2. Column Definitions

| Column | Data Type | Description |
|---|---|---|
| `Order_ID` | Text | Unique identifier assigned to an order. |
| `Order_Date` | Date | Date associated with the order. |
| `Category` | Text | Product category to which the item belongs. |
| `Product` | Text | Name of the product purchased. |
| `Quantity` | Integer | Number of units recorded for the order. |
| `Unit_Price_INR` | Decimal | Unit price in Indian rupees. |
| `Discount_Pct` | Decimal | Discount rate represented as a fraction; for example, 0.25 means 25%. |
| `Total_Sales_INR` | Decimal | Recorded sales amount in Indian rupees. |
| `Profit_INR` | Decimal | Recorded profit amount in Indian rupees. |
| `Payment_Method` | Text | Payment method used for the order. |
| `Fulfillment` | Text | Fulfillment method associated with the order. |
| `Order_Status` | Text | Recorded status of the order. |
| `Ship_State` | Text | Indian state associated with the shipment. |

## 3. Business Dimensions

### Product dimensions
- Category
- Product

### Transaction dimensions
- Order ID
- Order Date
- Order Status

### Operational dimensions
- Payment Method
- Fulfillment
- Ship State

### Numerical measures
- Quantity
- Unit Price
- Discount Percentage
- Total Sales
- Profit

## 4. Data Quality Checks

The supplied Excel dataset was checked for:

- Missing values across all 13 columns.
- Exact duplicate rows.
- Duplicate order identifiers.
- Valid date conversion and reporting-period boundaries.

Results:
- Missing values: 0
- Exact duplicate rows: 0
- Duplicate order IDs: 0
- Unique order IDs: 10,000

## 5. Interpretation Notes

- Monetary values are denominated in INR.
- Discount percentages are stored as decimal fractions.
- Each row has a unique Order ID in the supplied dataset.
- Order status should be considered when interpreting sales, profit, returns, and cancellations.
- The meaning of recorded sales and profit for cancelled or returned orders should be verified before calculating realized revenue or net profit.

