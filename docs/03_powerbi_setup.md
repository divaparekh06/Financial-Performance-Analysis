# 03 — Power BI Setup

## 1. Source loading

Only the **Financial Data** worksheet was loaded into the Power BI model.

The additional Excel worksheets created during the exploratory/validation process were not required as source tables.

This kept the Power BI model simple and avoided unnecessary duplicate tables.

---

## 2. Model objective

The project did not require a complex multi-table star schema because the supplied dataset was already organized as a single analytical financial table for this assignment.

The primary model therefore consists of the Financial Data table and measures built over it.

---

## 3. Measures

The report uses measures rather than hard-coded visual calculations wherever a reusable business metric is required.

Key measures include:

- Total Sales
- Total Profit
- Total Discounts
- Total Units Sold
- Profit Margin %
- Average Sale Price
- Discount Rate %

The exact DAX is documented in:

`powerbi/DAX_MEASURES.md`

---

## 4. Slicers

The dashboard uses four main slicers:

- Country
- Segment
- Product
- Discount Band

These were deliberately chosen because they allow a user to move from broad overview to targeted investigation.

Example:

`Segment = Enterprise`

turns the dashboard into an Enterprise-focused analysis.

---

## 5. Theme

A consistent Power BI theme was applied.

The semantic visual language is:

- Blue → Sales
- Dark blue → Profit
- Green → positive profitability
- Orange → discount-related emphasis
- Red → negative profitability

The global theme was used for consistency, while special profitability visuals received targeted formatting where necessary.

---

## 6. Conditional formatting

Conditional formatting was used particularly for:

- Profit Margin matrices
- Product × Discount Profit matrices

The purpose is analytical, not decorative:

- negative values become visually obvious
- stronger positive values become visually obvious
- the user can detect patterns without reading every number
