# Microsoft Fabric Monitoring Hub 

This hands-on lab demonstrates how to monitor data engineering activities in Microsoft Fabric using the centralized Monitoring Hub.

## Lab Objectives

✔️ Create and monitor a Lakehouse  
✔️ Build and track Dataflow Gen2 pipelines  
✔️ Run and observe Spark notebook executions  
✔️ Customize monitoring views for operational analytics  

## Prerequisites

- Microsoft Fabric tenant access
- Workspace with Fabric capacity (Trial/Premium/Fabric)
- Basic knowledge of:
  - Dataflows Gen2
  - Spark notebooks
  - Lakehouse architecture

## Step-by-Step Guide

### 1. Workspace Setup

1. Navigate to https://app.fabric.microsoft.com
2. Create new workspace with Fabric capacity
3. Verify empty workspace initialization

### 2. Lakehouse Creation

1. Select "Create" → "Lakehouse"
2. Name your lakehouse (e.g., "SalesData")
3. Observe empty Tables/Files sections

### 3. Dataflow Implementation

1. Create new Dataflow Gen2
2. Import CSV from: 
   https://raw.githubusercontent.com/MicrosoftLearning/dp-data/main/products.csv
3. Publish and monitor execution status
4. Verify products table creation in Lakehouse

### 4. Spark Notebook Monitoring

1. Create new Notebook
2. Connect to Lakehouse
3. Run Spark query on products table
4. Stop Spark session
5. Review execution in Monitoring Hub

### 5. Advanced Monitoring

1. View historical runs
2. Apply filters (Status=Success, Type=Dataflow)
3. Customize columns:
   - Activity Name
   - Duration  
   - Submitted By
   - etc.

### Key Features Demonstrated

▸ Unified Monitoring: Track all Fabric items in one hub
▸ Run History: Audit past executions with detailed metadata
▸ Custom Views: Filter by status/type and select relevant columns

### Cleanup

1. Navigate to Workspace Settings
2. Select "Remove this workspace"
