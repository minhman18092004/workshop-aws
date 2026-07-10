---
title: "Week 8 Worklog"
date: 2026-06-10
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---

### Week 8 Objectives:

* Configure user authentication for the application.
* Connect the frontend with AWS Cognito sign-up and sign-in flows.
* Ensure runtime settings are injected through environment variables.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2   | - Review the Cognito integration flow and confirm the authentication endpoints required by the frontend.<br>- Identify the environment values that must be provided at runtime. | 06/08/2026 | 06/08/2026 | content/5-Workshop/5.4-Cognito-Auth/ |
| 3   | - Configure Amplify and link the frontend to the Cognito user pool and app client identifiers.<br>- Make sure the app can read the authentication settings from the environment. | 06/09/2026 | 06/09/2026 | content/5-Workshop/5.4-Cognito-Auth/ |
| 4   | - Implement sign-up and confirmation flows and validate the registration process end to end.<br>- Check that the authentication state is handled correctly after account creation. | 06/10/2026 | 06/10/2026 | content/5-Workshop/5.4-Cognito-Auth/ |
| 5   | - Add sign-in handling and verify token-based access to protected routes in the application.<br>- Test the login journey with a real account. | 06/11/2026 | 06/11/2026 | content/5-Workshop/5.4-Cognito-Auth/ |
| 6   | - Review the authentication configuration and confirm that the runtime values are stable.<br>- Result: the user login flow was ready for the next integration steps. | 06/12/2026 | 06/12/2026 | content/5-Workshop/5.4-Cognito-Auth/ |

### Week 8 Achievements:

* Connected the frontend to Cognito-based authentication flows.
* Externalized the auth settings for runtime configuration.
* Verified that registration and login worked end to end.
