# FabricNeedles

Reusable Microsoft Fabric tools to accelerate deployment and operationalize data engineering workflows (Lakehouse, notebooks, pipelines).

## What this is

**FabricNeedles** is a small toolkit of reusable helpers intended to reduce copy/paste in Fabric notebooks and make deployments more repeatable. The focus is on:

- **Idempotent deployments** (create-or-get patterns)
- **Consistent OneLake pathing** (Files/Tables with ABFSS)
- **Metadata-driven workflows** (manifest/spec-driven ingestion + promotion patterns)
