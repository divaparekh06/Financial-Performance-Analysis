# DAX Measures

> Replace the table name only if your Power BI model uses a different name. The project uses `Financial Data`.

## Total Sales

```DAX
Total Sales =
SUM('Financial Data'[Sales])
```

## Total Profit

```DAX
Total Profit =
SUM('Financial Data'[Profit])
```

## Total Discounts

```DAX
Total Discounts =
SUM('Financial Data'[Discounts])
```

## Total Units Sold

```DAX
Total Units Sold =
SUM('Financial Data'[Units Sold])
```

## Profit Margin %

```DAX
Profit Margin % =
DIVIDE(
    [Total Profit],
    [Total Sales]
)
```

## Average Sale Price

```DAX
Average Sale Price =
AVERAGE('Financial Data'[Sale Price])
```

## Discount Rate %

```DAX
Discount Rate % =
DIVIDE(
    [Total Discounts],
    SUM('Financial Data'[Gross Sales])
)
```

---

# Why DIVIDE is used

`DIVIDE()` is preferable to direct division for a reusable Power BI measure because it handles a zero denominator safely.

For example:

```DAX
DIVIDE([Total Profit], [Total Sales])
```

is safer than:

```DAX
[Total Profit] / [Total Sales]
```

---

# Formatting

Recommended formats:

| Measure | Format |
|---|---|
| Total Sales | Currency/financial units, display in M/K |
| Total Profit | Currency/financial units, display in M/K |
| Total Discounts | Currency/financial units, display in M/K |
| Total Units Sold | Number, display in M/K |
| Profit Margin % | Percentage, 1–2 decimals |
| Average Sale Price | Currency/number, 1–2 decimals |
| Discount Rate % | Percentage, 1–2 decimals |
