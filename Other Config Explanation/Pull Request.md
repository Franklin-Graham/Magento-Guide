Azure Pull Request (PR) Request Guide:
#### **Step 1: Create a New Branch**

Before making changes, create a new branch from the latest "develop" branch.
![[Screenshot 2025-02-04 163435.png]]

Creating New Branch:
Name: provide the Name as required (add the path feature, as mentioned in IMG)
Based on: develop (Ensure always to select develop branch while raising PR's)
Worked Items to link: Select the work item of store creation 
![[Pasted image 20250204164403.png]]


Step 2: Clone the Magento Repo in the Local Machine:
   Clone this repo in local: https://dev.azure.com/clearesultdev/Digital%20Platform/_git/org.digital.ec.magento/
   How to clone?
   open Terminal and command git clone <add the cloning repo>
   
Step 3: Edit the file (magento-vars.php):
	Once the cloning is done, the next step is to add the New store URL and Store Code in the 'magento-vars.php' file (use any tools like VS code for editing)
	Add New elseif condition and add the store URL and Store Code
	for Eg:
	url: -entergytx.clearesult.io
	Store code: main_entergytx
	EC2-QA:
	elseif (isHttpHost("ec2-" . $defaultEnv . "-entergytx.clearesult.io")) {
	        $_SERVER["MAGE_RUN_CODE"] = "main_entergytx";
	        $_SERVER["MAGE_RUN_TYPE"] = "website";
	    }
	    
	once updated, in the same file update the below code for PROD as well with Prod url,
	EC2-PROD:
	Add new elseif condition
	elseif (isHttpHost("entergytx.clearesult.com") || isHttpHost("ec2-" . $defaultEnv . "-entergytx.clearesult.io/")) {
         $_SERVER["MAGE_RUN_CODE"] = "main_entergytx";
         $_SERVER["MAGE_RUN_TYPE"] = "website";
        }

Step 4: Git pull command
	Use the below code to push the code changes,
	 PR code deploy commands:
		git pull
		git checkout feature/1233440-New-Store-EntergyTx
		git status
		git add magento2ce/magento-vars.php
		git commit -m "store code update"
		git push
   
		   Commands Explanation (just for reference):
		   Switch to the develop branch
			git checkout develop:
			This switches the working branch to develop, ensuring you're on the latest development branch before making changes.
			Pull the latest changes from the remote repository
			
			git pull:
			Fetches and merges the latest updates from the remote develop branch into your local develop branch.
			Switch to the feature branch
			
			git checkout feature/1233440-New-Store-EntergyTx:
			Moves to the feature branch where new changes are being made (feature/1233440-New-Store-EntergyTx).
			Check the status of the working directory
			
			git status:
			Displays the status of changes (modified, untracked, or staged files).
			Stage a specific file for commit
			
			git add magento2ce/magento-vars.php:
			Stages magento-vars.php for the next commit.
			Commit the staged changes with a message
			
			git commit -m "store code update":
			Creates a commit with the message "store code update" to record changes in the local repository.
			Push the changes to the remote repository
			
			git push:
			Uploads the committed changes from the local branch (feature/1233440-New-Store-EntergyTx) to the remote repository.
			
			Summary:
			The workflow ensures that the latest updates from develop are included in the feature branch.
			The magento-vars.php file is modified, staged, committed, and then pushed to the remote repository.
			This process is typically followed when working on a new feature to keep the  branch updated and ready for review.
			
	Step 5: Create New pull request:
	       Title: provide any store related name
	       Description: add as required
	       Reviewers: choose the reviewer from platform team for Approval
	       Work items to link: select the relevant work item.