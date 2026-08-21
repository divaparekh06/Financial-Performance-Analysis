# Power BI Report Build Guide

## Page 1 — Executive Overview

### Header

Title:

**Financial Performance Overview**

Subtitle:

**Sales, profitability, product, segment and regional performance analysis**

### Slicers

- Country
- Segment
- Product
- Discount Band

### KPI cards

- Total Sales
- Total Profit
- Profit Margin %
- Total Discount
- Total Units Sold

### Visuals

1. Sales & Profit Trend
2. Sales & Profit by Country
3. Profit Margin by Segment
4. Sales & Profit by Product
5. Profit Margin by Discount Band

---

# Page 2 — Profitability Deep Dive

### Header

**Profitability Deep Dive**

Subtitle:

**Investigating margin drivers, discount impact, product performance and segment profitability**

### Slicers

- Segment
- Country
- Product
- Discount Band

### KPI cards

- Total Sales
- Total Profit
- Profit Margin %
- Total Discount

### Visuals

1. Segment × Discount Band → Profit Margin %
2. Profit Margin by Product
3. Profit Margin by Country
4. Enterprise Profit by Discount Band
5. Enterprise Sales by Discount Band
6. Discount Rate by Discount Band
7. Product × Discount Band → Total Profit

### Conditional formatting

Use:

- red for negative
- neutral/intermediate around zero
- green for positive

---

# Page 3 — Key Insights & Recommendations

### Header

**Key Insights & Recommendations**

### Four sections

1. Executive Finding
2. Key Findings
3. Recommendations
4. Analytical Conclusion

Keep text concise and visual.

Do not place the full detailed methodology on the dashboard page.

The detailed reasoning belongs in the repository documentation.

---

# Theme

Semantic palette:

| Role | Hex |
|---|---|
| Sales | `#2F80ED` |
| Profit | `#173F8A` |
| Positive profitability | `#27AE60` |
| Discount emphasis | `#F2994A` |
| Negative profitability | `#D64545` |

---

# Interaction philosophy

The slicers are not decorative.

They should allow users to move from:

**Overall business**

to:

**specific segment**

to:

**specific country/product/discount context**

without rebuilding calculations.

---

# Design principle

Do not add visuals merely because space is available.

Every visual should answer a business question.
