Day 1 — Introduction to Data Analytics on Google Cloud

Course: Introduction to Data Analytics on Google Cloud (Google Skills)
Path: Data Analyst

Full polished PDF version (with diagrams and icons) is in assets/day-01-notes.pdf. This file is the plain-text/markdown version for quick reading and searching on GitHub.


Overview: The Data Analytics Lifecycle

Every data analytics workflow on Google Cloud follows the same basic lifecycle, no matter how big or small the project is. Three things form the foundation for everything else:


Storing
Managing
Organizing


On top of this foundation, data moves through five stages in a continuous loop:

Ingest → Process → Store → Analyze → Activate


In simple words: First you bring data in (Ingest), clean and transform it (Process), keep it somewhere safe (Store), find insights from it (Analyze), and finally put those insights to use — reports, dashboards, or ML models (Activate). Activate often feeds new data back into Ingest, so the cycle repeats.




Analogy — running a restaurant kitchen: ingredients arrive at the back door (Ingest), the chef washes and chops them (Process), they get stored in the fridge or pantry (Store), the chef decides what dish to cook by checking what is fresh (Analyze), and finally the dish is served to a customer (Activate). Tomorrow, new ingredients arrive again, and the cycle repeats.



Quick summary of tools used at each stage

StageGoogle Cloud ProductsPurposeIngestPub/Sub, Dataflow, Dataproc, Cloud Data FusionBring in real-time and batch dataProcessDataflow, Dataproc, Cloud Data FusionClean, transform, and prepare dataStoreCloud Storage, Cloud SQL, Spanner, BigQuery, Firestore, Bigtable, AlloyDBKeep data organized and scalableAnalyzeBigQuery, Looker, Looker StudioQuery, analyze, and visualize dataActivateVertex AI, AutoML, Workbench, TensorFlowTurn insights into ML and action


Ingestion

Ingestion is the very first step: getting raw data from wherever it lives into Google Cloud, in real time or in batches.


Real-time vs. batch: Real-time (streaming) is like a live cricket score that updates the moment something happens. Batch is like a weekly bank statement — data is collected and processed all at once, on a schedule (e.g., once a day or once a week).



Cloud Data Fusion


A fully managed, cloud-first data integration service.
A code-free ETL (Extract, Transform, Load) tool.
Integrates data across on-premises and cloud sources (on-premises = servers/computers owned and run by a company itself, as opposed to the cloud) using a visual, drag-and-drop interface — no need to write pipelines by hand.



What is ETL? Extract (pull data out of a source, like a sales system), Transform (clean it up — fix errors, rename columns, convert formats), Load (put it into its new home, like a database). Cloud Data Fusion lets you do all three by dragging and connecting boxes on a screen, similar to building a flowchart, instead of writing code.



Pub/Sub & Dataflow


Both are streaming analytics services used together for real-time data pipelines.
Pub/Sub is used for ingestion: it receives and queues messages/events as they arrive.
Dataflow is used for analytics and processing: it transforms and processes the streamed or batched data.



In simple words: Pub/Sub is like a mailbox that catches incoming data the moment it arrives. Dataflow then opens that mail and processes it.




Process

Once data is ingested, it needs to be cleaned, transformed, and made ready for analysis. Processing simply means fixing errors, removing duplicates, converting formats, or combining fields so the data is usable.


Dataproc can be used for batch processing of data.
Dataflow is used to stream data for real-time processing.
Cloud Data Fusion is used to integrate data coming from multiple sources into one clean pipeline.



Everyday example: Raw data is like vegetables straight from the farm — some dirty, oddly shaped, or mixed with stones. Processing is washing, peeling, and cutting them into uniform pieces, so they're ready to cook (analyze) later.




Tip to remember: Dataproc = batch, Dataflow = stream, Data Fusion = integration from many sources. All three can also help at the Ingest stage; they overlap because ingestion and processing often happen together.




Store

Storage also needs to scale with your data. There are three broad storage options:


Databases
Data Warehouses
Data Lakes


Storage products on Google Cloud

