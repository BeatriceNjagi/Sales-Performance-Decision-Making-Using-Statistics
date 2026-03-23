# Sales Performance & Decision-Making Using Statistics

A data analysis project exploring monthly sales revenue using descriptive statistics and hypothesis testing — to understand how sales are performing and whether a new marketing strategy is improving revenue.

---

## Project Overview

This project uses statistical analysis on monthly revenue data to answer three practical business questions:

1. How is sales performance trending?
2. How reliable are the insights from this data?
3. Has a new marketing strategy actually improved revenue?

---

## Tools Used

- **Python** — data analysis and statistical testing
- **Pandas** — data manipulation
- **Statsmodels** — hypothesis testing
- **Matplotlib** — visualisation

---

## Part 1 — Sales Performance Summary

### Measures of Central Tendency

| Measure | Value |
|---|---|
| Mean | 248,159 |
| Median | 250,309 |
| Mode | 105,775 |

The mean and median are nearly identical, indicating a stable, balanced distribution with no major outliers. The lower mode points to a recurring group of below-average months.

### Measures of Dispersion

| Measure | Value |
|---|---|
| Range | 198,604 |
| Variance | 1,199,955,652 |
| Standard Deviation | 34,640 |

A standard deviation of ~34K against a mean of ~248K reflects moderate month-to-month variability — typical for most businesses, but worth managing.

---

## Part 2 — Did the Marketing Campaign Work?

To find out, we compared revenue during campaign periods vs. non-campaign periods using a one-tailed hypothesis test.

**Hypotheses:**

```
H₀: Mean revenue (campaign) = Mean revenue (no campaign)
H₁: Mean revenue (campaign) > Mean revenue (no campaign)
```

### Test Results

| Metric | Result |
|---|---|
| Test Statistic | 4.34 |
| P-value | 0.0000162 |
| Effect Size (Cohen's d) | 0.262 |
| Decision | Reject H₀ |

**P-value (0.0000162):** A p-value this low means there is only a 0.00162% chance the revenue difference occurred by chance. This is strong statistical evidence that the campaign had a real effect.

**Effect size (Cohen's d = 0.262):** A small to moderate effect — the campaign increased revenue in a meaningful but not dramatic way.

| Cohen's d | Interpretation |
|---|---|
| < 0.2 | Negligible |
| 0.2 – 0.5 | Small to moderate |
| 0.5 – 0.8 | Medium |
| > 0.8 | Large |

---

## Key Insights

- Sales are generally stable, with mean and median close together and moderate variability.
- Certain months consistently underperform, pulling the mode significantly below the average.
- The marketing campaign has had a statistically significant positive effect on revenue, though the practical impact is moderate.
- Results are highly reliable — low p-value, balanced data distribution, and consistent effect size all reinforce confidence in the findings.

---

## Recommendations

1. **Target low-performing months** — use promotions or campaigns to lift revenue during periods that consistently fall below average.
2. **Maximise peak months** — ensure inventory, staffing, and marketing are fully supported during high-revenue periods.
3. **Monitor continuously** — track revenue month-over-month to assess whether the campaign's impact grows or plateaus over time.
4. **Investigate the root cause of low months** — understanding seasonal or operational drivers will enable more targeted interventions.

---

## Conclusion

The analysis confirms that the marketing campaign has a statistically significant positive effect on revenue, with a small to moderate practical impact. Sales are stable overall, but low-performing months present a clear opportunity for improvement. Continued monitoring and targeted strategy adjustments will be key to driving more consistent growth.

---

*Analysis by [Beatrice Njagi](https://github.com/BeatriceNjagi)*
