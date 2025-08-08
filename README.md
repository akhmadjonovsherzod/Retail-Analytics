# 🛒 Retail Transactions Data Analysis

This project performs an in-depth analysis of retail transaction data using Python and pandas. 
The main focus is to explore customer purchasing behavior, evaluate discount impact, and identify top-performing households and products. 
The insights derived help understand sales dynamics and customer value.

## 📁 Files Used

- `project_transactions.csv` – Contains transactional-level retail data, including sales values, discounts, and product details.
- `product.csv` – Contains product metadata such as manufacturer, department, and description.
- This project is continuously improving, so the new analysis will be added, there will be more data files used...

---

## 🧪 Key Analysis Steps

### 📌 Data Preparation
- Loaded `project_transactions.csv` with optimized data types for memory efficiency.
- Calculated:
  - `total_discount`: Sum of `RETAIL_DISC` and `COUPON_DISC`.
  - `percentage_discount`: Ratio of discount to sales value, capped between 0 and 1.
- Removed unnecessary columns (`RETAIL_DISC`, `COUPON_DISC`, `COUPON_MATCH_DISC`).

---

### 📊 Descriptive Analysis

#### General Stats
- Total **Sales Value**: `$6,666,243.50`
- Total **Discount Given**: `$1,178,658.08`
- **Overall Discount Rate**: `17.7%`
- **Average Percentage Discount per Transaction**: `20.7%`
- **Total Quantity Sold**: `216,713,611 units`
- **Maximum Quantity in Single Transaction**: `89,638 units`

#### Transaction Metrics
- **Avg. Sales Value per Basket**: `$28.62`
- **Avg. Sales Value per Household**: `$3,175.91`

---

## 🏠 Household-Level Insights

- Top 10 households identified by:
  - **Sales Value**
  - **Quantity Purchased**

- Top household by both metrics: **Household Key 1023**
  - Total Value: `$38,319.79`
  - Total Quantity: `4,479,917 units`

- Distribution of household sales value visualized using a histogram.

---

## 🛍️ Product-Level Insights

- Top 10 products based on **Sales Value**:
  - Includes bananas, milk, strawberries, gasoline, paper towels, etc.
- Calculated overall **discount impact** on top products: `~10.3%`

- Bar charts used to visualize top products and household-product intersections.

---

## 🔍 Further Explorations

- Merged product metadata (`product.csv`) with transaction-level data.
- Identified most frequently purchased products by top-value households.
- Investigated specific high-volume product (ID: `6534178`, GASOLINE-REG UNLEADED).

---

## 📌 Tools & Libraries Used

- Python
- pandas
- numpy
- matplotlib (for plotting)

---

## 📈 Next Steps

- Deep dive into time-based patterns (weekly/monthly trends).
- RFM analysis for customer segmentation.
- Basket analysis (market basket, co-purchase behavior).
