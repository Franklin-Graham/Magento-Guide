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

elseif (isHttpHost("ec2-" . $defaultEnv . "-entergytx.clearesult.io")) {
        $_SERVER["MAGE_RUN_CODE"] = "main_entergytx";
        $_SERVER["MAGE_RUN_TYPE"] = "website";
    }

