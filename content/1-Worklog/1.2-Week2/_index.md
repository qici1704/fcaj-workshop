---
title: "Week 2 Worklog"
date: 2026-10-05
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---


### Week 2 Objectives:

* Review Machine Learning fundamentals: Cost Function, Gradient Descent, Cross-Validation, data types, Feature Scaling, and One-Hot Encoding.
* Learn about basic AWS services; practice with EC2, AMI, EBS, and S3.
* Learn about Serverless, AWS Lambda, and AWS Fargate; compare how these services and EC2 apply to different use cases.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Review the uses and meaning of the cost function in machine learning <br> - Review training a model with Gradient Descent                                                                                             | 05/10/2026   | 05/10/2026      |
| 3   | - Learn about AWS and the types of services: <br>&emsp; + Compute <br>&emsp; + Storage <br>&emsp; + Networking <br>&emsp; + Database <br>                                            | 06/10/2026   | 06/10/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Learn about Cross-Validation to make the most of data in machine learning <br> - Process Categorial data & One-Hot Encoding: <br>&emsp; + Nominal & Ordinal Data <br>&emsp; + One-Hot method for Nominal data <br> - Feature Scaling methods: <br>&emsp; + Standardization <br>&emsp; + Min-Max Normalization <br> - **Practice:** <br>&emsp; + Split the dataset into Train/Test/Valid sets <br>&emsp; + Practice Feature Scaling on a dataset <br> &emsp; + Practice using the One-Hot method for Nominal data | 07/10/2026   | 07/10/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - Learn the basics of EC2: <br>&emsp; + Instance types <br>&emsp; + AMI <br>&emsp; + EBS <br>&emsp; + Instance Lifecycle <br> - Ways to remotely SSH into EC2 <br> - Learn about Elastic IP <br> - Learn the basics of S3: <br>&emsp; + Bucket, Object, Key <br>&emsp; + Storage Class <br>&emsp; + Versioning <br>&emsp; + Multipart Upload <br>&emsp; + Access permissions <br> - **Practice:** <br>&emsp; + Create and SSH into an EC2 <br>&emsp; + Attach EBS to an EC2 <br>&emsp; + Configure the environment                 | 08/10/2026   | 08/10/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - Learn the basics of Serverless <br> - Learn about the AWS Lambda service <br> - Learn about the AWS Fargate service <br> - Compare EC2, Lambda, and Fargate in different scenarios <br> - **Practice:** <br>&emsp; + Grant EC2 access to S3 <br>&emsp; + Download data from S3 <br>&emsp; + Upload results to S3 and clean up resources to avoid incurring costs                                                                                         | 09/10/2026   | 09/10/2026      | <https://cloudjourney.awsstudygroup.com/> |


### Week 2 Results:

* Understand what gradient descent means and how gradient descent works in a machine learning model.
  * The concept of Gradient descent
  * The role Gradient descent plays in a machine learning model and its effects on the function's parameters
  * The Gradient descent algorithm
  * What a model trained with Gradient descent looks like internally
  * The relationship between Gradient descent and Learning rate

* Distinguish the data types of each Feature:
  * Nominal
  * Ordinal
  * Ratio
  * Interval

* Understand how to apply Feature Scaling and its methods:
  * When to use Feature Scaling
  * Standardization and its applications
  * Min-Max Normalization and its applications

* Learn how to use One-Hot Encoding on a Nominal dataset so that the model does not receive noise when training.

* Understand the applications of EC2 and the relationship between EC2 and AMI.

* Create an EC2 using the default VPC, including:
  * Instance Type
  * EBS (Elastic Block Store)
  * Key Pair
  * Elastic ID
  * Security Group

* Distinguish between Instance Store and EBS, and when to store data in each.

* Know how to choose the appropriate Instance Type for each task:
  * P or G families: Have NVIDIA GPUs. Mainly used to train Deep Learning models or run heavy models (such as LLMs)
  * R family: A lot of RAM. Used when processing large amounts of data that require loading the entire dataset into memory
  * C family: A lot of CPU. Used to process logic and crawl data at high speed
  * T or M families: Balanced CPU/RAM. Used as a Web Server or to run a regular backend API

* Understand the basics of S3:
  * Know how to choose the right S3 option for the need
  * Understand how the S3 Multipart Upload feature works
  * Know how to customize access permissions for specific objects

* Data should be compressed before uploading to S3 to significantly reduce Request costs (For example: compress 1 million different .png files into one .zip file).

* Understand what Serverless is and when Serverless should be used.

* Know how to apply services such as EC2, Lambda, and Fargate in different scenarios based on:
  * Cost
  * Latency
  * Scaling speed
  * AI training support
  * Startup latency

