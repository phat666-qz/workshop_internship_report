---
title: "Worklog Week 11"
date: 2026-04-17
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Objectives:
* Decouple grading logic from the exam submission request using SQS Grading Queue and Lambda Grading Worker.

### Tasks to implement this week:
| Day | Task | Start Date | End Date | References |
| --- | ---- | ---------- | -------- | ---------- |
| Monday | - Design asynchronous architecture using AWS SQS for the exam submission feature. | 29/06/2026 | 29/06/2026 |  |
| Tuesday | - Deploy AWS SQS Grading Queue and modify the submission API to push messages into the Queue. | 30/06/2026 | 30/06/2026 |  |
| Thursday | - Directly test SQS message -> Lambda Grading Worker -> MongoDB result using sample payloads. | 02/07/2026 | 02/07/2026 |  |
| Friday | - Log errors and troubleshooting steps when the worker lacks the Mongoose model or fails to update grading status. | 03/07/2026 | 03/07/2026 |  |

### Achievements:
* Successfully decoupled the grading logic, reducing load on the primary API.
* The backend saves the submission with an 'in-progress' status, sends the job to SQS, and the worker processes the grading/updates the result in MongoDB.
