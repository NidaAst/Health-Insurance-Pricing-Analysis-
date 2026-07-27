# Health-Insurance-Pricing-Analysis-
An analysis of health insurance charge drivers (smoking, BMI, age) using Python and Pandas — found smoking + obesity compound to nearly double costs

## Overview
Analysed a dataset of 1,338 health insurance policyholders to identify the key factors driving insurance charges, using Python and Pandas.

## Key Findings

**Smoking status** Smoking status was the single strongest driver of charges. Smokers were charged on average **£32,050** compared to **£8,434** for non-smokers — roughly 3.8x higher.

**BMI** had little effect on charges on its own however, it became a powerful driver when combined with smoking status. Among smokers, those with a BMI over 30 (obese) were charged **£41,558** on average versus **£21,363** for non-obese smokers — nearly double.

**Combined risk analysis** confirmed an interaction effect rather than a simple additive one:
| Group | Avg Charges | Sample Size |
|---|---|---|
| Non-smoker, Not Obese | £7,977 | 502 |
| Non-smoker, Obese | £8,821 | 562 |
| Smoker, Not Obese | £21,363 | 129 |
| Smoker, Obese | £41,558 | 145 |

Obesity alone increased charges by only ~11% among non-smokers, but among smokers, obesity nearly doubled the charges hence showcasing smoking and obesity compound each other's cost impact rather than simply adding together.

**Age** showed a gradual, consistent rise in charges within both smoking groups, with smokers remaining substantially higher across all ages.

**Region** showed modest differences, with the Southeast averaging the highest charges (£14,700) compared to elsewhere (£12,300–13,400).

**Number of children** showed a mild rise in charges from 0–3 children, though results for 4–5 children were unreliable due to small sample sizes (n=25 and n=18 respectively).

## Tools Used
Python, Pandas, Matplotlib

## Files
- `insurance_analysis.ipynb` — full analysis notebook with code, charts, and comments.
