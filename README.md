# gcp

Before you begin make sure to:
- Enable the Deployment Manager and Cloud IAM APIs
- Grant permissions to the Google APIs service account
https://cloud.google.com/iam/docs/maintain-custom-roles-deployment-manager


RUN THE FOLLOWING COMMANDS:

0. gcloud config set project advance-genre-239305
1. gcloud deployment-manager deployments create kobura-role --config roles.yaml
2. gcloud deployment-manager deployments create kobura-service-account --config service_accounts.yaml
