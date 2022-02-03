# GET CPU AND RAM PROVISIONED ACROSS MULTIPLE PROJECTS
Prerequisites:
1) gcloud - Ensure you have your environment configured to execute the gcloud

EXAMPLE: 
gcloud config list
[compute]
region = us-ast
zone = us-east-b
[core]
account = user@user.com
disable_usage_reporting = True
project = dev-project-1

2) Permissions - You will need write permissions to the folder you use here

To Execute:
./master

Notes:
-"master" is the main script which calls get_projects and then cpu_ram scripts. 
