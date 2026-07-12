---
title: "Worklog Week 6"
date: 2026-07-05
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Week 6 Objectives:

* Learn about serverless architecture and its operational and cost benefits.
* Understand AWS Lambda services, mastering how to write, package, and deploy functions.
* Understand routing mechanisms and API management using Amazon API Gateway as the primary communication entry point.
* Architect and deploy a robust serverless Backend, orchestrating smooth integrations across S3, API Gateway, Lambda, and DynamoDB.
* Design and implement secure, scalable RESTful API standards catering to modern distributed applications.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Research Serverless architecture foundations on AWS <br>&emsp; + Analyze definitions, advantages, and practical real-world use-cases of Serverless <br>&emsp; + Explore the AWS Lambda service: Event sources and Execution environments <br>&emsp; + Examine Amazon API Gateway and its integration patterns with Lambda | 25/05/2026 | 25/05/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 3 | - **Lab:** Deploying a Serverless Backend (Part 1: Data Structures and Processing) <br>&emsp; + Design and initialize a NoSQL data table using Amazon DynamoDB <br>&emsp; + Write Lambda function source code (Python/Node.js) to interact with DynamoDB <br>&emsp; + Configure secure IAM Roles to grant necessary execution permissions to Lambda | 26/05/2026 | 26/05/2026 | <https://000078.awsstudygroup.com/> |
| 4 | - **Lab:** Deploying a Serverless Backend (Part 2: Event Integration) <br>&emsp; + Configure S3 Event Notifications to act as automatic Lambda triggers <br>&emsp; + Test the continuous data flow: S3 Upload -> Lambda Execution -> DynamoDB logging <br>&emsp; + Monitor and analyze system logs leveraging the Amazon CloudWatch service | 27/05/2026 | 27/05/2026 | <https://000078.awsstudygroup.com/> |
| 5 | - Understand REST API design and advanced API Gateway configurations <br>&emsp; + Review standard RESTful API design principles (Methods: GET, POST, PUT, DELETE) <br>&emsp; + Survey Resource, Method, and Integration Request setups within API Gateway <br>&emsp; + Learn about CORS (Cross-Origin Resource Sharing) mechanisms and API authorization | 28/05/2026 | 28/05/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 6 | - **Lab:** Building Comprehensive Serverless APIs <br>&emsp; + Initialize a new REST API on API Gateway and define the underlying resource structure <br>&emsp; + Map specific API endpoints (GET/POST) to their respective backend Lambda functions <br>&emsp; + Deploy the API to a Stage and perform rigorous testing using Postman/cURL | 29/05/2026 | 29/05/2026 | <https://000066.awsstudygroup.com/> |

### Week 6 Results:

* Attained comprehensive understanding of the modern request processing flow: Client -> API Gateway -> AWS Lambda -> Database.
* Successfully deployed a practical Serverless Backend, flawlessly combining the S3, Lambda, and DynamoDB service ecosystem.
* Acquired the capability to independently design and publish a secure, highly available RESTful API via API Gateway.
* Mastered configuring specialized IAM Roles (Principle of Least Privilege) for individual Lambda functions to ensure robust security.
* Proficiently utilized CloudWatch for continuous monitoring, log analysis, and troubleshooting within a distributed serverless environment.
