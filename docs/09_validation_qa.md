# 09 - Final Validation and QA

## 1. Overall KPI validation

With all slicers cleared:

- Total Sales ≈ 118.73M
- Total Profit ≈ 16.89M
- Profit Margin ≈ 14.23%
- Total Discounts ≈ 9.21M
- Units Sold ≈ 1.13M

---

## 2. Enterprise validation

With Segment = Enterprise:

- Total Sales ≈ 19.61M
- Total Profit ≈ −614.55K
- Profit Margin ≈ −3.13%

---

## 3. Slicer validation

Each slicer was tested:

- Country
- Segment
- Product
- Discount Band

Combined filtering was also tested.

Example:

`Country = France`

+

`Segment = Enterprise`

should filter the page to that exact analytical context.

---

## 4. Cross-page consistency

Page 1 and Page 2 use the same underlying model.

Therefore, when the same filter context is applied, shared KPIs should agree.

This was used as a practical model-validation test.

---

## 5. Visual validation

Check that:

- Sales visuals use Sales.
- Profit visuals use Total Profit.
- Margin visuals use Profit Margin %.
- Profit-by-discount uses Total Profit rather than Profit Margin %.
- Sales-by-discount uses Total Sales.
- Product × Discount uses Total Profit.
- Discount Rate uses Discounts ÷ Gross Sales.

---

## 6. Formatting validation

Recommended:

- Profit Margin → percentage
- Discount Rate → percentage
- Sales → M/K
- Profit → M/K
- Discounts → M/K
- Units → M/K

Avoid displaying unnecessarily long decimal values.

---

## 7. Analytical wording validation

Do not state:

> Discounts caused Enterprise losses.

Preferred:

> Higher discount intensity is strongly associated with lower Enterprise profitability.

Reason:

Correlation/association does not by itself establish causality.

---

## 8. Final user experience test

The report should open with all slicers cleared.

A viewer should be able to:

1. understand overall performance;
2. notice Enterprise as an anomaly;
3. navigate to the profitability page;
4. select Enterprise;
5. reproduce the discount-profitability investigation;
6. read the recommendations.

---

## 9. Final completion criteria

The project is considered complete when:

- calculations are validated;
- slicers work;
- visuals update correctly;
- all three pages are aligned;
- numbers are appropriately formatted;
- recommendations match the evidence;
- the `.pbix` is saved and backed up;
- documentation is committed to GitHub.
