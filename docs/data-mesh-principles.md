# Data Mesh Implementation at Shell

## Four Principles Applied

### 1. Domain Ownership
- Each domain team (Upstream, Downstream, Chemicals, Trading) owns their Data Products
- Domain teams responsible for schema · quality · SLAs · documentation
- Central platform team provides infrastructure only

### 2. Data as a Product
- Every Data Product has: schema contract · SLA · quality metrics · documentation
- Discoverable via Collibra data catalog
- Versioned and governed via Unity Catalog

### 3. Self-Serve Infrastructure
- Shell.ai platform for engineers · analysts · data scientists
- No ticket needed to access approved Data Products
- Databricks notebooks for exploration and analysis

### 4. Federated Governance
- Unity Catalog enforces access policies across all domains
- Collibra holds business definitions · lineage · ownership
- GDPR compliance built into access controls

## Technology Decisions

| Decision | Technology | Reason |
|---|---|---|
| Compute | Databricks | Unified analytics · Delta Lake native support |
| Storage format | Delta Lake + Parquet | ACID · CDC · time travel · columnar |
| Cloud storage | ADLS Gen2 | Azure-native · hierarchical namespace |
| Governance | Unity Catalog | Fine-grained column-level access |
| Catalog | Collibra | Business glossary · lineage · stewardship |
