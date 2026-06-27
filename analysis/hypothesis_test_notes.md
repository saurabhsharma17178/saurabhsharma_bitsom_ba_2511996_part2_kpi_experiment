# Hypothesis Test Notes

## 1. Null Hypothesis (H0)

The new onboarding campaign (Treatment Group) does not improve the Paid Conversion Rate compared to the Control Group.

---

## 2. Alternative Hypothesis (H1)

The new onboarding campaign (Treatment Group) improves the Paid Conversion Rate compared to the Control Group.

---

## 3. Type of Test

One-tailed hypothesis test.

Reason:
The business objective is to determine whether the Treatment Group performs better than the Control Group, not just whether it is different.

---

## 4. Significance Level

Alpha (α) = 0.05

A 95% confidence level is used for the experiment.

---

## 5. Metric Being Tested

Primary Metric:
- Paid Conversion Rate

Supporting Metrics:
- Trial Start Rate
- Onboarding Completion Rate
- Average Revenue Per User
- Engagement Score

Guardrail Metrics:
- Refund Rate
- Support Ticket Rate

---

## 6. Reason for Choosing This Metric

Paid Conversion Rate is the North Star Metric because it directly measures business success by indicating how many users become paying customers after experiencing the new onboarding process.

An increase in paid conversions leads to higher revenue and business growth.

---

## 7. Interpretation Logic

If the Treatment Group shows a statistically significant improvement in Paid Conversion Rate (p-value < 0.05), and there is no unacceptable increase in refund rate or support tickets, the new onboarding campaign should be recommended for rollout.

If the improvement is not statistically significant, or if guardrail metrics worsen considerably, the existing onboarding experience should be retained until further improvements are made.

## Test Output

### Test Inputs

- Control Users: 675
- Treatment Users: 715
- Control Conversions: 22
- Treatment Conversions: 50

### Results

- Control Conversion Rate: 3.26%
- Treatment Conversion Rate: 6.99%

### Decision Rule

Since the Treatment Group achieved a substantially higher Paid Conversion Rate than the Control Group, the Null Hypothesis is rejected at the chosen significance level (α = 0.05).

### Business Interpretation

The new onboarding campaign improved paid conversions. Based on the experiment results, the Treatment experience is recommended for rollout, while continuing to monitor guardrail metrics such as refund requests and support tickets.

# Task 8: Guardrail Metrics Evaluation

## 1. Refund Rate

- Control: 0.00%
- Treatment: 0.42%

Evaluation:
The Treatment Group shows a slight increase in refund requests. However, the increase is small and does not currently indicate a major business risk.

Risk Level: Low

---

## 2. Support Ticket Rate

- Control: 21.93%
- Treatment: 37.20%

Evaluation:
The Treatment Group generated more customer support tickets than the Control Group. This may indicate that users require additional assistance during onboarding.

Risk Level: Medium

---

## 3. Average Days to Convert

- Control: 8.86 Days
- Treatment: 6.40 Days

Evaluation:
Users in the Treatment Group converted faster than those in the Control Group, indicating a positive business impact.

Risk Level: None

---

## 4. Average Engagement Score

- Control: 56.97
- Treatment: 62.93

Evaluation:
User engagement improved in the Treatment Group, suggesting that the new onboarding experience is more effective.

Risk Level: None

---

## Overall Guardrail Assessment

Although the Treatment Group has a slightly higher refund rate and a noticeable increase in support ticket rate, it also achieves:

- Higher Paid Conversion Rate
- Faster Conversion
- Higher Engagement

Overall, the benefits outweigh the risks. The Treatment campaign is recommended for rollout while monitoring refund requests and customer support volume after launch.