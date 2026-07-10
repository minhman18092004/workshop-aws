---
title: "Week 5 Worklog"
date: 2026-05-20
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Week 5 Objectives:

* Build a reliable laptop data seeding pipeline.
* Clean and normalize raw product data before insertion.
* Verify the imported records against the database structure.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2   | - Review the target catalog fields and the product attributes required by the NovaTech schema.<br>- Identify how laptop names, specs, and pricing information should be mapped into the database. | 05/18/2026 | 05/18/2026 | content/5-Workshop/5.1-Architecture-Overview/ |
| 3   | - Build a crawler or batch import script to collect realistic laptop data for the initial seed set.<br>- Prepare the raw data in a format that can be transformed into structured records. | 05/19/2026 | 05/19/2026 | content/5-Workshop/5.2-RDS-Database/ |
| 4   | - Clean the imported data, standardize specification values, and remove duplicate records.<br>- Normalize the fields so the dataset fits the relational model consistently. | 05/20/2026 | 05/20/2026 | content/5-Workshop/5.2-RDS-Database/ |
| 5   | - Import the cleaned dataset into the database and confirm that the relations remain valid.<br>- Check that key product fields are stored correctly after insertion. | 05/21/2026 | 05/21/2026 | content/5-Workshop/5.2-RDS-Database/ |
| 6   | - Sample a subset of the imported rows and compare them with the source data.<br>- Result: the seeded catalog was accurate enough for the next implementation stages. | 05/22/2026 | 05/22/2026 | content/5-Workshop/5.1-Architecture-Overview/ |

### Week 5 Achievements:

* Established a repeatable data seeding flow for realistic laptop records.
* Cleaned and normalized product data before database import.
* Confirmed the seeded data could be used as a stable basis for later features.
