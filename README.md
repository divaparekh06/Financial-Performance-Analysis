# Financial Performance Analysis - Power BI

An end-to-end financial data analytics project built from the provided **Financial Data** worksheet and developed in Microsoft Power BI.

The project follows a complete analyst workflow:

**Raw financial data → data understanding → validation → measures → exploratory analysis → dashboard → profitability investigation → insights → recommendations**

The final Power BI report contains three pages:

1. **Executive Overview** - overall sales, profit, margin, products, countries, segments, discounts and trends.
2. **Profitability Deep Dive** - investigation of the Enterprise segment and the relationship between discount intensity and profitability.
3. **Key Insights & Recommendations** - concise executive summary of the findings and recommended actions.

---

## Project objective

The objective was not merely to create a collection of Power BI charts. The goal was to use the financial dataset to answer progressively deeper business questions:

- How is overall financial performance changing?
- Which countries, products and segments contribute to sales and profit?
- How does discounting relate to profitability?
- Which segment requires the most attention?
- Is the profitability problem isolated to a product or country?
- What happens to Enterprise profitability as discount intensity increases?
- Which Enterprise product is weakest?
- What should management investigate or change?

---

## Major finding

The central finding is that **Enterprise is the primary profitability concern**.

Enterprise has an overall profit margin of approximately **−3.13%**. The problem is broad: all six Enterprise products have negative profit margins, and Enterprise remains unprofitable across the countries analyzed.

The strongest observed relationship is between discount intensity and Enterprise profitability:

| Discount Band | Enterprise Profit Margin |
|---|---:|
| None | +4.00% |
| Low | +1.58% |
| Medium | −3.03% |
| High | −9.53% |

Enterprise High-discount sales are approximately **6.5M**, making High the largest Enterprise sales bucket among the discount bands examined. High-discount Enterprise transactions also correspond to the largest profit losses.

At the product level:

- **Carretera** is the weakest Enterprise product by total profit.
- **Montana** is the strongest Enterprise product by total profit.
- Carretera's largest identified loss occurs under the **High** discount band.

> Important analytical qualification: the report establishes a strong association between higher discount intensity and lower Enterprise profitability. It does **not** prove that discounting alone causes the losses.

---

## Overall dashboard values

With all filters cleared, the report produced approximately:

| KPI | Overall value |
|---|---:|
| Total Sales | 118.73M |
| Total Profit | 16.89M |
| Profit Margin | 14.23% |
| Total Discounts | 9.21M |
| Units Sold | 1.13M |

For Enterprise:

| KPI | Enterprise value |
|---|---:|
| Total Sales | 19.61M |
| Total Profit | −614.55K |
| Profit Margin | −3.13% |

Values may display with minor rounding differences depending on Power BI formatting.



**Complete: Analysis, dashboard construction, investigation, recommendations and documentation structure are ready.**
