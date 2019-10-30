GCP Service Account Deployment
Prerequisites
- Enabled Deployment Manager and Cloud IAM APIs
Enable it at https://console.developers.google.com/apis/api/iam.googleapis.com/overview
- An enabled deploymentmanager.googleapis.com API on your project
Enable it at https://console.cloud.google.com/flows/enableapi?apiid=deploymentmanager,iam
- Make sure your project’s service account (i.e. <RANDOM_NUMBER>@cloudservices.gserviceaccount.com) has the following roles:
 1. Role/Role Administrator
 2. IAM/Security Admin

- Make sure your project's service account(i.e. xxxxx@cloudservices.gserviceaccount.com) has the following roles:
   1.Role/Role Administrator
   2.IAM/Security Admin
   
RUN THE FOLLOWING COMMANDS:
1. Set cloud shell project project_id
   command:  gcloud config set project <project_id> (i.e advance-genre-239305)
2. Create deployment
   command: gcloud deployment-manager deployments create kobura-service-account --config kobura_service_account.yml
3. add iam policy binding to the service account you just created
  command: gcloud projects add-iam-policy-binding  advance-genre-239305 --member serviceAccount:cyb-kobura@advance-genre-  239305.iam.gserviceaccount.com --role roles/owner
   

More Info
https://cloud.google.com/iam/docs/maintain-custom-roles-deployment-manager
