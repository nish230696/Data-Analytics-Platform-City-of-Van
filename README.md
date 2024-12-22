# Data-Analytics-Platform-City-of-Van

AWS Data Analytics Platform for the City of Vancouver
This project focuses on creating an efficient, secure, and cost-effective Data Analytics Platform (DAP) leveraging AWS cloud tools. The objective is to analyze and derive actionable insights from the City's Open Data, particularly focusing on "Issued Building Permits."

Phase 1: Design and Implementation
Data Ingestion: The "Issued Building Permits" dataset was filtered for Downtown Vancouver for 2024. The data was ingested into AWS S3 buckets, categorized for unprocessed and processed files.

Data Profiling & Cleaning: AWS Glue DataBrew was utilized to handle missing values and normalize formats, improving data quality and usability.

Pipeline Design: The data pipeline streamlined transformations, dropping unnecessary features, and aggregating data for monthly permit analysis.

Phase 2: Enrichment, Protection, and Governance
Data Enrichment: Additional fields, such as holiday indicators, were added to explore their effects on permit issuance. SQL queries in AWS Athena revealed trends, such as a holiday-related delay in permit approvals.

Data Protection: Encryption using AWS KMS, bucket versioning, and replication rules ensured robust data security and compliance. Only authorized users were granted access.

Data Governance: Sensitive data detection was integrated, and quality checks filtered out low-quality records. A systematic pipeline organized validated and failed data for further processing.

Observability: Alarms and dashboards in CloudWatch monitored bucket activity, costs, and potential breaches. Metrics helped identify the most resource-intensive processes and ensured cost control.

Teamwork and Operational Analysis
The team collaborated on key architectural pillars:

Operational Excellence: Backup and automation steps enhanced reliability but lacked advanced recovery procedures.
Security: Encryption and controlled access were implemented, though traceability measures were limited.
Performance Efficiency: Efficient use of AWS Glue, S3, and Athena streamlined data operations but could improve with storage optimizations.
Cost Optimization: Although efforts to minimize costs were made, inconsistent analysis of capacity needs led to suboptimal resource utilization.
Sustainability: Minimal focus on environmental impact but reduced reliance on on-premises systems lowered energy consumption.
This initiative demonstrates how cloud computing tools can transform municipal data into actionable insights while adhering to governance, security, and cost-efficiency standards
