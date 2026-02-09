# FabricNeedles

Reusable Microsoft Fabric tools to accelerate deployment and operationalize data engineering workflows (Lakehouse, notebooks, pipelines).

## What this is

**FabricNeedles** is a small toolkit of reusable helpers intended to reduce copy/paste in Fabric notebooks and make deployments more repeatable. The focus is on:

- **Idempotent deployments** (create-or-get patterns)
- **Metadata-driven workflows** (manifest/spec-driven ingestion + promotion patterns)

### Index






Deploy Lakes:

Upload the requirements to the workspace. 
Open a new notebook and run this in a cell:
```
# first check if the notebook artifacts are accessible
notebookutils.notebook.get("util_deploy_lakes")
notebookutils.notebook.get("util_get_lake")

# if get returns the artifact, run this in a new cell:
notebookutils.notebook.run("util_deploy_lakes", timeout_seconds=200)
```

Required Notebooks
- util_deploy_lakes
- util_get_lake
