---
title: "Week 2 Worklog"
date: 2026-04-29
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Week 2 Objectives:

* Finalize the managed PostgreSQL database approach for transactional data.
* Secure backend configuration by externalizing connection values.
* Verify that the application can connect to the database under the new setup.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2   | - Create the RDS PostgreSQL instance and keep public access disabled.<br>- Review the endpoint, port, and VPC placement used for the database layer.<br>- Result: the database service was available inside the private network.<br>- Difficulty: connection scope had to be kept narrow for security.<br>- Next step: allow only the application server to reach the database. | 04/27/2026 | 04/27/2026 | content/5-Workshop/5.2-RDS-Database/ |
| 3   | - Add the database credentials to runtime environment variables instead of hardcoding them.<br>- Map the values into the Spring Boot datasource configuration.<br>- Result: the backend could read DB_URL, DB_USERNAME, and DB_PASSWORD at startup.<br>- Difficulty: the runtime values had to match the RDS endpoint exactly.<br>- Next step: test whether the application connects successfully with the injected values. | 04/28/2026 | 04/28/2026 | content/5-Workshop/5.2-RDS-Database/ |
| 4   | - Run the backend against the new database settings and confirm the connection path.<br>- Check that the schema and JPA settings behaved as expected in the deployment profile.<br>- Result: the backend could access PostgreSQL through the managed endpoint.<br>- Difficulty: any mismatch in host or password immediately blocked startup.<br>- Next step: keep the same pattern for other external services and configuration values. | 04/29/2026 | 04/29/2026 | content/5-Workshop/5.2-RDS-Database/ |

### Week 2 Achievements:

* Established a secure PostgreSQL deployment model using Amazon RDS.
* Externalized the database configuration so the backend no longer depended on hardcoded credentials.
* Confirmed that the Spring Boot application could connect to the managed database layer.