#ProductType1Cloud StorageObject storage2Cloud SQLRelational database3Cloud SpannerRelational database4BigQueryData warehouse5FirestoreNoSQL database6Cloud BigtableNoSQL database7AlloyDB for PostgreSQLRelational database

Databases

A database is an organized collection of data, stored in tables and accessed electronically from a computer system. Google Cloud offers both relational and non-relational (NoSQL) databases.


Analogy: A database is like a well-organized Excel workbook — data sits in neat rows and columns (tables), and you can quickly look up, add, or update information.



Relational Databases (SQL) — Cloud SQL, Cloud Spanner, AlloyDB for PostgreSQL
Can establish links/relationships between tables. Highly consistent and reliable; best suited for large, structured data.

Non-Relational Databases (NoSQL) — Bigtable, Firestore
Less structured, no fixed tabular format. Follows a flexible data model, ideal for data whose structure changes frequently.


Analogy: A relational (SQL) database is like a strict Excel sheet, where every row must follow the same fixed columns. A NoSQL database is like a set of flexible sticky notes, where each note can hold different information.



Data Warehouse

An enterprise system used for the analysis and reporting of structured and semi-structured data from multiple sources.
Example on Google Cloud: BigQuery, used to analyze data.

Data Lake

A repository designed to ingest, store, explore, process, and analyze any type or volume of raw data, regardless of source. Can store data in its original format, ignoring size limits, without much pre-processing.


Analogy: A data warehouse is like a well-labelled library — books are already sorted and catalogued. A data lake is like a large storage room where boxes are dumped as-is, unsorted, to be organized later. Both are useful: the warehouse for quick, structured answers; the lake for keeping everything just in case.



Types of Data


Structured — fits neatly into rows and columns (e.g., a customer table).
Unstructured — no fixed format (e.g., photos, videos, free text).
Semi-structured — some organization (tags/labels) but not a strict table (e.g., an email).



Analyze

BigQuery


BigQuery is at the core of data analytics on Google Cloud.
An elastic, flexible, secure, and reliable data warehouse that works across clouds and scales with your data.
Used to analyze data through SQL commands.
Lets you build a cloud-first data warehouse.



What is SQL? SQL (Structured Query Language) is a way of asking questions to your data using near-English sentences, e.g., "Show me all customers from Mumbai who spent over ₹5,000 last month." BigQuery lets you run these questions on huge amounts of data in seconds.



Looker & Looker Studio

Used to analyze and visualize data, turning raw query results into charts, dashboards, and reports.


Analogy: If BigQuery is the calculator that crunches the numbers, Looker/Looker Studio are the presenters that turn those numbers into easy-to-read graphs and dashboards.




Activate

Data is also the key to unlocking the value of Machine Learning on Google Cloud.


What is ML in one line? Teaching a computer to spot patterns in past data so it can make predictions on new data — e.g., showing it thousands of past emails marked "spam"/"not spam" so it learns to flag new spam automatically.



Vertex AI

The primary development product of the ML platform on Google Cloud. Includes:


AutoML — builds ML models automatically, with little to no coding required (good for beginners).
Workbench — a notebook-style workspace for writing and testing model code.
TensorFlow — a popular open-source library for building custom ML models from scratch.



In simple words: Once data is clean, stored, and analyzed, Activate is where it gets put to work — training ML models to make predictions or automate decisions.




Google Cloud Data Sources & Storage Methods

Data sources are connectors that let you query data from various sources without moving it first.


Analogy: A data source connection is like a universal charging cable — it lets BigQuery "plug into" data sitting anywhere and read it directly, without copying or moving it first.



Cloud Data Sources — stored on Google Cloud itself (e.g., a Cloud Storage bucket or Cloud SQL database).

External Data Sources — stored on-premises or in another cloud provider (e.g., an Amazon S3 bucket or Microsoft SQL Server database).

How to create a data source connection


Google Cloud Console
Cloud SDK
Google Cloud API


Benefits


Gives centralized access to your data, regardless of where it's stored.
Helps integrate data from different sources.
Useful for building data warehouses and data lakes.
Makes it easier to analyze and visualize data.



Notes compiled from personal study notes • Google Skills: "Introduction to Data Analytics on Google Cloud"
