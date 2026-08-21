# 02 — Data Validation

## Purpose

Before trusting Power BI calculations, the results were cross-checked using Excel.

This was important because a visually correct dashboard can still contain incorrect measures.

---

## 1. Validation philosophy

The validation workflow was:

**Excel calculation → Power BI measure → compare results**

The goal was to verify:

- totals
- aggregations
- ratios
- filter behavior
- derived metrics

---

## 2. COUNT vs COUNTA

A distinction was explicitly considered between `COUNT()` and `COUNTA()`.

### COUNT()

Counts numeric cells.

### COUNTA()

Counts non-empty cells regardless of whether the value is numeric, text or another supported non-empty type.

Therefore, the correct function depends on what is being counted.

If the task is:

> Count numeric transaction values

`COUNT()` may be appropriate.

If the task is:

> Count non-empty records/cells in a column that may contain text

`COUNTA()` may be appropriate.

This distinction was discussed during the initial Excel validation work.

---

## 3. Overall checkpoints

With all report filters cleared, the dashboard produced approximately:

| Metric | Checkpoint |
|---|---:|
| Total Sales | 118.73M |
| Total Profit | 16.89M |
| Profit Margin | 14.23% |
| Total Discounts | 9.21M |
| Units Sold | 1.13M |

These values became the principal cross-checkpoints for the report.

---

## 4. Profit margin validation

Profit margin was validated as:

`Total Profit ÷ Total Sales`

For the overall dataset:

`16.89M ÷ 118.73M ≈ 14.23%`

For Enterprise:

`−614.55K ÷ 19.61M ≈ −3.13%`

The negative sign is meaningful: Enterprise's total profit is negative relative to its sales.

---

## 5. Enterprise validation

The Enterprise filter was used as a controlled test.

Expected approximate values:

- Sales: 19.61M
- Profit: −614.55K
- Margin: −3.13%

If these values changed correctly when the Enterprise slicer was selected, it confirmed that the model/filter context was behaving as intended.

---

## 6. Validation of discount-band analysis

Enterprise margin by discount band:

| Band | Margin |
|---|---:|
| None | +4.00% |
| Low | +1.58% |
| Medium | −3.03% |
| High | −9.53% |

The same general pattern was observed in actual profit:

- None: positive
- Low: positive
- Medium: negative
- High: largest negative result

This cross-check was important because it demonstrated that the trend was not merely an artifact of percentage formatting.

---

## 7. Final QA principle

A dashboard visual was not considered validated merely because it looked plausible.

A result was considered trustworthy when:

1. the underlying measure was logically defined;
2. the Power BI result matched an independent calculation/checkpoint;
3. filtering produced the expected context;
4. the interpretation did not exceed the evidence.
