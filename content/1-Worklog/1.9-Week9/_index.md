---
title: "Week 9 Worklog"
date: 2026-06-17
weight: 1
chapter: false
pre: " <b> 1.9. </b> "
---

### Week 9 Objectives:

* Implement the voucher calculation engine.
* Support both percentage-based and fixed-amount discounts.
* Validate voucher conditions before applying the final price.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2   | - Review the discount scenarios required by the business flow and define the voucher data model.<br>- Identify the fields needed for application rules and pricing logic. | 06/15/2026 | 06/15/2026 | content/1-Worklog/1.9-Week9/ |
| 3   | - Implement voucher types for percentage discounts and fixed-amount discounts.<br>- Map the voucher settings to the pricing flow used by the order process. | 06/16/2026 | 06/16/2026 | content/1-Worklog/1.9-Week9/ |
| 4   | - Add validation rules for expiry date, minimum order value, and voucher usage limits.<br>- Make sure invalid vouchers are rejected before the price is calculated. | 06/17/2026 | 06/17/2026 | content/1-Worklog/1.9-Week9/ |
| 5   | - Compute the final payable amount after discount and verify the math with multiple cases.<br>- Check that the result remains consistent across edge scenarios. | 06/18/2026 | 06/18/2026 | content/1-Worklog/1.9-Week9/ |
| 6   | - Run end-to-end tests for the voucher flow and confirm the discount rules work as expected.<br>- Result: the voucher engine was ready for integration into checkout. | 06/19/2026 | 06/19/2026 | content/1-Worklog/1.9-Week9/ |

### Week 9 Achievements:

* Built a voucher system that supports percentage and fixed discounts.
* Validated the main business rules before discount application.
* Prepared the voucher logic for checkout integration.
