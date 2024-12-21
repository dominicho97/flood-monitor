# **Flood Monitoring Dashboard**

This project is an end-to-end **Flood Monitoring System** built using **Azure Blob Storage**, **Azure Data Factory**, **Azure Databricks**, and **Power BI**. It integrates data from the [Flood Monitoring API](https://environment.data.gov.uk/flood-monitoring/doc/reference) and provides actionable insights through an interactive **Power BI dashboard**.

![flood_dashboard1](https://github.com/user-attachments/assets/d2ed40e3-922d-43d4-9c2a-815bdf3ed05d)


![flood_dashboard](https://github.com/user-attachments/assets/b8bb8aa2-a467-43ce-af49-5a9c48496b49)

---

## **Overview**

Flooding can significantly impact infrastructure, communities, and ecosystems. This project aims to provide a real-time flood monitoring solution to:
- **Track flood alerts**.
- Analyze **severity levels**.
- Identify **affected areas**.
- Enable data-driven decisions using a scalable and automated Azure data pipeline.

## **Dashboard**
![Flood Monitoring Dashboard](https://github.com/user-attachments/assets/76a55b62-b041-46d3-9f36-d9a2d478f128)

---

## **Key Features**

- **Automated Data Pipeline**:
  - Fetches live flood data using **Azure Data Factory**.
  - Stores raw data in **Azure Blob Storage**.
- **Data Transformation**:
  - Processes and flattens raw JSON using **Azure Databricks**.
- **Interactive Visualization**:
  - Visualizes flood alerts, trends, and regions via **Power BI**.
- **Real-Time Insights**:
  - Updates automatically with new data for timely decision-making.

---

## **Technologies Used**

| **Component**          | **Technology**                                                                |
|-------------------------|-------------------------------------------------------------------------------|
| **Data Ingestion**      | Azure Data Factory                                                           |
| **Data Storage**        | Azure Blob Storage                                                           |
| **Data Transformation** | Azure Databricks                                                             |
| **Data Orchestration**  | Azure Data Factory                                                           |
| **Visualization**       | Power BI                                                                     |

---

## **Architecture**

### **High-Level Data Flow**
1. Data ingestion from the Flood Monitoring API using **Azure Data Factory**.
2. Raw JSON data stored in **Azure Blob Storage** (Raw Container).
3. Data transformed and flattened via **Azure Databricks**.
4. Processed data stored in **Azure Blob Storage** (Processed Container).
5. Insights visualized through **Power BI Dashboards**.

![Architecture Diagram](images/flood_monitor_architecture.png)

---

## **Project Components**

### **1. Services Overview**
   A centralized Azure Resource Group containing:
   ![Services Overview](https://github.com/user-attachments/assets/ef690172-0cac-4158-af8b-f3bb8d9a8ce6)

---

### **2. Blob Storage and Data Transformation**
   - **Blob Storage**: Stores raw and processed data.
   - **Databricks**: Performs data cleansing and flattening.
   ![Blob and Transformation](https://github.com/user-attachments/assets/d95279e4-a511-4000-afe6-1640e68fa1f5)

---

### **3. Databricks Transformations**
   - Custom logic for transforming JSON data into a tabular format for analysis.
   ![Databricks Code](https://github.com/user-attachments/assets/b9cf2639-7a12-44c1-b831-6c494bd971ff)

---

### **4. Azure Data Factory Pipeline**
   - Automates the end-to-end data flow:
     - Fetches data from the API.
     - Loads raw data into Blob Storage.
     - Triggers Databricks notebooks for data transformation.
     - Outputs processed data to Blob Storage.
   ![ADF Pipeline](https://github.com/user-attachments/assets/46d76648-f800-4e0f-b824-0855486b3e1c)

---

### **5. Power BI Dashboard**

#### **Visualizations**
- **Interactive Maps**:
  - **Flood Locations**: Shows regions affected by flooding.
  - **Severity Levels**: Highlights severity variations across regions.

- **Severity Breakdown**:
  - Bar chart illustrating the distribution of severity levels per region.

- **Key Metrics**:
  - Total flood alerts.
  - Most affected regions.
  - Recent severity changes.


