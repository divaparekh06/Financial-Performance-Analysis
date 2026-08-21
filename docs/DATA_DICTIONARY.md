# Data Dictionary

| Field | Type | Business meaning | Typical use |
|---|---|---|---|
| Segment | Categorical | Business/customer segment | Filter/group |
| Country | Categorical | Geographic market | Filter/group |
| Product | Categorical | Product | Filter/group |
| Discount Band | Categorical | Discount intensity category | Filter/group |
| Units Sold | Numeric | Quantity sold | Sum |
| Manufacturing Price | Numeric | Manufacturing cost per unit | Average/context |
| Sale Price | Numeric | Selling price per unit | Average/context |
| Gross Sales | Numeric | Sales before discount | Sum |
| Discounts | Numeric | Discount amount | Sum |
| Sales | Numeric | Realized sales/revenue | Sum |
| COGS | Numeric | Cost of goods sold | Sum |
| Profit | Numeric | Profit | Sum |
| Date | Date | Transaction/reporting date | Trend |
| Month Number | Numeric | Month index | Sorting/time |
| Month Name | Categorical | Month label | Trend |
| Year | Numeric | Year | Trend/filter |

---

# Important aggregation rules

### SUM

Appropriate for:

- Sales
- Profit
- Discounts
- Gross Sales
- COGS
- Units Sold

### AVERAGE

Potentially appropriate for:

- Sale Price
- Manufacturing Price

depending on the business question.

### Ratio

Profit Margin:

`Total Profit / Total Sales`

Discount Rate:

`Total Discounts / Total Gross Sales`

---

# Important warning

Do not interpret:

`SUM(Sale Price)`

as an average price.

Do not define Sale Price as:

`Units Sold × Manufacturing Price`

Sale Price is the per-unit selling-price field in the dataset.
