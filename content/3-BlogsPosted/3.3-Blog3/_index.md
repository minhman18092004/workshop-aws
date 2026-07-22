---
title: "Blog 3"
date: 2026-07-18
weight: 3
chapter: false
pre: " <b> 3.3. </b> "
---
# BLOG 3: THE AWS SAVINGS PLANS TRAP: SAVING 72% ON A WASTEFUL SYSTEM IS STILL... WASTEFUL!

When an AWS bill starts ballooning, the natural reflex of financial executives or Tech Leads is to find immediate discounts. The most frequently proposed "gold standard" solution is **AWS Savings Plans** or **Reserved Instances (RI)**—committing to a 1-to-3-year usage term in exchange for steep discounts of up to 72%.

Sounds like a great deal, right? But this is precisely where the financial trap lies!

---

## 1. The Trap: Locking Yourself into Waste

Imagine you are running an EC2 instance of type `m5.2xlarge` (8 vCPUs, 32 GiB RAM) costing roughly **$270/month**. Seeing the high bill, you decide to purchase a 3-year Compute Savings Plan to get a 50% discount. You sigh with relief, thinking you've slashed your bill in half.

However, the reality is that your system only ever utilizes up to 10% of its CPU and RAM. Technically, an `m5.large` instance (2 vCPUs, 8 GiB RAM) with a base price of around **$70/month** would run your workload seamlessly.

By rushing to buy a Savings Plan:
- **You lock yourself into over-provisioned hardware**: You commit to an unnecessary configuration for 3 full years.
- **You pay more than actual needs dictate**: You pay **$135/month** (after discount) for a workload that should only cost **$70/month** (at base, non-discounted rates).
- **You continue wasting money daily**: You are still overspending every day under the guise of "discounted pricing."

---

## 2. The Art of FinOps: "Shrink First, Commit Later"

To avoid wasting capital, the standard operating procedure for cloud engineers should always be: **Optimize your resources first (Right-sizing), then purchase commitments later (Commitment)**.

### Step 1: Let AWS Compute Optimizer guide you
Before committing funds, enable the free tool **AWS Compute Optimizer**. It uses machine learning to scan your EC2 usage history, pinpointing underutilized instances and recommending downsizing options or migrations to energy-efficient ARM-based AWS Graviton (`m7g`) instances.

### Step 2: Clean up orphaned resources
Decommission unused "orphaned" instances in Dev/Test environments before measuring the actual capacity needed for long-term commitments.

### Step 3: Lock in the commitment
Only after your infrastructure has been streamlined and trimmed of excess capacity should you use those baseline metrics to purchase Savings Plans.

---

## 3. Insightful Data Direct from AWS

According to *"The AWS State of Cost Efficiency Report"* published on the official AWS Cloud Financial Management Blog:

> "Organizations that combine both rightsizing and commitments improve their cost efficiency score **4 TIMES FASTER** than those that focus solely on buying Savings Plans without first optimizing their infrastructure." 
> 
> *— Source: AWS Cloud Financial Management Blog*

This **4x multiplier** proves that architectural optimization delivers far more sustainable value and deeper savings than purchasing financial discounts alone.

---

## 4. Conclusion & Discussion

**Key Takeaway:** Buying AWS Savings Plans is fantastic, but build them on top of a lean infrastructure. **Don't apply discounts to wasted capacity!**

Have you ever accidentally locked into a Savings Plan for an over-provisioned system? Feel free to share your experiences or discuss below!

---

## 5. Reference Links

Read the full report on the official AWS Cloud Financial Management Blog: 👉 [The AWS State of Cost Efficiency Report](https://aws.amazon.com/blogs/aws-cloud-financial-management/the-aws-state-of-cost-efficiency-report/)

## 6. Post Link

View the detailed post and join the discussion on Facebook: 👉 [Facebook Shared Post](https://www.facebook.com/groups/awsstudygroupfcj/permalink/2213983459366614/?rdid=xKQVbSx1f2LiQL6y#)