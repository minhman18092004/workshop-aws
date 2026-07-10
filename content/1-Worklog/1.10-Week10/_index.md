---
title: "Week 10 Worklog"
date: 2026-06-24
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Week 10 Objectives:

* Containerize the application services for repeatable deployment.
* Finalize the Docker Compose setup and service networking.
* Keep sensitive values outside the container images.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2   | - Refactor the existing Dockerfiles for the frontend and backend so the build and runtime steps remain separated.<br>- Reduce the chance of leaking environment-specific values into the images. | 06/22/2026 | 06/22/2026 | content/1-Worklog/1.3-Week3/ |
| 3   | - Define the Docker Compose stack for the frontend, backend, database, cache, and auxiliary services.<br>- Check that every container can resolve the others on the internal network. | 06/23/2026 | 06/23/2026 | content/1-Worklog/1.3-Week3/ |
| 4   | - Configure external environment bindings for the containers and verify the service-specific runtime values.<br>- Make the deployment easier to move between local and server environments. | 06/24/2026 | 06/24/2026 | content/1-Worklog/1.3-Week3/ |
| 5   | - Add persistent volumes where state must survive restarts and container recreation.<br>- Confirm that the database and supporting services keep their data. | 06/25/2026 | 06/25/2026 | content/1-Worklog/1.3-Week3/ |
| 6   | - Run the full stack locally and check that the application can start with a single orchestration command.<br>- Result: the project was ready for deployment workflow testing. | 06/26/2026 | 06/26/2026 | content/1-Worklog/1.3-Week3/ |

### Week 10 Achievements:

* Containerized the main application services.
* Built a reusable Docker Compose deployment stack.
* Kept runtime configuration external to the images.
