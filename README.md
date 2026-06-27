# Part 2: KPI Framework, Business Experiment Analysis & Decision Recommendation

## 1. Project Summary

This project analyzes an A/B experiment conducted for a subscription-based digital product company. The objective was to evaluate whether a new onboarding and activation experience (Treatment Group) should replace the existing onboarding process (Control Group).

The analysis includes KPI framework design, experiment analysis, hypothesis testing, guardrail metric evaluation, and a final business recommendation.

---

# 2. Business Problem

The company launched a new onboarding campaign to improve user activation and paid conversions.

The business decision is to determine whether the Treatment experience should be launched to all users based on experiment results.

---

# 3. Dataset Description

Dataset File:

* campaign_experiment_data.xlsx

Dataset contains:

* User information
* Experiment Group (Control / Treatment)
* Region
* Device Type
* Traffic Source
* Plan Type
* Landing Page Visit
* Trial Start
* Onboarding Completion
* Paid Conversion
* Revenue (30 Days)
* Support Tickets
* Refund Requests
* Days to Convert
* Engagement Score

---

# 4. Business Objective

Evaluate whether the new onboarding campaign improves business performance while maintaining acceptable guardrail metrics.

---

# 5. North Star Metric

**Paid Conversion Rate**

Reason:

Paid Conversion Rate directly measures business growth because it represents the percentage of users who become paying customers after onboarding.

Supporting KPIs:

* Landing Page Visit Rate
* Trial Start Rate
* Onboarding Completion Rate
* Average Revenue Per User

Guardrail Metrics:

* Refund Rate
* Support Ticket Rate
* Days to Convert
* Engagement Score

---

# 6. KPI Framework

North Star Metric

Paid Conversion Rate

Primary Drivers

* Landing Page Visit Rate
* Trial Start Rate
* Onboarding Completion Rate

Sub Drivers

* Device Type
* Region
* Traffic Source
* Plan Type

Guardrail Metrics

* Refund Rate
* Support Ticket Rate
* Days to Convert
* Engagement Score

---

# 7. Data Preparation

The following data quality checks were performed:

* Missing value analysis
* Duplicate User ID check
* Group count validation
* Binary value validation
* Revenue outlier review
* Segment distribution verification

No critical data quality issues affecting the experiment were identified.

---

# 8. Experiment Summary

| Metric                   | Control | Treatment |
| ------------------------ | ------: | --------: |
| User Count               |     675 |       715 |
| Paid Conversion Rate     |   3.26% |     6.99% |
| Refund Rate              |   0.00% |     0.42% |
| Support Ticket Rate      |  21.93% |    37.20% |
| Average Engagement Score |   56.97 |     62.93 |
| Average Days to Convert  |    8.86 |      6.40 |

Treatment outperformed Control on the primary business metric.

---

# 9. Hypothesis Testing

Null Hypothesis (H0)

The new onboarding campaign does not improve Paid Conversion Rate.

Alternative Hypothesis (H1)

The Treatment onboarding experience improves Paid Conversion Rate.

Test Type

One-tailed hypothesis test

Significance Level

α = 0.05

Test Inputs

* Control Users = 675
* Treatment Users = 715
* Control Converted Users = 22
* Treatment Converted Users = 50

Conclusion

Treatment achieved a higher Paid Conversion Rate (6.99%) compared to Control (3.26%).

The Null Hypothesis is rejected.

---

# 10. Guardrail Metrics Evaluation

Refund Rate

* Slight increase
* Low business risk

Support Ticket Rate

* Increased
* Medium business risk

Days to Convert

* Improved
* Positive impact

Engagement Score

* Improved
* Positive impact

Overall, the improvement in conversion outweighs the increase in support demand.

---

# 11. Segment Analysis

Segment-level analysis was performed for:

* Region
* Device Type
* Traffic Source

Treatment generally showed stronger performance across major customer segments.

---

# 12. Final Recommendation

## Recommendation

**Launch the Treatment onboarding experience.**

Reason:

* Paid Conversion Rate improved significantly.
* User engagement increased.
* Users converted faster.
* Revenue performance improved.
* Refund rate remained low.

Support ticket volume should continue to be monitored after rollout.

---

# 13. Repository Structure

```
part2_kpi_experiment/

├── data/
│   └── campaign_experiment_data.xlsx
│
├── analysis/
│   ├── experiment_analysis.xlsx
│   └── hypothesis_test_notes.md
│
├── outputs/
│   ├── experiment_summary.xlsx
│   ├── recommendation_memo.md
│   └── kpi_tree.png
│
├── screenshots/
│   ├── summary_metrics.png
│   ├── hypothesis_test_output.png
│   └── kpi_tree_preview.png
│
└── README.md
```

---

# 14. Files Included

* campaign_experiment_data.xlsx
* experiment_analysis.xlsx
* experiment_summary.xlsx
* hypothesis_test_notes.md
* recommendation_memo.md
* kpi_tree.png
* summary_metrics.png
* hypothesis_test_output.png
* kpi_tree_preview.png
* README.md

---

# 15. Key Business Insights

* Treatment nearly doubled the Paid Conversion Rate.
* User engagement improved.
* Users converted more quickly.
* Refund rate remained acceptable.
* Support tickets increased and should be monitored after rollout.

---

# 16. Assumptions

* Paid Conversion Rate is the primary success metric.
* Experiment groups were randomly assigned.
* Dataset accurately represents experiment outcomes.

---

# 17. Limitations

* Results are based on a single experiment period.
* Long-term customer retention was not evaluated.
* Further monitoring is recommended after rollout.

---

# 18. Screenshots Included

* summary_metrics.png
* hypothesis_test_output.png
* kpi_tree_preview.png
