---
title: "Worklog Week 5"
date: 2026-07-05
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Week 5 Objectives:

* Learn about cloud computing platforms with Amazon EC2 virtual servers and related concepts such as AMI, Security Groups, and Key Pairs.
* Learn about managed relational databases (Amazon RDS) and data backup and recovery strategies.
* Research the Auto Scaling mechanism to dynamically scale system capacity based on real-time application traffic.
* Grasp the operating principles of Elastic Load Balancing (ELB) to distribute traffic and ensure High Availability.
* Practice deploying a fundamental application architecture integrating EC2 (Compute) and RDS (Database) based on AWS best practices.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Research on the Amazon EC2 platform <br>&emsp; + Classify and select appropriate Instance Types tailored for specific workloads <br>&emsp; + Explore the Amazon Machine Image (AMI) concept and initialization process <br>&emsp; + Understand the EC2 Lifecycle and evaluate various purchasing options | 18/05/2026 | 18/05/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 3 | - Investigate Amazon Relational Database Service (RDS) <br>&emsp; + Analyze Multi-AZ deployment architectures to ensure Disaster Recovery <br>&emsp; + Examine the Read Replica mechanism to alleviate read query loads on primary DBs <br>&emsp; + Evaluate supported database engines within RDS (MySQL, PostgreSQL, Aurora) | 19/05/2026 | 19/05/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 4 | - Study Elastic Load Balancing and Auto Scaling mechanisms <br>&emsp; + Analyze traffic distribution algorithms of the Application Load Balancer (ALB) <br>&emsp; + Configure Launch Templates and Auto Scaling Groups (ASG) <br>&emsp; + Formulate automated scale-out and scale-in strategies using CloudWatch metrics | 20/05/2026 | 20/05/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 5 | - **Lab:** Compute Essentials Practice with Amazon EC2 <br>&emsp; + Deploy a Linux EC2 virtual server, configure Security Groups, and establish SSH <br>&emsp; + Install a web server (Apache/Nginx) automatically via User Data scripts <br>&emsp; + Monitor resources and test instance state changes (Stop/Terminate operations) | 21/05/2026 | 21/05/2026 | <https://000004.awsstudygroup.com/> |
| 6 | - **Lab:** Database Essentials Practice with Amazon RDS <br>&emsp; + Provision a MySQL-based RDS instance securely within a Private Subnet <br>&emsp; + Configure Security Groups to allow secure EC2 to RDS connectivity <br>&emsp; + Execute essential administrative tasks: Automated Backups and Manual Snapshots | 22/05/2026 | 22/05/2026 | <https://000005.awsstudygroup.com/> |

### Week 5 Results:

* Mastered the provisioning, configuration, and lifecycle management of EC2 instances on the AWS platform.
* Successfully deployed Amazon RDS services, demonstrating a clear understanding of network and security configurations to protect databases.
* Deepened knowledge of High Availability system design paradigms by seamlessly combining ELB with Auto Scaling.
* Gained proficiency in utilizing User Data scripts to automate the bootstrapping process of web services on EC2 instances.
