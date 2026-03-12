# cerulean_workflows
Repository of the CIF argo workflows



Workflows here are directly usable on CIF platform. 
To re-use on a different platform, some adaptations might be needed. 

## Quick Setup
### 1. Clone the repository

### 2.Update Environment-Specific Settings
Edit workflow.yaml and change:

Change namespace namespace: your-namespace

Update/remove storage class (or use "standard") storageClassName: your-storage-class # or remove this line

Update/remove service account serviceAccountName: your-service-account # or remove this line

Connect your bucket if needed or store artifacts directly

### 3. use credentials for the services

Option A

set credentials as secrets on kubernetes level and adapt names in the workflow

Option B

use credentials directly in the workflow and just delete the env variable section from workflow yaml and replace variables with actual values
