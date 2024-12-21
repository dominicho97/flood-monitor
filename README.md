# **Flood Monitoring Dashboard**

This project is an end-to-end **Flood Monitoring System** built using **Azure Blob storage**,**Azure Data factory**, **Azure Databricks** and **Power BI** . It integrates data from the [Flood Monitoring API](https://environment.data.gov.uk/flood-monitoring/doc/reference) and provides valuable insights using a **Power BI dashboard**.

---

## **Project Overview**

Flooding can cause severe impacts on infrastructure, communities, and ecosystems. This project aims to provide a real-time flood monitoring solution to track flood alerts, severity levels, and affected areas using a comprehensive data pipeline and AI-driven insights.

### **Key Features**
- **Real-Time Data Pipeline**:
  - Fetches live flood data from the API and stores it in Azure Blob Storage.
- **Data Transformation**:
  - Cleanses and flattens raw JSON data using Azure Databricks.
- **Interactive Visualizations**:
  - Power BI dashboards for visualizing flood alerts, severity trends, and affected regions.

---

## **Technologies Used**

| **Component**          | **Technology**                                                                 |
|-------------------------|-------------------------------------------------------------------------------|
| **Data Ingestion**      | [Flood Monitoring API](https://environment.data.gov.uk/flood-monitoring/doc/reference) |
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

## **Power BI Dashboard**

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

### **Screenshots**
1. **Dashboard Overview**
   ![Dashboard Overview](images/dashboard_overview.png)

2. **Map Visualization**
   ![Map Visualization](images/map_visualization.png)

3. **Severity Trends**
   ![Severity Trends](images/severity_trends.png)




