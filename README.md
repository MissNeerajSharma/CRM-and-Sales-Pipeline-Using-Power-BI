## End-to-End CRM and Sales Analytics Project: On-Premise to Azure Cloud with Power BI Dashboard
# Project Overview
This project showcases an end-to-end solution for CRM and Sales Analytics, leveraging Azure Cloud services and Power BI. The objective was to migrate on-premise data to Azure, transform and load it into Azure Synapse Analytics, create clusters using Databricks for data processing, and develop insightful Power BI dashboards for data visualization and decision-making. Finally, schedules and alerts were managed to ensure timely data updates and notifications.

## Step-by-Step Process
1. Data Migration from On-Premise to Azure Cloud
Objective: Migrate CRM and Sales data from on-premise SQL Server to Azure SQL Database for scalable and efficient data storage.

# Steps:
Assessment and Planning:

# Assess the existing on-premise database structure and data volume.
Plan the migration strategy, including downtime requirements and data synchronization methods.
Azure SQL Database Setup:

# Create an Azure SQL Database instance on the Azure portal.
Configure firewall settings to allow connections from the on-premise environment.

# Data Migration:
Use the Data Migration Assistant (DMA) to assess database compatibility.
Employ the Azure Database Migration Service (DMS) to transfer the data from on-premise SQL Server to Azure SQL Database.
Verification:

# Verify data integrity and completeness post-migration.
2. Data Processing with Azure Databricks
Objective: Process and transform the migrated data using Azure Databricks to prepare it for analytical workloads.

# Steps:
Databricks Cluster Setup:

# Create an Azure Databricks workspace.
Set up a cluster with appropriate configurations (e.g., number of nodes, instance types).
Data Ingestion:

# Connect to Azure SQL Database from Databricks.
Ingest data into Databricks using Spark SQL.
Data Transformation:

Perform necessary data transformations using PySpark or SQL in Databricks notebooks.
Cleanse, aggregate, and prepare the data for analysis.
Storage in Delta Lake:

Store the processed data in Delta Lake for efficient querying and analytics.
3. Loading Data into Azure Synapse Analytics
Objective: Load the transformed data into Azure Synapse Analytics for advanced analytics and reporting.

Steps:
Azure Synapse Analytics Setup:

# Create an Azure Synapse workspace.
Set up a dedicated SQL pool (formerly SQL Data Warehouse) for data storage.
Data Loading:

Use Azure Data Factory (ADF) to orchestrate the data movement from Delta Lake in Databricks to Synapse.
Create pipelines in ADF to load data into Synapse, ensuring scheduling and dependency management.
Verification:

Verify data integrity and completeness in Synapse Analytics.
# 4. Power BI Dashboard Development
Objective: Develop interactive dashboards in Power BI for CRM and Sales Analytics, using data from Azure Synapse Analytics.

Steps:
Power BI Setup:

Install and configure Power BI Desktop.
Connect Power BI to Azure Synapse Analytics.
Data Modeling:

Create a data model in Power BI, establishing relationships between tables.
Define calculated columns and measures using DAX for advanced analytics.
Dashboard Design:

Design and develop interactive visuals and dashboards to provide insights into CRM and Sales data.
Utilize charts, graphs, and other visual elements to represent key metrics and KPIs.
Publishing and Sharing:

Publish the Power BI reports to Power BI Service.
Share dashboards with stakeholders and set up access permissions.

# 5. Scheduling and Alerts Management
Objective: Manage data refresh schedules and set up alerts to ensure timely updates and notifications.

Steps:
Data Refresh Scheduling:

Configure data refresh schedules in Power BI Service to ensure dashboards are up-to-date.
Set up incremental data refresh for efficiency.
Alerts Setup:

Define data-driven alerts in Power BI to notify stakeholders of critical changes or thresholds.
Use Power Automate to create workflows for automated notifications and actions.
Monitoring and Maintenance:

Monitor data refresh activities and resolve any issues promptly.
Maintain and update dashboards as required to reflect changing business needs.

![](https://github.com/MissNeerajSharma/CRM-and-Sales-Pipeline-Using-Power-BI/blob/main/Screenshot%202024-07-21%20171810.png)
![](https://github.com/MissNeerajSharma/CRM-and-Sales-Pipeline-Using-Power-BI/blob/main/Screenshot%202024-07-21%20171831.png)

# Key Features
Analyze Key Sales Metrics: Evaluate gross leads, deal values, and conversion rates to understand overall sales performance.
Assess Sales Performance: Measure the number of customers, deals won, and deal conversion rates to identify strengths and areas for improvement.
# Visualize Global Reach: 
Use an interactive map to pinpoint sales performance across various countries, facilitating targeted sales strategies.
Monitor Sales Pipeline Health: Track the status of leads at different stages to optimize the sales process.
Highlight Top Sales Agents: Recognize top performers and their contributions to motivate and set benchmarks for the sales team.
Forecast Future Success: Project potential sales and lead values for the upcoming months to ensure proactive planning and strategy adjustments.
# Data and Metrics
Key Metrics
Gross Leads: 3,000
Gross Deal Value: $8.28M
Lead Conversion Rate: 28.90%
Valid Leads: 744
Valid Deal Value: $2.1M
Sales Performance
Customers in System: 867
Deals Won: 83
Deal Conversion Rate: 9.57%
Average Gross Deal Value: $2.76K
Sales Pipeline Health
Initial Contact: 298 leads
Nurturing: 220 leads
Proposal Sent: 140 leads
Won: 83 deals
Opened: 65 deals
Lost: 61 deals
Top Sales Agents
Laura Thompson: 749 leads, 21 deals won, $48,693 deal value
Sarah Davis: 249 leads, 8 deals won, $34,873 deal value
Michael Brown: 483 leads, 13 deals won, $25,903 deal value
Forecasting Future Success
With $1.38M in new leads expected in the next three months, the data-driven approach ensures the team stays ahead of the curve.

## Tools and Technologies
Power BI: For data visualization and dashboard creation.
CRM System: To collect and manage sales data.
SQL: For data extraction and transformation.
Azure: For data storage and processing.
