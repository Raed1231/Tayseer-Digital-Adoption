# Tayseer: Regional Adoption Funding Recommendation
 
A data-driven funding recommendation for raising digital-service adoption in the Saudi regions that remain below the 65% target. The analysis uses the Tayseer services dataset (synthetic training data) and ends in a proposal to a decision committee: how to split a SAR 40 million budget, and how to release it.
 
> **Note:** All data in this project is synthetic and was provided for training purposes. The figures do not describe real services, users, or regions' actual performance.
 
## Recommendation
 
Approve **SAR 40 million** for the eight regions below the 65% digital-adoption target, allocated in proportion to each region's weighted gap.
 
- **SAR 27 million** goes to Najran, Northern Borders and Al-Baha, which together account for 67.6% of the weighted gap.
- **SAR 13 million** goes to the other five lagging regions: Jazan, Asir, Tabuk, Hail and Al-Jouf.
- Funding is released in phases: **SAR 10 million** first, then the remaining **SAR 30 million** after a 90-day review of measured results.
## Key findings
 
| Finding | Value |
|---|---|
| National adoption, December 2025 | 66.2% (1.2 pp above target) |
| National adoption, January 2022 | 54.1% |
| Change over 48 months | +12.1 pp |
| Target first exceeded | August 2025 |
| Regions below the 65% target | 8 of 13 |
| Largest regional gap | Najran, 60.9% (4.1 pp below target) |
| Share of weighted gap in the top three regions | 67.6% |
 
The national average is above target, but it hides regional differences: eight regions are still below 65%. Regions close to the line, such as Al-Jouf (64.8%) and Hail (64.7%), are treated as below target, because the decision is based on precise values rather than rounded percentages.
 
## Method
 
**Adoption rate** is a user-weighted average:
 
```
Adoption = SUM(digital_adoption_pct × unique_users) / SUM(unique_users)
```
 
**Weighted gap** combines how far a region is below the target with the size of its user weights:
 
```
Weighted gap = (65% − regional adoption) × user weights
```
 
Each region's share of the total weighted gap determines its share of the budget, rounded to the nearest SAR 100,000.
 
- **Baseline:** December 2025
- **Period covered:** January 2022 to December 2025 (48 months)
- **Target:** 65% digital adoption per region
## Proposed allocation
 
| Region | Adoption | Gap (pp) | Allocation (SAR million) |
|---|---|---|---|
| Najran | 60.9% | 4.14 | 12.4 |
| Northern Borders | 62.7% | 2.30 | 7.8 |
| Al-Baha | 62.8% | 2.22 | 6.8 |
| Jazan | 63.0% | 1.97 | 6.6 |
| Asir | 64.4% | 0.64 | 2.7 |
| Tabuk | 64.5% | 0.52 | 2.0 |
| Hail | 64.7% | 0.26 | 1.0 |
| Al-Jouf | 64.8% | 0.18 | 0.7 |
| **Total** | | | **40.0** |
 
Najran alone accounts for 31.1% of the weighted gap, Northern Borders for 19.6%, Al-Baha for 16.9% and Jazan for 16.4%.
 
## Options considered
 
| Option | Use of SAR 40M | Tradeoff |
|---|---|---|
| Equal funding across 13 regions | About SAR 3.08M per region | Funds regions already above target |
| Full focus on three regions | Fund only the top three regions | Leaves Jazan and other gaps unfunded |
| **Weighted funding across eight regions (selected)** | Each region receives its gap share | Requires a review of delivery costs |
 
The selected option concentrates funding on the highest-priority regions while still covering every region below target.
 
## Phased release
 
| Stage | Amount | What happens |
|---|---|---|
| Phase one | SAR 10M | Identify where users stop in the service journey; test simpler steps and digital assistance |
| Within 30 days | | Programme team verifies the baseline and identifies barriers and intervention costs |
| After 90 days | | Committee reviews adoption, improvement costs and comparisons |
| Phase two | SAR 30M | Released, or the intervention adjusted, based on measured results |
 
The 90-day review asks three questions: did adoption improve, at what cost, and does the improvement reflect the intervention or the general upward trend?
 
## Limitations
 
- **Synthetic data.** The dataset is training data, not operational data.
- **User weights are not headcounts.** `unique_users` provides row-level weights. Summing it across channels and services does not give a count of distinct people.
- **No cost or return data.** The dataset contains no intervention costs and no experiment measuring returns, so there is no cost per adoption point or return per riyal. The weighted gap ranks the size of the need; it does not show which region delivers the highest return.
- **Proposals, not causal estimates.** The budget and interventions are planning proposals. The analysis does not claim that SAR 40 million guarantees reaching the target.
- **Charts are reproductions.** The charts are rebuilt from the CSV using the Tableau guide formula; they are not screenshots of a completed team dashboard.
## Data and materials
 
- **Dataset:** `tayseer_services_synthetic.csv`
- **Presentation:** `Tayseer_Presentation_EN.pptx` (7 content slides with speaker notes)
- **Tools:** Tableau, following the Lab 4 Tableau steps student guide

## Acknowledgment

This project was completed as part of a [SDAIA Academy](https://github.com/SDAIAAcademy) training programme Data Visualization & Storytelling.

## Team
 
- Rayan Aloraydi
- Raed Alokaili
- Mohammed Alarifi
- Khaled Alromaizan
 
