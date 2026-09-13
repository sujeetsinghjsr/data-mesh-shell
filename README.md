# Shell Data Mesh Platform — Enterprise Transformation

> IBM India embedded at Shell | Aug 2022 – Oct 2025

## Overview

Contributed to Shell's enterprise **Data Mesh transformation** enabling domain-oriented
Data Products across global business units using Azure, AWS, and Databricks.

## Architecture

```
Shell Business Domains
    ↓
Domain Data Products (owner: each domain team)
    ↓
Databricks Lakehouse (Bronze → Silver → Gold)
    ↓  Delta Lake · Parquet · ADLS Gen2
Unity Catalog (governance · lineage · access controls)
    ↓
Collibra (metadata · data catalog · business glossary)
    ↓
Shell.ai Platform (self-serve for engineers · analysts · data scientists)
```

## What I Worked On

### Databricks Lakehouse
- Designed Bronze / Silver / Gold layer architecture using Delta Lake and Parquet
- Implemented CDC (Change Data Capture) for incremental processing
- Built batch and real-time streaming pipelines using PySpark and Apache Spark
- Enabled ADLS Gen2 as scalable lakehouse storage on Azure

### Data Governance
- Implemented Unity Catalog for data governance and policy-based access controls
- Integrated Collibra for metadata management, data lineage, and data catalog
- Built data quality and validation frameworks for domain data products
- Delivered GDPR-compliant data modernisation across global business units

### Data Mesh Principles Applied

| Principle | Implementation |
|---|---|
| Domain ownership | Each domain team owns and maintains their Data Product |
| Data as a product | Schema contracts · SLAs · quality metrics per Data Product |
| Self-serve infrastructure | Shell.ai platform for engineers and analysts |
| Federated governance | Unity Catalog + Collibra for policy enforcement |

### Shell.ai Platform
- Enabled self-serve data access for engineers, analysts, and data scientists
- Built governed Data Products supporting large-scale analytics and AI workloads
- Led PoC initiatives validating new capabilities before enterprise rollout

## Technology Stack

| Category | Technology |
|---|---|
| Compute | Databricks · Apache Spark · PySpark |
| Storage | Delta Lake · Parquet · ADLS Gen2 |
| Cloud | Microsoft Azure · AWS |
| Governance | Unity Catalog · Collibra |
| Patterns | Data Mesh · Data Products · CDC · Streaming · Batch |
| Compliance | GDPR |
| Tools | JIRA · Confluence · Azure DevOps |
