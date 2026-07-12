---
title: "Worklog Week 8"
date: 2026-07-05
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Week 8 Objectives:

* Finalize the seamless interaction architecture between the Frontend application and the Serverless API backend, ensuring both high performance and robust security.
* Master the AWS Shared Responsibility Model to explicitly distinguish security and compliance obligations between the customer and the cloud provider.
* Establish comprehensive visibility and traceability mechanisms by aggregating and analyzing cloud service logs (CloudTrail, CloudWatch).
* Investigate automated resource auditing mechanisms to evaluate configuration compliance across the AWS environment (AWS Config).
* Outline the developmental roadmap and formulate the initial deployment strategy for the real-world Examora project architecture.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Complete Frontend Lab <br> - **Practice:** <br>&emsp; + Integrate Frontend source code (React/Vue) with Amazon API Gateway, meticulously handling HTTP responses and CORS configurations. <br>&emsp; + Embed Cognito-issued JWT Tokens within API request headers to enforce stringent, stateless authentication mechanisms. <br>&emsp; + Manage client-side error states (e.g., 401 Unauthorized, 403 Forbidden) and optimize overall User Experience (UX). | 08/06/2026 | 08/06/2026 | <https://000079.awsstudygroup.com/> |
| 3 | - Learn Security & Monitoring <br> - **Details:** <br>&emsp; + Analyze the AWS Shared Responsibility Model, clarifying data protection and operating system patching duties at the application layer. <br>&emsp; + Explore Amazon CloudTrail to continuously monitor, log, and retain account activity related to API calls across the AWS infrastructure. <br>&emsp; + Construct security auditing scenarios utilizing CloudTrail logs to detect anomalous behaviors and mitigate potential internal threats. | 09/06/2026 | 09/06/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 4 | - Learn CloudWatch <br> - **Details:** <br>&emsp; + Set up centralized observability using CloudWatch Metrics to aggregate performance indicators for EC2, Lambda, and DynamoDB. <br>&emsp; + Configure CloudWatch Alarms to trigger automated notifications (via SNS) when resource utilization breaches predefined thresholds. <br>&emsp; + Ingest, store, and analyze system logs leveraging CloudWatch Logs, employing Log Insights for real-time diagnostic queries. | 10/06/2026 | 10/06/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 5 | - Learn AWS Config <br> - **Details:** <br>&emsp; + Initialize AWS Config to record the historical configurations of active AWS resources deployed within the ecosystem. <br>&emsp; + Assess infrastructure compliance continuously by deploying AWS Config Rules (Managed Rules) against organizational policies. <br>&emsp; + Analyze automated remediation workflows designed to rectify non-compliant resources swiftly and autonomously. | 11/06/2026 | 11/06/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 6 | - Project planning <br> - **Details:** <br>&emsp; + Synthesize acquired Serverless and Security proficiencies to architect a high-level technical blueprint for the Examora project. <br>&emsp; + Define the Minimum Viable Product (MVP) scope, cataloging the core AWS services designated for the initial launch phase. <br>&emsp; + Develop a detailed Work Breakdown Structure (WBS) and roadmap to allocate resources and schedule tasks for upcoming weeks. | 12/06/2026 | 12/06/2026 | |

### Week 8 Results:

* Engineered a reliable communication pipeline between the Frontend and Serverless Backend, accurately integrating the Cognito authentication flow.
* Successfully deploying automated system error alert workflows utilizing CloudWatch and SNS.
* Achieved the capability to trace and audit infrastructure configuration histories via CloudTrail and AWS Config, ensuring sustained compliance.
* The Examora project implementation plan has been finalized.
