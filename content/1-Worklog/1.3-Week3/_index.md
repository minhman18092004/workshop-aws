---
title: "Week 3 Worklog"
date: 2026-05-06
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---

### Week 3 Objectives:

* Start the containerization baseline for both frontend and backend.
* Externalize runtime settings so the application can be deployed in multiple environments.
* Prepare the project structure for a GitOps-style deployment workflow.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2   | - Review the current frontend and backend startup flow to identify values that should be injected at runtime rather than hardcoded.<br>- List the environment variables needed for later deployment work. | 05/04/2026 | 05/04/2026 | content/5-Workshop/5.2-RDS-Database/ |
| 3   | - Draft the initial Dockerfile structure for the backend service using a clean runtime image flow.<br>- Keep the build process separate from runtime settings. | 05/05/2026 | 05/05/2026 | content/5-Workshop/5.6-Non-AWS-Services/ |
| 4   | - Draft the frontend Dockerfile and verify that the application can be started with external configuration values.<br>- Confirm that the image build does not embed environment-specific secrets. | 05/06/2026 | 05/06/2026 | content/5-Workshop/5.6-Non-AWS-Services/ |
| 5   | - Align the configuration approach between frontend and backend so both services can read the same deployment values.<br>- Prepare for future container orchestration steps. | 05/07/2026 | 05/07/2026 | content/5-Workshop/5.6-Non-AWS-Services/ |
| 6   | - Review the prepared container setup and check that the project can later be moved into a GitOps deployment model.<br>- Result: the deployment foundation was ready for the next stages. | 05/08/2026 | 05/08/2026 | content/5-Workshop/5.6-Non-AWS-Services/ |

### Week 3 Achievements:

* Prepared the initial Dockerfile strategy for both frontend and backend.
* Moved the project closer to environment-based deployment by separating runtime settings from source code.
* Established the groundwork needed for the later GitOps and container orchestration phases.
