# **Flood Monitoring Dashboard**

This project is an end-to-end **Flood Monitoring System** built using **Azure Blob storage**,**Azure Data factory**, **Azure Databricks** and **Power BI** . It integrates data from the [Flood Monitoring API](https://environment.data.gov.uk/flood-monitoring/doc/reference) and provides valuable insights using a **Power BI dashboard**.

---

## **Project Overview**

Flooding can cause severe impacts on infrastructure, communities, and ecosystems. This project aims to provide a real-time flood monitoring solution to track flood alerts, severity levels, and affected areas using a comprehensive data pipeline and AI-driven insights.

 ![flood_dashboard2](https://github.com/user-attachments/assets/76a55b62-b041-46d3-9f36-d9a2d478f128)

### **Key Features**
- **Data Pipeline**:
  - Fetches live flood data from the API using Azure Data Factory and stores it in Azure Blob Storage.
- **Data Transformation**:
  - Cleanses and flattens raw JSON data using Azure Databricks.
- **Automation**:
  - Azure Data Factory automates the data pipeline for regular updates.
    
- **Interactive Visualizations**:
  - Power BI dashboards for visualizing flood alerts, severity trends, and affected regions.

---
## **Technologies Used**

| **Component**          | **Technology**                                                                 |
|-------------------------|-------------------------------------------------------------------------------|
| **Data Ingestion**      | Azure Data Factory                                                           |
| **Data Storage**        | Azure Blob Storage                                                           |
| **Data Transformation** | Azure Databricks                                                             |
| **Data Orchestration**  | Azure Data Factory                                                           |
| **Visualization**       | Power BI                                                                     |


---

## **Architecture Diagram**

![Architecture Diagram](images/flood_monitor_architecture.png)

1. Real-time data ingestion from the Flood Monitoring API.
2. Raw JSON stored in Azure Blob Storage (Raw Container).
3. Data cleansing and flattening using Databricks.
4. Transformed data stored in Azure Blob Storage (Processed Container).
5. Power BI dashboard connected to processed data for insights.

---


1. **Dashboard Overview**
  ![flood_dashboard2](https://github.com/user-attachments/assets/76a55b62-b041-46d3-9f36-d9a2d478f128)


3. **Services overview (azure resource group**
   ![flood_rg](https://github.com/user-attachments/assets/ef690172-0cac-4158-af8b-f3bb8d9a8ce6)


4. **Blob storage, data transformation, ADF pipeline**
   ![blob](https://github.com/user-attachments/assets/d95279e4-a511-4000-afe6-1640e68fa1f5)
***data transforations (databricks)***
   ![databricks_code3](https://github.com/user-attachments/assets/b9cf2639-7a12-44c1-b831-6c494bd971ff)
***ADF pipeline***
  ![pipeline_1](https://github.com/user-attachments/assets/46d76648-f800-4e0f-b824-0855486b3e1c)
6. ## **Power BI Dashboard**

### **Visualizations**
- **Interactive Map (flood location focus)**:
  - Displays flood-affected regions with severity levels.
  - 
- **Interactive Map (severity level focus )**:
  - Displays flood-affected regions with severity levels.

- **Severity Breakdown**:
  - Bar chart showing the distribution of severity levels per by flood-affected region .
  - 
- **Key Metrics**:
  - Total alerts, most affected regions, and recent severity changes.
  ![powerbi_renamed](https://github.com/user-attachments/assets/104ba17f-55f5-4639-97e5-51684b748417)









