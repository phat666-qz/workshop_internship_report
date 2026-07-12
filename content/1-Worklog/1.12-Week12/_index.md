---
title: "Worklog Week 12"
date: 2026-04-17
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

### Week 12 Objectives:

* Deploy the frontend application to the production environment using AWS Amplify Hosting, establishing an automated build and deploy pipeline.
* Set up and link the project's official domain name through AWS Route 53, ensuring professionalism and memorability for end users.
* Synthesize the complete system architecture, problem statements, solutions, and cost estimations into a comprehensive Project Proposal.
* Perform final testing on the entire system before submitting it to the workshop.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Conduct in-depth research on AWS Amplify Hosting and its mechanism for serving Single Page Applications (SPAs).<br>&emsp; + Analyze how Amplify processes build specs and securely manages environment variables.<br>&emsp; + Integrate the source repository (GitHub/GitLab) with Amplify to trigger the CI/CD pipeline.<br>&emsp; + Configure the `amplify.yml` file to define dependencies installation, build, and deployment steps for the React project. | 06/07/2026 | 06/07/2026 | |
| 3 | - Verify and test the manual deployment process directly on the AWS Amplify Hosting platform.<br>&emsp; + Monitor build logs within the console to ensure the static file generation process completes without errors.<br>&emsp; + Set up a Custom Domain on Route 53, directing Alias/CNAME records to the Amplify application URL.<br>&emsp; + Confirm that the official domain `examora.click` is consistently accessible and that the SSL (HTTPS) certificate is automatically provisioned. | 07/07/2026 | 07/07/2026 | |
| 4 | - Review the content for the Proposal.<br>&emsp; + Clearly articulate the real-world problem and the corresponding system features and approach (Problem and Solution).<br>&emsp; + Design and provide detailed descriptions for the System Architecture Diagram using tools like draw.io or Lucidchart.<br>&emsp; + Utilize the AWS Pricing Calculator to generate a highly realistic monthly operational cost estimate breakdown. | 08/07/2026 | 08/07/2026 | |
| 5 | - Review the entire project and content to prepare the workshop report.<br>&emsp; + Review test case scenarios, re-execute core flow tests, and finalize the ultimate testing documentation.<br>&emsp; + Design presentation slides, distilling the key technological highlights (Serverless, SQS, S3 Presigned URLs).<br>&emsp; + Cross-check the Workshop Report content to ensure a professional tone and absolute technical accuracy. | 09/07/2026 | 09/07/2026 | |

### Week 12 Results:

* The web application is successfully hosted on AWS Amplify, featuring fast page load speeds and an automated CI/CD pipeline upon new code commits.
* The system is accessible smoothly via the custom domain `examora.click`, with connections fully secured by standard HTTPS encryption.
* All content, demo scripts, and Workshop Reports have been fully prepared.
