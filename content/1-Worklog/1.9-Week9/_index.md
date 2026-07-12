---
title: "Worklog Week 9"
date: 2026-07-05
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Week 9 Objectives:

* Precisely define the Minimum Viable Product (MVP) scope for the Examora project, ensuring a strategic focus on high-value core functionalities.
* Conduct a comprehensive code review of the existing Frontend and Backend source code to facilitate a seamless architectural migration process.
* Finalize the AWS Serverless Hybrid Architecture design, strategically blending traditional infrastructure components with AWS managed services.
* Deploy a robust, end-to-end authentication and authorization solution utilizing Amazon Cognito in tandem with Amazon SES for automated email delivery.
* Package and migrate the legacy Express Backend application to an AWS Lambda environment, securing all endpoints using API Gateway JWT Authorizers.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Define the MVP Scope & Architecture <br> - **Details:** <br>&emsp; + Analyze business requirements to strictly define essential MVP features (e.g., Authentication, Profile Management, Examination execution). <br>&emsp; + Evaluate the existing Node.js/Express codebase, decoupling tightly integrated modules to streamline serverless or containerized deployments. <br>&emsp; + Consolidate the AWS Serverless Hybrid architectural blueprint, mapping out interaction flows between internal VPCs and public AWS services. | 15/06/2026 | 15/06/2026 | |
| 3 | - Self-study Monitoring Services <br> - **Practice:** <br>&emsp; + Conduct an in-depth exploration of CloudWatch Logs to establish a centralized log monitoring strategy tailored for Production environments. <br>&emsp; + Examine the distinct log structures of AWS Lambda functions, analyzing initialization metrics (Cold Start), execution Duration, and Billed Duration. <br>&emsp; + Formulate robust Log Insights queries to rapidly isolate and diagnose Exceptions originating from the Node.js source code. | 16/06/2026 | 16/06/2026 | |
| 4 | - Prepare Test Cases for Authentication Migration <br> - **Details:** <br>&emsp; + Compile an exhaustive checklist of critical Frontend application flows requiring regression testing post-migration to the Cognito authentication system. <br>&emsp; + Define comprehensive edge-case scenarios encompassing JWT token issuance, expiration handling, and seamless token refresh mechanisms. <br>&emsp; + Draft mock datasets corresponding to diverse user roles to proactively assess potential security vulnerabilities prior to full integration. | 17/06/2026 | 17/06/2026 | |
| 5 | - Test Cognito Authentication Integration <br> - **Practice:** <br>&emsp; + Integrate the AWS Amplify SDK (or Cognito Identity libraries) into the localized Frontend development environment. <br>&emsp; + Execute end-to-end testing of core user workflows, including Sign-in, Sign-out, and Forgot Password recovery processes. <br>&emsp; + Capture and systematically record exceptions related to Token validation and Session timeouts, iteratively refining client-side error handling logic. | 18/06/2026 | 18/06/2026 | |
| 6 | - Test User Groups & Role Synchronization <br> - **Practice:** <br>&emsp; + Simulate a privilege escalation workflow by transitioning a user from the `STUDENT` group to the `TEACHER` group directly via the Amazon Cognito Console. <br>&emsp; + Implement event-driven mechanisms (webhooks or Lambda Triggers) to synchronize the updated user role state to the `giaovien` collection within the MongoDB database. <br>&emsp; + Verify data integrity and authorization enforcement: ensure newly minted tokens accurately reflect the updated group claim and that the Backend API responds appropriately based on role permissions. | 19/06/2026 | 19/06/2026 | |

### Week 9 Results:

* Achieved a thorough understanding of the interlinked frontend/backend codebase structure, successfully delineating modules to retain and components requiring AWS refactoring.
* Deployed a fully functional and secure user registration pipeline, seamlessly integrating email-based OTP verification (Amazon SES) and cross-platform authentication flows.
* Executed smooth and reliable synchronization of User Profiles between the Amazon Cognito directory and the legacy MongoDB database, ensuring strict data consistency.
* Successfully migrated the foundational Backend API infrastructure to AWS Lambda, harnessing the flexibility and virtually infinite auto-scaling capabilities inherent to Serverless computing.
* Finalized the integration of Amazon API Gateway coupled with JWT Authorizer configurations, establishing a robust security perimeter to meticulously govern all incoming Frontend traffic.
