---
title: "Week 11 Worklog"
date: 2026-07-01
weight: 2
chapter: false
pre: " <b> 1.11. </b> "
---

### Week 11 Objectives:

* Prepare the deployment configuration for GitOps-style operations.
* Separate application code from infrastructure and runtime definitions.
* Verify that configuration changes can be tracked and applied cleanly.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2   | - Review the current deployment layout and decide which files should live outside the application repository.<br>- Identify the runtime values and manifests that need to be moved to a separate config space. | 06/29/2026 | 06/29/2026 | content/1-Worklog/1.12-Week12/ |
| 3   | - Create or clean up the dedicated deployment repository structure for YAML and compose files.<br>- Keep the deployment configuration focused and isolated from source code. | 06/30/2026 | 06/30/2026 | content/1-Worklog/1.12-Week12/ |
| 4   | - Prepare the sync mechanism that watches configuration changes and applies them to the target environment.<br>- Check that the deployment flow follows a pull-based model. | 07/01/2026 | 07/01/2026 | content/1-Worklog/1.12-Week12/ |
| 5   | - Test a configuration drift scenario and confirm that the deployment state can be restored from Git.<br>- Make sure the server side remains aligned with the repository state. | 07/02/2026 | 07/02/2026 | content/1-Worklog/1.12-Week12/ |
| 6   | - Review the overall deployment workflow and finalize the notes needed for the final monitoring week.<br>- Result: the GitOps preparation was complete. | 07/03/2026 | 07/03/2026 | content/1-Worklog/1.12-Week12/ |

### Week 11 Achievements:

* Separated deployment configuration from application code.
* Prepared a GitOps-oriented sync model for deployment changes.
* Verified the system could recover from configuration drift.
