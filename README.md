# GCP Service Account Deployment
Prerequisites
- Enabled Deployment Manager and Cloud IAM APIs
  Enable it by visiting https://console.developers.google.com/apis/api/iam.googleapis.com/overview?project=<PROJECT_ID>
  
  To Register your application for Cloud Deployment Manager V2 API, Identity and Access Management (IAM) API in Google Cloud Platform:
  https://console.cloud.google.com/flows/enableapi?apiid=deploymentmanager,iam&_ga=2.80242391.-132539637.1571300522

- Make sure your project's service account(i.e. xxxxx@cloudservices.gserviceaccount.com) has the following roles:
   1.Role/Role Administrator
   2.IAM/Security Admin
   
RUN THE FOLLOWING COMMANDS:
1. Set cloud shell project project_id
   command:  gcloud config set project <project_id> (i.e advance-genre-239305)
2. Create deployment
   command: gcloud deployment-manager deployments create kobura-service-account --config kobura_service_account.yml
   

More Info
https://cloud.google.com/iam/docs/maintain-custom-roles-deployment-manager

