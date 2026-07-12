---
title: "Worklog Week 10"
date: 2026-07-05
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Week 10 Objectives:

* Migrate the entire static file upload flow (e.g., user avatars, class cover images) from direct backend processing to an S3 Upload Bucket architecture utilizing Presigned URLs to significantly reduce server bandwidth overhead.
* Decouple the computationally expensive Word (.docx) exam import feature into a separate, background-running asynchronous process.
* Develop and configure a dedicated Lambda function (Lambda Import Word Processor) to handle the Word parsing logic, operating on an event-driven mechanism triggered by S3 upload events.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Conduct in-depth research on the architecture and operational mechanism of AWS S3 Presigned URLs.<br>&emsp; + Implement URL generation logic with specific expiration times using Node.js (AWS SDK).<br>&emsp; + Configure secure IAM Roles and Policies allowing the backend to issue valid URLs.<br>&emsp; + Adjust CORS settings on the S3 bucket to permit direct PUT requests from the frontend client. | 22/06/2026 | 22/06/2026 | |
| 4 | - Refactor APIs related to image update operations across the application.<br>&emsp; + Test the user avatar upload flow via Presigned URLs, verifying correct file formatting and integrity.<br>&emsp; + Test the class cover image upload flow, focusing on handling large file sizes efficiently.<br>&emsp; + Implement robust error handling on the frontend for scenarios where the Presigned URL expires or access is denied. | 24/06/2026 | 24/06/2026 | |
| 6 | - Perform comprehensive monitoring and debugging for the Lambda function utilizing AWS CloudWatch.<br>&emsp; + Monitor the execution stream of the Lambda Import Word Processor via CloudWatch Logs.<br>&emsp; + Analyze logs during valid .docx file uploads: verify successful text/image extraction and DB persistence.<br>&emsp; + Analyze logs during invalid file uploads (wrong format, corrupted files): ensure graceful error throwing without causing function crashes. | 26/06/2026 | 26/06/2026 | |

### Week 10 Results:

* All primary upload flows (avatars, class images) are operating smoothly via presigned URLs. Files are systematically stored with the correct S3 prefixes.
* The backend API system is completely relieved from handling intermediary file transfers (multipart/form-data), resulting in substantial CPU and memory savings.
* The Lambda Import Word function is triggered reliably, demonstrating the capability to parse complex .docx structures and extract raw data accurately.
* The Lambda function successfully establishes connections to MongoDB, transforming raw data and persisting multiple-choice/essay questions according to the defined schema.
* Exceptions and runtime errors within the Lambda function are logged in detail to CloudWatch.
