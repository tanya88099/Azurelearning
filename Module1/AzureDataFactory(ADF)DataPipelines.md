**Module 1: Azure Data Factory (ADF) – Data Pipelines**

🧠** Theory:**
ADF is an ETL tool in Azure to orchestrate and automate data workflows from source to destination (SFTP, RDBMS, Blob, etc.).
🛠 **Resume Line:**
"Designed and deployed 15+ data pipelines in Azure Data Factory to automate ingestion from SFTP, RDBMS, SQL Datahub, and Datawarehouse"
✅ **Practical Steps:**
1.	Go to Azure Portal → Create ADF instance.
2.	Author a pipeline using Copy Activity:
o	Source: SFTP or SQL Server (use sample database like AdventureWorks)
o	Sink: Azure Blob or Azure SQL DB
3.	Create Linked Services, Datasets
4.	Trigger pipeline and monitor runs
5.	Explore Data Flow for transformations
🎯 Practice Task: Build 3 pipelines (SFTP→Blob, SQL→Blob, Blob→SQL DB)

**Start from here:** 
✅ **MODULE 1: Automating Data Pipelines with Azure Data Factory (ADF)**
🎯 **Objective:**
Build 3 pipelines that ingest data from:
•	✅ SFTP → Azure Blob Storage
•	✅ SQL Server (on-prem/cloud) → Azure Blob Storage
•	✅ Azure Blob → Azure SQL Database
________________________________________
**🔸 THEORY OVERVIEW**
What is ADF?
Azure Data Factory is a cloud-based ETL and data integration service that lets you:
•	Move data from 90+ sources (on-prem/cloud)
•	Transform data using mapping data flows
•	Schedule and monitor pipelines
Key Concepts:
Concept	Purpose
Linked Service	Connection info to source/destination (like DSN)
Dataset	Metadata of the data you want to move (table/file)
Pipeline	The workflow that contains activities (e.g., copy)
Trigger	A way to schedule a pipeline (manual, scheduled)
________________________________________
**🔸 PRACTICAL SETUP**
🧩 Prerequisites:
1.	✅ Azure Subscription: https://azure.microsoft.com/free/
2.	✅ Azure Storage Account with Blob container
3.	✅ Azure SQL Database (or use local SQL Server with Integration Runtime)
4.	✅ Dummy SFTP server (use free online one: https://www.wftpserver.com/, or local SFTP setup via FileZilla)
🔹 STEP-BY-STEP TASKS
________________________________________
✅ Task 1: SFTP → Blob Storage
1️⃣ Create Azure Data Factory
•	Go to Azure Portal → Search “Data Factory” → Create
•	Region: Same as your storage account
•	Name: ADF-Demo-Tanya
<img width="439" height="352" alt="image" src="https://github.com/user-attachments/assets/027a5d58-b9c4-4fea-a3cc-c76b1f4e5eb9" />
