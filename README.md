# gcp-deployment
IaC using GCP Deployment Manager

# Description
This will deploy a simple Apache2 web server in Compute Engine along with a custom VPC

# Usage
1) Enable Deployment Manager API: `gcloud services enable deploymentmanager.googleapis.com`
3) Make a mock deployment: `gcloud deployment-manager deployments create my-deploy --config deploy.yaml --preview`
4) If `STATE` for all services are marked as `IN_PREVIEW`, proceed the actual deployment: `gcloud deployment-manager deployments update my-deploy`
