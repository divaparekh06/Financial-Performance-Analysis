# 01 — Data Understanding

## 1. First objective

Before building visuals, the dataset was treated as a business table rather than immediately as a Power BI chart source.

The first task was to understand:

- what each column represents
- which columns are numeric
- which columns are categorical
- which columns should be aggregated
- which columns should be averaged
- which columns should be used for grouping/filtering
- which columns represent costs, revenue and discounts

---

## 2. Measure classification

### Additive measures

These can generally be summed across records:

- Sales
- Profit
- Discounts
- Gross Sales
- COGS
- Units Sold

### Descriptive/non-additive fields

These should not normally be summed:

- Country
- Product
- Segment
- Discount Band
- Date
- Month Name
- Year

### Per-unit fields

These represent unit-level values and should generally be averaged when asking for an average price:

- Manufacturing Price
- Sale Price

---

## 3. Why aggregation matters

A major modeling mistake would be to sum a per-unit price and interpret the result as a meaningful average price.

For example:

`SUM(Sale Price)`

does not answer:

> What was the average selling price?

For that question, an average or a properly weighted average is required depending on the business definition.

Similarly, profit margin should not be calculated by simply averaging row-level percentages when a weighted business-level margin is required.

The report therefore uses:

`Total Profit / Total Sales`

for the overall profit margin.

---

## 4. Key business relationships

The following relationships became important later:

**Gross Sales**
→ original sales value before discount

**Discounts**
→ value sacrificed through discounts

**Sales**
→ realized revenue after discounts

**COGS**
→ cost of goods sold

**Profit**
→ financial result

**Profit Margin**
→ profit relative to sales

This gives the core financial chain:

`Gross Sales → Discounts → Sales → Profit → Profit Margin`

---

## 5. Initial analytical questions

Before building the final dashboard, the analysis was framed around:

1. How large are total sales?
2. How large is total profit?
3. What is the overall profit margin?
4. Which countries generate the most sales/profit?
5. Which products perform best?
6. Which segments perform best?
7. Does discount intensity affect profitability?
8. Does high sales necessarily mean high profit?
9. Is poor profitability concentrated in a specific segment?
10. If a segment is weak, is the weakness caused by a country, product or discount pattern?

These questions guided the later visuals.
