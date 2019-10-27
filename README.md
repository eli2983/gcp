# gcp

RUN THE FOLLOWING COMMANDS:

0. gcloud config set project elis-project-1983
1. gcloud deployment-manager deployments create kobura-role --config roles.yaml
2. gcloud deployment-manager deployments create kobura-service-account --config service_accounts.yaml
