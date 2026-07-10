---
title: "Week 4 Worklog"
date: 2026-05-13
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Week 4 Objectives:

* Set up the image storage layer for product assets.
* Keep the S3 bucket private while serving files through CloudFront.
* Move storage-related values into external configuration for later deployment.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2   | - Review the storage requirements for product images and confirm why the application server should not host all assets directly.<br>- Identify the private storage flow between S3 and CloudFront. | 05/11/2026 | 05/11/2026 | content/5-Workshop/5.3-S3-Storage/ |
| 3   | - Configure the S3 bucket and update the access policy so only CloudFront can read objects.<br>- Verify that image delivery works through the CDN domain instead of the raw bucket URL. | 05/12/2026 | 05/12/2026 | content/5-Workshop/5.3-S3-Storage/ |
| 4   | - Integrate the backend storage service with the AWS SDK and prepare upload/delete flows for product images.<br>- Result: image handling could be performed through the API layer. | 05/13/2026 | 05/13/2026 | content/5-Workshop/5.3-S3-Storage/ |
| 5   | - Externalize the bucket name, region, and access credentials into environment variables.<br>- Keep the deployment configuration separate from source code. | 05/14/2026 | 05/14/2026 | content/5-Workshop/5.3-S3-Storage/ |
| 6   | - Recheck the full storage path from the backend to S3 and then to CloudFront.<br>- Result: the image delivery flow was ready for production-style deployment. | 05/15/2026 | 05/15/2026 | content/5-Workshop/5.3-S3-Storage/ |

### Week 4 Achievements:

* Built a private and CDN-based storage approach for product images.
* Connected the backend to S3 through the AWS SDK and standardized runtime configuration.
* Prepared the storage layer for later deployment and scaling work.
