# 10 — Viva / Presentation Notes

## Project in one sentence

> I built an interactive Power BI financial performance dashboard to analyze sales and profitability across products, countries, segments and discount levels, then investigated Enterprise's negative profitability and converted the findings into recommendations.

---

## Why Power BI?

Power BI allows:

- interactive filtering;
- reusable DAX measures;
- dynamic visual updates;
- KPI reporting;
- drill-down analysis;
- conditional formatting;
- dashboard storytelling.

---

## Why use measures?

Measures respond dynamically to filter context.

For example:

`[Total Profit]`

changes automatically when the user selects:

- Enterprise
- a country
- a product
- a discount band

This makes the dashboard interactive rather than static.

---

## Why profit margin?

Profit alone does not show efficiency relative to sales.

Profit margin:

`Profit ÷ Sales`

shows the percentage of sales represented by profit.

---

## Why not simply average profit margins?

A simple average of row-level margins can give every row equal weight.

The report instead uses:

`Total Profit ÷ Total Sales`

which reflects the aggregate financial result of the filtered sales base.

---

## Why investigate Enterprise?

Enterprise was identified as the major negative-profitability segment.

Its overall margin was:

**−3.13%**

This made it the natural focus for diagnostic analysis.

---

## Why investigate countries?

The goal was to determine whether Enterprise's weakness was geographically concentrated.

It was not isolated to one country among the countries analyzed.

---

## Why investigate products?

The goal was to determine whether one product was responsible.

All six Enterprise products were negative, although Carretera was the weakest.

---

## Why investigate discount bands?

Discounting directly affects realized revenue and therefore can affect profitability.

The margin pattern was:

- None: +4.00%
- Low: +1.58%
- Medium: −3.03%
- High: −9.53%

This made discount intensity a strong candidate for further investigation.

---

## Why calculate Discount Rate?

Discount Band is categorical.

Discount Rate quantifies the discount relative to Gross Sales:

`Discounts ÷ Gross Sales`

This provides a measurable interpretation of discount intensity.

---

## Does the analysis prove discounts cause the losses?

No.

The analysis identifies a strong association.

To establish causality, further transaction-level analysis would be needed.

---

## What is the strongest finding?

Enterprise has a broad profitability issue:

- −3.13% overall margin
- all six products negative
- countries analyzed negative
- profitability deteriorates with discount intensity
- High-discount sales are substantial
- Carretera is the weakest product

---

## What would you investigate next?

A deeper analysis could examine:

- transaction-level discount decisions
- customer/order characteristics
- product cost structure
- pricing
- realized selling price
- sales mix
- country-specific economics
- whether high discounts are strategically justified

---

## Why is Montana mentioned?

Montana is the strongest Enterprise product by total profit.

It provides an internal benchmark for asking:

> What is different about the economics of a stronger Enterprise product?

---

## Why is Carretera important?

Carretera is the weakest Enterprise product by total profit, and its largest identified loss occurs at High discount.

It is therefore a priority for deeper investigation.

---

## Presentation storyline

Use this sequence:

1. Introduce the objective.
2. Show Page 1.
3. Explain the overall KPIs.
4. Point out Enterprise's negative margin.
5. Move to Page 2.
6. Select Enterprise.
7. Show all six products are negative.
8. Show countries remain negative.
9. Show margin declines with discount.
10. Show actual profit losses.
11. Show high-discount sales volume.
12. Show Carretera as the weakest product.
13. Move to Page 3.
14. Present recommendations.
15. Explicitly state that association does not prove causation.
