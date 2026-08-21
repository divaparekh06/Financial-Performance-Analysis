# 04 - Measures and Calculations

## 1. Total Sales

### Definition

Sum of the Sales field.

### Business meaning

Total realized sales/revenue represented by the filtered dataset.

---

## 2. Total Profit

### Definition

Sum of the Profit field.

### Business meaning

Total profit represented by the filtered dataset.

---

## 3. Total Discounts

### Definition

Sum of Discounts.

### Business meaning

Total discount value given across the filtered dataset.

---

## 4. Total Units Sold

### Definition

Sum of Units Sold.

### Business meaning

Total quantity sold.

---

## 5. Profit Margin %

### Definition

`Total Profit ÷ Total Sales`

### Why this definition is used

It produces a business-level weighted margin.

It is preferable to simply averaging row-level profit percentages when the objective is to measure the profitability of the entire filtered sales base.

---

## 6. Average Sale Price

### Definition

Average of the Sale Price field.

### Business meaning

Average listed/selling price per unit represented by the rows in the filtered dataset.

### Important distinction

Sale Price is a per-unit selling-price field.

It should not be confused with:

`Units Sold × Manufacturing Price`

That multiplication describes a cost-side relationship and does not define Sale Price.

---

## 7. Discount Rate %

### Definition

`Total Discounts ÷ Total Gross Sales`

### Business meaning

The proportion of gross sales represented by discounts.

Example:

If Gross Sales = 1,000,000 and Discounts = 100,000:

`100,000 ÷ 1,000,000 = 10%`

So 10% of gross sales value was given away through discounts.

---

## 8. Why Discount Band and Discount Rate are different

### Discount Band

A categorical label:

- None
- Low
- Medium
- High

### Discount Rate

A calculated quantitative ratio:

`Discounts ÷ Gross Sales`

The band tells us the category.

The rate tells us the effective magnitude of discounting in the filtered data.

---

## 9. Enterprise discount-rate observations

Approximate effective rates observed:

| Band | Effective Discount Rate |
|---|---:|
| None | ~0% |
| Low | ~2.4% |
| Medium | ~6.8% |
| High | ~12.5% |

The increasing rates provide quantitative context for the categorical discount bands.
