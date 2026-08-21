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
