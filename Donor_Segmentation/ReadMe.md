# Donor Segmentation & Fundraising Insights

> Using RFM analysis to identify high-value donor segments, predict churn risk, and guide evidence-based fundraising strategy across 1,000+ donor records.

**Tools:** Python · Pandas · Matplotlib · Seaborn · Scikit-learn · NumPy  
**Dataset:** 1,000 donor records (simulated from real nonprofit giving patterns)  
**Framework:** RFM Analysis (Recency · Frequency · Monetary)  
**Segments Identified:** 7 distinct donor personas

---

## The Business Problem

A nonprofit organization was running campaigns without knowing which donors were worth prioritizing, which were at risk of lapsing, and which had already been lost. Every dollar spent on the wrong donor is a dollar not spent on mission.

**The goal: segment donors by behavior, predict retention risk, and surface the 5 actions the fundraising team can take this week.**

---

## What is RFM Analysis?

RFM is the gold-standard framework for donor and customer segmentation used by nonprofits, healthcare systems, and consumer brands worldwide.

- **Recency** — How recently did they give? (Lower days = better)
- **Frequency** — How many times have they given?
- **Monetary** — How much have they given in total?

Each donor receives a score of 1–5 on each dimension. Combined scores create behavioral segments that predict future giving behavior better than demographics alone.

---

## The 7 Donor Segments

| Segment | Description | Strategy |
| :--- | :--- | :--- |
| Champions | Recent, frequent, high-value | Steward heavily — potential board members |
| Loyal Donors | Consistent givers, mid-value | Upsell to major gifts program |
| Recent Donors | New donors, not yet habitual | Onboard aggressively — first 90 days critical |
| High-Value | Large gifts, less frequent | Personal outreach — major gift cultivation |
| At-Risk | Were loyal, now lapsing | Reactivation campaign — act within 30 days |
| Needs Attention | Mid-tier, inconsistent | Targeted messaging — segment by interest |
| Lost Donors | Long lapsed, low engagement | Low-cost win-back or sunset |

---

## Key Findings

**1. The 180-day retention cliff is real**  
Donors contacted within 180 days of their last gift retain at 72%. After 2 years that drops to 12%. This single insight alone could reshape campaign timing.

**2. Champions are 5% of donors but drive outsized revenue**  
Just 51 donors make up the Champion segment — yet they contribute disproportionately to total funds raised. They deserve personal, high-touch stewardship.

**3. Major Gift Officers deliver the highest avg gift — but low volume**  
The channel analysis reveals MGOs are highest per-gift value but serve the fewest donors. Online drives volume but lower retention — the two channels need different strategies.

**4. 13+ year donors give 3x more and retain at double the rate**  
Tenure is the strongest predictor of lifetime value. Investing in early donor retention pays compounding returns over time.

**5. 34% of donors are in Needs Attention — the biggest opportunity**  
This segment is not lost — they just have not been engaged strategically. A targeted campaign to this group is the highest-ROI opportunity in the database.

---

## Key Metrics

| Metric | Value |
| :--- | ---: |
| Total donors analyzed | 1,000 |
| Total funds raised | $10.3M |
| Average gift size | $10,340 |
| Overall retention rate | 32.8% |
| Retention rate within 180 days | 72% |
| Champion donors | 51 (5%) |
| At-risk donors | 130 (13%) |

---

## Business Recommendations

| Priority | Recommendation | Expected Impact |
| :--- | :--- | :--- |
| High | Launch 30-day reactivation campaign for At-Risk segment | Recover 30-40% before they lapse |
| High | Personal stewardship plan for all 51 Champions | Protect highest-value relationships |
| High | Contact all donors within 90 days of their last gift | Defend the 72% retention window |
| Medium | Shift budget from low-retention Online to Event/MGO channels | Improve retention mix |
| Medium | Create multi-year giving recognition program | Accelerate tenure-based LTV growth |
| Low | Sunset Lost Donors after one low-cost win-back attempt | Reduce wasted outreach spend |

---
## Visualizations

### RFM Donor Segments
![Segments](https://raw.githubusercontent.com/Cinco33/Data_Science_Portfolio/main/Donor_Segmentation/images/01_rfm_segments.png)

### Revenue by Segment
![Revenue](https://raw.githubusercontent.com/Cinco33/Data_Science_Portfolio/main/Donor_Segmentation/images/02_revenue_by_segment.png)

### Average Gift by Donor Type
![Gift](https://raw.githubusercontent.com/Cinco33/Data_Science_Portfolio/main/Donor_Segmentation/images/03_avg_gift_by_type.png)

### Retention Rate by Recency — The 180-Day Cliff
![Retention](https://raw.githubusercontent.com/Cinco33/Data_Science_Portfolio/main/Donor_Segmentation/images/04_retention_by_recency.png)

### Channel Performance — Revenue and Retention
![Channels](https://raw.githubusercontent.com/Cinco33/Data_Science_Portfolio/main/Donor_Segmentation/images/05_channel_performance.png)

### Donor Map — Recency vs Gift Size
![Scatter](https://raw.githubusercontent.com/Cinco33/Data_Science_Portfolio/main/Donor_Segmentation/images/06_rfm_scatter.png)

### Campaign Performance
![Campaigns](https://raw.githubusercontent.com/Cinco33/Data_Science_Portfolio/main/Donor_Segmentation/images/07_campaign_performance.png)

### Donor Lifetime Value by Tenure
![LTV](https://raw.githubusercontent.com/Cinco33/Data_Science_Portfolio/main/Donor_Segmentation/images/08_ltv_by_tenure.png)

### Geographic Distribution
![Geo](https://raw.githubusercontent.com/Cinco33/Data_Science_Portfolio/main/Donor_Segmentation/images/09_geographic_distribution.png)

### KPI Summary
![KPIs](https://raw.githubusercontent.com/Cinco33/Data_Science_Portfolio/main/Donor_Segmentation/images/10_kpi_summary.png)
## How to Run

```bash
git clone https://github.com/Cinco33/Data_Science_Portfolio.git
cd Data_Science_Portfolio/Donor_Segmentation_Fundraising
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook Donor_Segmentation_Analysis.ipynb
```

---

## Project Structure
