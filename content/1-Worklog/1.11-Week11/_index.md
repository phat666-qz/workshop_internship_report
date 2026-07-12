---
title: "Worklog Week 11"
date: 2026-07-05
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Week 11 Objectives:

* Completely decouple the complex grading logic from the user's exam submission request, allowing the primary API to solely handle submission acknowledgement.
* Utilize AWS SQS (Simple Queue Service) to construct a Grading Queue, acting as a highly reliable buffer to hold incoming grading requests during traffic spikes.
* Develop a dedicated Lambda Grading Worker designed to consume messages from the SQS queue and execute grading algorithms completely independently.
* Implement dynamic submission state management within MongoDB to provide users with real-time grading progress.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Research and design the Asynchronous Architecture for the exam submission system.<br>&emsp; + Evaluate the pros and cons of AWS SQS against alternative queueing solutions for this specific workload.<br>&emsp; + Draft the comprehensive data flow diagram: Client -> API Gateway -> Backend -> SQS -> Lambda -> MongoDB.<br>&emsp; + Define and standardize the payload structure for messages dispatched to the SQS queue. | 29/06/2026 | 29/06/2026 | |
| 3 | - Provision and configure the AWS SQS Grading Queue infrastructure on the cloud environment.<br>&emsp; + Tune critical parameters such as Visibility Timeout and Message Retention Period to align with the Lambda execution window.<br>&emsp; + Refactor the Submit Exam API: Register the submission in the database with an "In-progress" status initially.<br>&emsp; + Implement the backend logic to package submission details and seamlessly push the message to the SQS Queue. | 30/06/2026 | 30/06/2026 | |
| 4 | - Develop and program the Lambda Grading Worker responsible for the core grading computations.<br>&emsp; + Integrate the SQS trigger for the Lambda function, configuring an optimal batch size for cost efficiency.<br>&emsp; + Write the core logic to compare candidate responses against standard answer keys and calculate the final score.<br>&emsp; + Initialize a secure connection to MongoDB from within the Lambda environment and execute the document update for the exam result. | 01/07/2026 | 01/07/2026 | |
| 5 | - Conduct comprehensive End-to-End Testing for the automated grading pipeline.<br>&emsp; + Utilize the AWS Management Console or AWS CLI to inject raw SQS messages utilizing simulated payload templates.<br>&emsp; + Monitor the lifecycle: Lambda Grading Worker invocation, message processing, and comprehensive log generation.<br>&emsp; + Rigorously verify the accuracy of the computed scores and the corresponding status transitions within the MongoDB database. | 02/07/2026 | 02/07/2026 | |
| 6 | - Optimizing the error handling process in Worker.<br>&emsp; + Completely resolve the Mongoose model initialization error occurring within the serverless execution context.<br>&emsp; + Implement robust error catching logic for scenarios where grading fails, guaranteeing a fallback status update to "Grading Error".<br>&emsp; + Persist all detailed error stack traces directly to CloudWatch for comprehensive forensic analysis and debugging. | 03/07/2026 | 03/07/2026 | |

### Week 11 Results:

* The backend system is smoothly integrated with AWS SQS. Every submitted exam is encoded into a message and securely buffered awaiting processing, eliminating data loss risks.
* The Lambda Grading Worker operates consistently, automatically pulling messages from the queue, comparing answers, and calculating final scores with absolute precision.
* The system comprehensively tracks the lifecycle of a submission, seamlessly transitioning from 'In-progress' to 'Completed' or 'Error', updating in real-time within MongoDB.
* Environmental issues, such as missing Mongoose model contexts in serverless environments, have been definitively fixed, ensuring the Worker function never crashes unexpectedly.
