# Analyzing-DNS-Logs-using-Splunk-SIEM
A SOC Project that analyzes DNS based log files using Splunk SIEM to identify suspicious activity, create customized fields and to build detection logic using SPL (Search Processing Language)


Objectives:
- Ingest and analyze DNS logs in Splunk Enterprise
- Create custom fields for better visibility
- Identify suspicious DNS patterns
- Support SOC Investigation with dashboards and queries

Tools & Technologies:
- Splunk Enterprise / Splunk SIEM
- DNS log sources (BIND / Windows DNS / Zeek DNS logs)
- SPL (Search Processing Language)

Project Architecture:

- DNS logs are collected from log sources
- Logs are ingested into Splunk
- Fields are extracted and normalized by creating indexes
- SPL queries are used for detection and analysis
- Dashboards and alerts support SOC workflows

Procedure:
1. Log Ingestion
Configure DNS log forwarding to Splunk
Verify indexing and sourcetype assignment

2. Field Creation & Normalization
Extract fields such as:
-Query name
-Query type
-Source IP
-Response code
-Create calculated fields for enrichment

3. Analysis Using SPL:
-Identify high-frequency DNS queries
-Detect suspicious domains and uncommon TLDs
-Monitor NXDOMAIN and failed resolution patterns

4. Detection Use Cases:
-Malware C2 communication via DNS
-DNS tunneling behavior
-Phishing and newly registered domains

5. Visualization & Reporting:
-Build dashboards for DNS activity trends
-Create alerts for high-risk indicators

Learning Outcomes:
-Hands-on experience with Splunk SIEM
-Practical understanding of DNS-based threats
-Ability to design SOC-ready detection logic
