# IOC Investigation Dashboard (SOC MVP)

## Project Overview:
An end-to-end Security Operations Center (SOC) Minimum Viable Product (MVP) designed to automate Threat Intelligence ingestion, data enrichment, and incident correlation using Python and Splunk Enterprise.

## Key Features:
* **Automated Threat Intel Ingestion:** Fetches live IOC feeds from ThreatFox API via Python.
* **Metadata Enrichment:** Automatically assigns `incident_id`, `status`, `assigned_analyst`, and severity tags.
* **IOC-to-Incident Linking:** Correlates multiple raw IOCs (IPs, domains) into unified threat campaigns using Splunk `stats` and `values()` aggregation.
* **Multi-Panel Analytics:**
  * SOC Main Triage Feed
  * Incident Campaign Correlation
  * Severity Breakdown & Threat Classification
  * Historical IOC Trend View (Time-Series Analysis)

## Technologies Used:
* **Language:** Python 3.x
* **SIEM Platform:** Splunk Enterprise
* **Data Sources:** ThreatFox (Abuse.ch) API
* **Data Format:** CSV / JSON Structured Logs

## Repository Structure:
* `fetch_ioc_feeds.py` - Main data pipeline and enrichment script
* `live_ioc_feed.csv` - Ingested IOC log dataset
* `SPL Queries.txt` - Splunk dashboard panel queries
* `Arisha Fatima_IOC_Investigation_Dashboard.pdf` - Complete documentation & analysis report
