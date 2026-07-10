---
title: "Week 6 Worklog"
date: 2026-05-27
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Week 6 Objectives:

* Prepare the application server environment for real deployment.
* Connect the backend runtime with systemd, reverse proxy, and the payment flow.
* Standardize external configuration for the deployed application.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2   | - Review the DigitalOcean server configuration and prepare the Ubuntu environment for the backend application.<br>- Confirm that the deployment host is ready for remote access and package installation. | 05/25/2026 | 05/25/2026 | content/5-Workshop/5.6-Non-AWS-Services/ |
| 3   | - Install the Java runtime and register the backend JAR as a systemd service.<br>- Ensure the service can start automatically and run in the background. | 05/26/2026 | 05/26/2026 | content/5-Workshop/5.6-Non-AWS-Services/ |
| 4   | - Configure Nginx as a reverse proxy for the API domain and forward public traffic to the backend's internal port.<br>- Check that the server responds correctly through the proxy layer. | 05/27/2026 | 05/27/2026 | content/5-Workshop/5.6-Non-AWS-Services/ |
| 5   | - Add HTTPS support for the deployment endpoint and keep the runtime values in a separate environment file.<br>- Synchronize the deployment settings with the current management model. | 05/28/2026 | 05/28/2026 | content/5-Workshop/5.6-Non-AWS-Services/ |
| 6   | - Integrate the PayOS payment flow and verify that payment link and QR code generation work correctly.<br>- Result: the server was ready for a secure end-to-end backend deployment. | 05/29/2026 | 05/29/2026 | content/5-Workshop/5.6-Non-AWS-Services/ |

### Week 6 Achievements:

* Set up the application server with systemd and Nginx.
* Standardized runtime configuration through an external environment file.
* Verified that the deployed backend could support the payment workflow.
