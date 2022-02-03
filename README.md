# GCP -- GET CPU AND RAM PROVISIONED ACROSS MULTIPLE PROJECTS
**OBJECTIVE**
These scripts iterate through GCP projects and instances to produce the total CPU and RAM provisioned. The output is printed to the screen, and can be seen in FinalReport.txt once the process is complete. 

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

2) (Optional) - Prepare projects.txt. This is a flat file with one project-id per line. If you do not prepare this file the process will gather all CPU and RAM across all projects for which you have access.

3) Permissions - You will need write permissions to the folder you use here

**TO EXECUTE:**
./master

**NOTES**
* "master" is the main script which calls get_projects, get_cpu_ram, and calculate scripts. 

* If you have many projects, you may need to either increase the iterations through get_cpu_ram by uncommenting lines in the block starting at line 59. You may also need to add iterations here. 
