# Church-sChicken-RealTime-Analysis
Project Idea: Church’s Chicken – Restaurant Performance Analytics Pipeline
Let’s build a project that simulates a real-world data engineering scenario for a fast-food chain like Church’s Chicken.
What This Project Will Cover:
Component	Tools
Data Ingestion	Azure Blob Storage → ADF Copy
Transformation	Mapping Data Flows (cleaning, deriving fields)
Logging	Stored Procedure for activity logging
Orchestration	Control flow in ADF (lookup, if, parameter-driven pipeline)
Analytics Layer	Load into Azure SQL or Synapse
Visualization (Optional)	Power BI or Excel dashboard

Project Theme: “Restaurant Sales & Support Dashboard”
You’ll simulate and work on:
•	Restaurant-wise daily sales
•	Support tickets for laptop or POS issues
•	Downtime tracking
•	Weekly performance reports
•	Resume-from-last-failed pipeline execution
Folder Structure (on GitHub):
pgsql
CopyEdit
churchs-chicken-analytics/
├── data/
│   ├── sales_data.csv
│   ├── support_logs.csv
├── adf/
│   ├── pipeline_export.json
│   └── sql_scripts/
│       └── create_checkpoint_table.sql
├── README.md
└── visuals/
    └── dashboard.png (optional)

Key Deliverables:
1.	ADF Pipeline:
o	Copy raw sales and support data from Blob
o	Clean data in Mapping Data Flow (nulls, date formats)
o	Log status with a stored proc
o	Use Lookup + If Condition to resume intelligently
2.	Azure SQL DB:
o	Tables: Sales, SupportTickets, ADFCheckpoint
o	Store clean data
3.	Bonus: Power BI Report:
o	Total sales per store
o	Number of support tickets per region
o	Downtime vs. sales correlation
________________________________________
💬 Elevator Pitch for Interviews:
"I built a data pipeline simulating a real business case from my previous role. The project automates ingestion of restaurant sales and support logs, cleans and transforms them in ADF, logs activity status for pipeline resumption, and stores data into Azure SQL DB. This gave me hands-on experience with orchestrating ETL processes, implementing checkpointing logic, and simulating real-time data support workflows."
________________________________________
Would you like me to:
•	Generate sample CSV files for sales data and support logs?
•	Create the README structure with steps?
•	Or help you start building the pipeline architecture in ADF?

