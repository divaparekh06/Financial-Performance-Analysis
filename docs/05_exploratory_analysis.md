# 05 — Exploratory Analysis

## 1. Why exploratory analysis came before the dashboard

The dashboard was not designed blindly.

The exploratory phase was used to discover which questions deserved visual treatment.

The main principle was:

> Start broad, identify an anomaly, then investigate the anomaly.

---

## 2. Time analysis

### Sales

Total sales generally increased over time, although the line contained noticeable peaks and drops.

Observation:

> Sales show an overall upward tendency rather than a continuously increasing sequence.

### Profit

Total profit appeared comparatively more stable than sales, with several peaks and fluctuations.

Observation:

> Increasing sales did not automatically translate into proportionally increasing profit.

This was one reason profitability deserved independent analysis rather than being inferred from sales alone.

---

## 3. Segment analysis

The segment comparison identified Enterprise as the major profitability concern.

Enterprise showed an overall negative profit margin.

This created the next analytical question:

> Is Enterprise's poor result caused by one product, one country, or a broader segment-level issue?

---

## 4. Product analysis

Product-level analysis was used to determine whether Enterprise weakness was concentrated.

When Enterprise was selected:

- all six products had negative profit margins;
- Carretera was the lowest-profit product;
- Montana was the highest-profit product.

Observation:

> Enterprise's profitability problem is portfolio-wide, although product performance differs materially.

---

## 5. Country analysis

Enterprise was filtered and profitability was examined by country.

The countries analyzed all remained negative for Enterprise.

Observation:

> The Enterprise issue is not isolated to one geography.

This shifted attention away from a country-specific explanation and toward broader commercial/product economics.

---

## 6. Discount-band analysis

This became the central diagnostic investigation.

Enterprise profit margins:

| Discount Band | Profit Margin |
|---|---:|
| None | +4.00% |
| Low | +1.58% |
| Medium | −3.03% |
| High | −9.53% |

Observation:

> Profitability deteriorates progressively as discount intensity increases.

---

## 7. Actual profit by discount band

The analysis then moved from percentage margin to actual profit.

Why?

A margin percentage alone does not communicate financial magnitude.

The actual-profit visual showed:

- None → positive
- Low → positive
- Medium → negative
- High → largest negative

Observation:

> The deterioration in margin corresponds to actual financial losses, not merely a percentage presentation effect.

---

## 8. Sales by discount band

Enterprise sales by discount band were then examined.

Approximate High-discount Enterprise sales:

**6.5M**

High was the largest Enterprise sales bucket among the discount bands analyzed.

Observation:

> The high-discount problem affects a substantial amount of Enterprise revenue.

---

## 9. Discount rate analysis

To quantify discount intensity, the following was calculated:

`Discount Rate = Discounts ÷ Gross Sales`

Approximate Enterprise values:

| Band | Rate |
|---|---:|
| None | ~0% |
| Low | ~2.4% |
| Medium | ~6.8% |
| High | ~12.5% |

Observation:

> The categorical discount bands correspond to progressively larger effective discount rates.

---

## 10. Product × Discount investigation

The final drill-down used:

- Product as rows
- Discount Band as columns
- Total Profit as values

Conditional formatting made negative and positive profit visually obvious.

Key observation:

> Carretera is the weakest Enterprise product, and its largest identified loss occurs in the High discount band.

Montana was identified as the strongest Enterprise product by total profit.

---

## 11. Analytical progression

The complete reasoning chain was:

**Enterprise is unprofitable**
→ Is it one country?
→ No.

**Is it one product?**
→ No; all six products are negative.

**Does discount intensity relate to margin?**
→ Yes; margin declines from +4.00% to −9.53%.

**Is this financially significant?**
→ Yes; High-discount Enterprise sales are ~6.5M and High corresponds to the largest losses.

**Where is the weakest product-level combination?**
→ Carretera + High discount.

This progression is the central analytical story of the project.
