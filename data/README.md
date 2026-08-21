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

### Revenue

Money a business earns from selling its goods or services before subtracting operating expenses and other costs. (Price x Quantity)

### Units Sold

Volume Metrics, number of units sold in the record.

### Manufacturing Price

Manufacturing cost per unit.

### Sale Price

Selling price per unit.

**Important:** Sale Price is not calculated as `Units Sold × Manufacturing Price`.

Conceptually, sales revenue is related to units sold and selling price, while manufacturing price represents a cost-side measure.

### Gross Sales

It represents sales before deductions such as discounts, returns and allowances.

### Discounts

Can be promotional, volume trade, seasonal or customer-specific discount.

### Sales

Gross Sales - Deductions/Discounts

### COGS

Cost of goods sold.
They are the direct costs associated with producing or acquiring the goods. (Eg: Raw materials, direct labor, manufacturing cost)
It doesn't include maketting, office rent, salaries etc.

### Gross Profit

Net sales- COGS. It tells us how much money remains after covering COGS.

### Gross Profit Margin

(Gross Profit/Revenue) x 100

### Profit Margin

(Profit/Revenue) x 100

### Manufacturing Cost

Cost associated with producing a product

### Discount Band

Categorical classification of discount intensity:

- None
- Low
- Medium
- High

### Segment

A segment groups customers based on some meaningful characteristics. Eg: Government, consumers, enterprise etc.

### Country

Geographic market.

### Data Grain

Grain means what does one record/row represents. Eg: one row: one order

### Cost Vs. Expense

Cost is the money spent to produce something.
Expense is the cost that is recognized as an expense in the accounting period.

---

## Data handling principle

The dataset was intentionally kept simple.

No unnecessary data-cleaning transformation was introduced merely for the sake of transformation. The supplied worksheet was considered sufficiently clean for the intended analysis, after validation of fields, types and core calculations.

---


