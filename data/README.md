# Data

## Source worksheet

The Power BI model uses the **Financial Data** worksheet.

The later Excel worksheets created during analysis were validation/working sheets and were not required as Power BI source tables.

---

## Source fields

The financial dataset contains the following important fields used during analysis:

- Segment
- Country
- Product
- Discount Band
- Units Sold
- Manufacturing Price
- Sale Price
- Gross Sales
- Discounts
- Sales
- COGS
- Profit
- Date
- Month Number
- Month Name
- Year

---

## Important field meanings

### Units Sold

Number of units sold in the record.

### Manufacturing Price

Manufacturing cost per unit.

### Sale Price

Selling price per unit.

**Important:** Sale Price is not calculated as `Units Sold × Manufacturing Price`.

Conceptually, sales revenue is related to units sold and selling price, while manufacturing price represents a cost-side measure.

### Gross Sales

Sales value before the recorded discount.

### Discounts

Discount amount applied to the gross sales value.

### Sales

Realized sales/revenue after discounts in the supplied financial dataset.

### COGS

Cost of goods sold.

### Profit

Profit value provided by the dataset.

### Discount Band

Categorical classification of discount intensity:

- None
- Low
- Medium
- High

### Segment

Business/customer segment.

### Country

Geographic market.

### Product

Product identifier/name.

---

## Data handling principle

The dataset was intentionally kept simple.

No unnecessary data-cleaning transformation was introduced merely for the sake of transformation. The supplied worksheet was considered sufficiently clean for the intended analysis, after validation of fields, types and core calculations.

---

## Recommended repository handling

If the dataset is permitted to be shared publicly, place the original workbook/CSV in this directory.

If it is not permitted to be shared, **do not commit the dataset**. Keep only this documentation file and explain that the source data is course/institution-provided.

The `.pbix` report may also be subject to course/institution sharing restrictions.
