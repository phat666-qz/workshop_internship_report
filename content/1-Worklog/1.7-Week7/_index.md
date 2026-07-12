---
title: "Worklog Week 7"
date: 2026-07-05
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Week 7 Objectives:

* Learn about NoSQL database architecture, focusing on the scalability and query performance of Amazon DynamoDB.
* Analyze non-relational data modeling patterns (Partition keys, Sort keys, Global Secondary Indexes) to optimize storage and retrieval operations.
* Build a solid foundation in identity management and application authentication within a cloud environment.
* Evaluate and design a comprehensive authorization solution for AWS resources utilizing role-based access controls.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Introduction to NoSQL Database <br> - **Details:** <br>&emsp; + Analyze the architectural characteristics of Amazon DynamoDB compared to traditional RDBMS systems. <br>&emsp; + Evaluate data routing strategies, partitioning mechanisms, and their impact on read/write performance. <br>&emsp; + Research concepts regarding Read/Write Capacity Units (RCU/WCU) and On-Demand billing models. | 01/06/2026 | 01/06/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 3 | - Complete NoSQL Database Lab <br> - **Practice:** <br>&emsp; + Provision and configure basic DynamoDB tables, establishing Partition and Sort Keys tailored to specific access patterns. <br>&emsp; + Execute data ingestion, updates, and queries (Query vs. Scan) utilizing both the AWS Management Console and AWS CLI. <br>&emsp; + Profile and optimize query costs by applying Filter Expressions to narrow down scan ranges efficiently. | 02/06/2026 | 02/06/2026 | <https://000060.awsstudygroup.com/> |
| 4 | - Introduction to User Authentication <br> - **Details:** <br>&emsp; + Distinctly differentiate between Authentication (AuthN) and Authorization (AuthZ) in the context of application security. <br>&emsp; + Explore the dual architecture of Amazon Cognito: User Pools (user directory management) and Identity Pools (credential provisioning). <br>&emsp; + Study the token issuance lifecycle (Access Tokens, ID Tokens) in adherence to OAuth2.0 and OIDC standards. | 03/06/2026 | 03/06/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 5 | - Complete User Authentication Lab (Part 1) <br> - **Practice:** <br>&emsp; + Design and deploy a Cognito User Pool, implementing robust password policies and Multi-Factor Authentication (MFA). <br>&emsp; + Implement end-to-end user registration, email/phone verification, and sign-in workflows using the Cognito Hosted UI. <br>&emsp; + Customize user attributes and schema mappings to securely store personalized application data. | 04/06/2026 | 04/06/2026 | <https://000081.awsstudygroup.com/> |
| 6 | - Complete User Authentication Lab (Part 2) <br> - **Practice:** <br>&emsp; + Configure a Cognito Identity Pool to federate user identities with IAM Roles, granting precise AWS resource access. <br>&emsp; + Integrate authorization layers, enabling authenticated users to safely invoke backend APIs and retrieve S3 objects. <br>&emsp; + Perform security testing on token workflows and simulate access denial scenarios based on predefined IAM policies. | 05/06/2026 | 05/06/2026 | <https://000081.awsstudygroup.com/> |

### Week 7 Results:

* Successfully designing DynamoDB tables that deliver low latency.
* Implemented a comprehensive identity management solution via Amazon Cognito User Pools, supporting seamless onboarding and authentication flows.
* Successfully integrated Cognito Identity Pools with AWS IAM, securely delegating fine-grained access to AWS resources based on the principle of least privilege.
* Established a robust conceptual and practical framework for deploying JWT-based authentication in Serverless applications for subsequent project phases.
