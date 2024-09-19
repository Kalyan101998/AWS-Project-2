<h1 align="center">AWS Project 2</h1>


# Project Description: Data Protection, Governance, and Monitoring
* This project involves setting up a comprehensive data analytics platform using AWS services to manage the City of Vancouver’s animal control data. 
## Project Title: AWS Data Analytic Platform for the City of Vancouver - Part 2
* This project aims to design and implement a Data Analytics Platform (DAP) using Amazon Web Services (AWS) to Data Protection, Governance, and Monitoring
## Project Objective:
* Designing & Implementing DAP.
## Methodology:
* The process of providing Data Protection, Governance, and Monitoring for DAP designed as follows.
### 1. Data Protection
- To secure the data, multiple AWS services were used:
  - **S3 Bucket Policies**: Restricted access to the data to authorized users only.
  - **AWS KMS (Key Management Service)**: Enabled encryption using a symmetric key created through AWS KMS, ensuring all data stored in S3 buckets was encrypted.
  - **Data Replication**: Established backup procedures to replicate data across AWS regions, preventing data loss and ensuring disaster recovery
 ![image](https://github.com/user-attachments/assets/e49efe9a-7758-422c-969f-7b38e11e7fc8)
![image](https://github.com/user-attachments/assets/5bac0387-47a8-41ea-a63b-f82b65df2bea)
![image](https://github.com/user-attachments/assets/5b6d4b52-f84a-4280-ba46-e9ba173893fe)

### 2. Data Governance
- To enhance data governance and secure data access, I set up a data pipeline using AWS Glue and S3. The pipeline begins with storing data in an S3 bucket and includes steps to detect sensitive information, such as personal data. It then evaluates the data quality to ensure integrity. A row-level transformation is applied to modify the data, followed by a conditional router that filters the data based on defined criteria. Unnecessary columns are removed by changing the schema, ensuring that only essential information is retained. 
![image](https://github.com/user-attachments/assets/6bce9758-bad3-401f-93e7-51940f268a2c)
![image](https://github.com/user-attachments/assets/addc8763-4371-43fa-b61c-8bcf62bca1a6)


### 3. Data Monitoring
- Monitoring data effectively is crucial for ensuring system health and keeping track of usage metrics. The screenshots show the use of Amazon CloudWatch to create custom dashboards, which aid in tracking and managing system performance.
 ![image](https://github.com/user-attachments/assets/990d846f-b05e-4520-a026-8245fda714eb)

- The CloudWatch dashboard, named "part2-parksrecreandpets-animalconinv-kalyan," includes:
* Estimated Charges: Displays a gauge indicating the current estimated costs.
* Number of Objects: Shows a graph tracking the count of objects over time.
* Bucket Size in Bytes: Illustrates the size of the bucket in bytes, providing insights into storage usage.
* Alam: An alarm named "animalcoinv-Alam-kalyan" is configured to monitor specific thresholds, such as the number of objects or estimated charges. When these thresholds are exceeded, an email alert is triggered, ensuring proactive monitoring.

![image](https://github.com/user-attachments/assets/59aacaee-a8e7-4820-9ba7-28de79c4cca9)

- AWS Glue job monitoring is depicted, summarizing job runs with details such as:
* Total Runs: Three jobs executed, with two successful and one failed.
* Run Success Rate: 67% success rate.
* Resource Usage: Visual representation of resource utilization over time.
- Lastly, the CloudTrail screenshot shows a trail named "part2-animalconinv-trail-kalyan" configured in the US East (N. Virginia) region, with logging enabled to track user activity and API usage.
![image](https://github.com/user-attachments/assets/02133a49-c1fb-4ddc-ae47-388c70f3e977)


## AWS CloudTrail
The CloudTrail configuration includes a trail named "part2-animalconinv-trail-kalyan" in the US East (N. Virginia) region. Logging is enabled, capturing user activity and API usage for enhanced security and compliance.


