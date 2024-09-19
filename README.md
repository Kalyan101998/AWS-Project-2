<h1 align="center">AWS Project 2</h1>


# Project Description: Data Protection, Governance, and Monitoring
* The City of Vancouver requires a robust and efficient data platform to manage and analyze safety-issued operating permits for water systems, including cooling towers, water features, and other public systems.

## Project Title: AWS Data Analytic Platform for the City of Vancouver - Part 2
* This project aims to design and implement a Data Analytics Platform (DAP) using Amazon Web Services (AWS) to store, process, and analyze water system permits to ensure public health standards are met and to streamline responses to any identified issues.
## Project Objective:
* Designing & Implementing DAP.
## Methodology:
* The process of providing Data Protection, Governance, and Monitoring for DAP designed as follows.
### 1. Data Protection
- To secure the data, multiple AWS services were used:
  - **S3 Bucket Policies**: Restricted access to the data to authorized users only.
  - **AWS KMS (Key Management Service)**: Encryption was enabled using a symmetric key created through AWS KMS to ensure all data stored in the S3 buckets was encrypted.
  - **Data Replication**: Backup procedures were put in place to replicate data across AWS regions to prevent data loss and ensure disaster recovery.
  ![image](https://github.com/user-attachments/assets/adc2dab1-f4d2-49b9-bf2b-dd5057a7ea83)
### 2. Data Governance
- AWS CloudTrail was employed to track all API calls, changes, and events in the AWS environment.
- This provided full transparency and traceability for any modifications made to the data or system configurations. 
![image](https://github.com/user-attachments/assets/d596b711-6e10-4db8-baab-9eb1e96da184)
![image](https://github.com/user-attachments/assets/0e5b7c79-c800-471a-b3cc-28c76620d94e)
![image](https://github.com/user-attachments/assets/68b25121-9d78-4c8f-a926-af8550b1003b)
![image](https://github.com/user-attachments/assets/6c99d3ff-f0d0-4cd7-b696-d433992f8f5c)
### 3. Data Monitoring
- AWS CloudWatch was used to monitor system performance, track resource usage, and set alarms for predefined thresholds. Custom dashboards displayed metrics such as:
  - **Estimated Charges**: Monitoring costs associated with data storage and processing.
  - **Bucket Size (in Bytes)**: Tracking the growth of the data stored in the S3 buckets over time.
  ![image](https://github.com/user-attachments/assets/db2e5517-f2c0-406a-882b-bd4560242e39)
  ![image](https://github.com/user-attachments/assets/d5d8364d-f4f9-48b1-a33b-df459f4bbc95)
- Screenshots and Visuals
  - **S3 Bucket Management and Encryption**: Demonstrates the security configurations, including encryption and replication rules.
  - **CloudTrail Logging**: Captures user actions and API requests to ensure full governance and compliance.
  - **CloudWatch Dashboard**: Highlights system health, storage costs, and monitoring details.
  ![image](https://github.com/user-attachments/assets/e3bde002-8dbf-434e-96bd-17f93438fcaf)
  ![image](https://github.com/user-attachments/assets/67f6f996-f65a-4c57-8dc2-007e083a2933)

