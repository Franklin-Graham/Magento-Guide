Why this PR needed? 
	PR for Order sync from Magento to Salesforce
	 Order Flow : Magento -> Lambda -> DSMT/ATLAS(salesforce)
Note** : Ensure all below changes are done only in 'Develop' branch

Step 1: Create a new branch in Azure

![[Screenshot 2025-02-04 163435.png]]

Creating New Branch:
Name: provide the Name as required (add the path feature, as mentioned in IMG)
Based on: develop (Ensure always to select develop branch while raising PR's)
Worked Items to link: Select the work item of store creation 

Step 2: clone the relevant repository in local machine:
Clone this repo in local: https://dev.azure.com/clearesultdev/Digital%20Platform/_git/org.digital.backend.salesforce-dispatcher/
   How to clone?
   open Terminal and command git clone <add the cloning repo>
   
Step 3: Add the code
	Once the cloning is done, the next step is to add the "Tenant id" and Store Code in the 'websites.config.js' file which is under 'salesforce-dispatcher' file (use any tools like VS code for editing)
	Add the store code, name, tenant (Salesforce dev will provide the name and tenant)
		![[Pasted image 20250204204420.png]]

Step 4: Git pull commands
	Use the below code to push the code changes,
	 PR code deploy commands:
		git pull
		git checkout feature/1233440-New-Store-EntergyTx
		git status
		git add magento2ce/magento-vars.php
		git commit -m "store code update"
		git push
		
Step 5: Create New pull request:
	       Title: provide any store related name
	       Description: add as required
	       Reviewers: choose the reviewer from platform team for Approval
	       Work items to link: select the relevant work item.
	       
	     *Once got an Approval, merge the code
Note** : Ensure all changes are done only in Develop branch
