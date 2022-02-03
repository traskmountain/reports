# GCP -- GET CPU AND RAM PROVISIONED ACROSS MULTIPLE PROJECTS
**PREREQUISITES:**
1) gcloud - Ensure you have your environment configured to execute the gcloud

**EXAMPLE:**

	gcloud config list

	[compute]

	region = us-ast

	zone = us-east-b

	[core]

	account = user@user.com

	disable_usage_reporting = True

	project = dev-project-1

2) Permissions - You will need write permissions to the folder you use here

**TO EXECUTE:**
./master

**NOTES**
"master" is the main script which calls get_projects, get_cpu_ram, and calculate scripts. 

If you have many projects, you may need to either increase the iterations through get_cpu_ram by uncommenting lines in the block starting at line 59. You may also need to add iterations here. 
