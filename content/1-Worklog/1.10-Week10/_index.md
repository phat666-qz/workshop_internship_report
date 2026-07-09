---
title: "Worklog Week 10"
date: 2026-04-17
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Objectives:
* Migrate the file upload flow to S3 Upload Bucket using presigned URLs and separate the Word import feature into an asynchronous Lambda function.

### Tasks to implement this week:
| Day | Task | Start Date | End Date | References |
| --- | ---- | ---------- | -------- | ---------- |
| Monday | - Learn how to generate and use Presigned URLs on AWS S3, configure corresponding IAM roles. | 22/06/2026 | 22/06/2026 |  |
| Wednesday | - Test avatar and class image uploads after the frontend switched to using presigned URLs. | 24/06/2026 | 24/06/2026 |  |
| Friday | - Check CloudWatch Logs of the Lambda Import Word Processor when valid and invalid .docx files are uploaded. | 26/06/2026 | 26/06/2026 |  |

### Achievements:
* Presigned URLs work correctly for main upload flows; files are saved with the correct S3 prefixes.
* Lambda Import Word can successfully parse .docx files and save questions into MongoDB.
