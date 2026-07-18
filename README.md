# ☁️ Day 1 — Introduction to Data Analytics on Google Cloud

> **Course:** Introduction to Data Analytics on Google Cloud  
> **Learning Path:** Data Analyst (Google Skills)


This README contains the markdown version of my study notes for quick reading and GitHub search.

---

# 📚 Topics Covered

- Data Analytics Lifecycle
- Data Ingestion
- Data Processing
- Data Storage
- Data Analysis
- Data Activation
- Google Cloud Data Sources
- Google Cloud Analytics & ML Services

---

# 🔄 Data Analytics Lifecycle

Every analytics workflow on Google Cloud follows a continuous cycle:

```text
Ingest → Process → Store → Analyze → Activate
```

Everything is built on three core foundations:

- Store Data
- Manage Data
- Organize Data

### Lifecycle Overview

| Stage | Purpose |
|--------|---------|
| Ingest | Bring data into Google Cloud |
| Process | Clean and transform data |
| Store | Save data securely and efficiently |
| Analyze | Generate insights |
| Activate | Use insights in dashboards, reports, or ML models |

---

# 🍽️ Easy Analogy

Think of a restaurant kitchen.

- Ingredients arrive → **Ingest**
- Washed & chopped → **Process**
- Stored in fridge → **Store**
- Chef decides the menu → **Analyze**
- Food served to customers → **Activate**

---

# 🛠 Google Cloud Services

| Stage | Google Cloud Products |
|--------|----------------------|
| Ingest | Pub/Sub, Dataflow, Dataproc, Cloud Data Fusion |
| Process | Dataflow, Dataproc, Cloud Data Fusion |
| Store | Cloud Storage, Cloud SQL, BigQuery, Firestore, Bigtable, AlloyDB, Cloud Spanner |
| Analyze | BigQuery, Looker, Looker Studio |
| Activate | Vertex AI, AutoML, Workbench, TensorFlow |

---

# 📥 Ingestion

Data ingestion is the process of bringing raw data into Google Cloud.

### Types

### 🔹 Real-time (Streaming)
- Continuous updates
- Example: Live cricket score

### 🔹 Batch
- Processed on a schedule
- Example: Bank statement

---

## Cloud Data Fusion

- Fully managed ETL service
- Drag-and-drop interface
- Integrates cloud and on-premises data
- No coding required

### ETL

- **Extract** → Collect data
- **Transform** → Clean & modify
- **Load** → Store in destination

---

## Pub/Sub

- Receives incoming events
- Message queue service

**Think of it as:** 📬 Mailbox

---

## Dataflow

- Processes streaming or batch data
- Performs transformations

**Think of it as:** 📖 Opening and processing the mail

---

# ⚙️ Processing

Processing prepares raw data for analysis.

Common tasks:

- Remove duplicates
- Fix errors
- Change formats
- Merge datasets

### Services

- Dataflow → Streaming
- Dataproc → Batch
- Cloud Data Fusion → Integration

---

# 💾 Storage

Google Cloud offers three major storage approaches.

## Database

Stores structured data.

Examples:

- Cloud SQL
- Cloud Spanner
- AlloyDB
- Firestore
- Bigtable

---

## Data Warehouse

Designed for analytics.

Example:

- BigQuery

---

## Data Lake

Stores raw data of any type.

Example:

- Cloud Storage

---

## Storage Services

| Product | Type |
|----------|------|
| Cloud Storage | Object Storage |
| Cloud SQL | Relational Database |
| Cloud Spanner | Relational Database |
| AlloyDB | Relational Database |
| BigQuery | Data Warehouse |
| Firestore | NoSQL Database |
| Bigtable | NoSQL Database |

---

# 🗄 Database Types

## Relational (SQL)

Examples

- Cloud SQL
- Cloud Spanner
- AlloyDB

Characteristics

- Tables
- Fixed schema
- Relationships

---

## NoSQL

Examples

- Firestore
- Bigtable

Characteristics

- Flexible schema
- Handles changing data structures

---

# 📂 Types of Data

### Structured

- Tables
- Rows and columns

Example:

Customer database

---

### Semi-Structured

Contains labels or tags.

Example:

Emails

---

### Unstructured

No predefined format.

Examples

- Images
- Videos
- Audio
- Documents

---

# 📊 Analyze

## BigQuery

Google Cloud's enterprise data warehouse.

Features

- SQL-based analytics
- Highly scalable
- Fast querying
- Cloud-native

---

## Looker

Business Intelligence platform for dashboards and reports.

---

## Looker Studio

Free visualization tool for creating interactive dashboards.

---

# 🤖 Activate

Turn insights into Machine Learning solutions.

## Vertex AI

Google Cloud's ML platform.

Includes:

- AutoML
- Vertex AI Workbench
- TensorFlow

---

# 🔗 Google Cloud Data Sources

Google Cloud can connect to data stored in different locations.

## Cloud Sources

Stored within Google Cloud.

Examples

- Cloud Storage
- Cloud SQL

---

## External Sources

Stored outside Google Cloud.

Examples

- Amazon S3
- Microsoft SQL Server
- On-premises databases

---

## Ways to Create Connections

- Google Cloud Console
- Cloud SDK
- Google Cloud APIs

---

# ✅ Benefits

- Centralized data access
- Connect multiple data sources
- Build Data Warehouses
- Build Data Lakes
- Easier analytics
- Better reporting
- Supports Machine Learning

---

# 📝 Key Takeaways

- Data analytics follows a continuous lifecycle.
- Google Cloud provides services for every stage of analytics.
- BigQuery is the core analytics platform.
- Looker and Looker Studio help visualize data.
- Vertex AI enables Machine Learning.
- Google Cloud supports both cloud-native and external data sources.

---

## 📌 Resources

- **Course:** Introduction to Data Analytics on Google Cloud
- **Platform:** Google Skills
- **Learning Path:** Data Analyst

---

> **Notes compiled as part of my Google Cloud Data Analytics learning journey.**
```
