Go to -> stores -> configuration -> select website scope -> Eligibility Apps -> Eligibility Vue Apps
# Eligibility Vue Apps
- Vue Apps Options by MultiIncentive
  Is Enabled: Enable
  Rebate: 
  Is Enabled: Enable
- Prescreened Apps:
  Is Enabled : Disable
- Assessment Apps:
  Is Enabled : Disable
- Vue Apps Options by Income Verification:
  Is Enabled : Enable
  Document Upload:
  S3 Bucket Endpoint : Ensure the URL (mostly default and QA & PROD the URLs differ)
  Project Key: Differ for store
  Documents Upload App URL: Ensure the URL (mostly default and QA & PROD the URLs differ)
  ![[Pasted image 20250203225353.png]]
  
  **Leave rest of the settings as default

# Income Verification V2:
  
Go to -> stores -> configuration -> select website scope -> Eligibility Apps -> Income Verification V2

- General:
  Enable: Yes 
- Product Settings
  Income Verification Product : select the "Income Verification" product that created [[INCOME VERIFICATION]]
	![[Pasted image 20250203225842.png]]
- Modal Options: Theme:
  Show Store Logo: No
  Show Powered By CLEAResult Logo : No
  
- Modal Options: Customer:
  Redirect Customer : Yes
  Redirect to : Create Account
  
- Modal Options: Documents Upload:
  Configure the Endpoint and Project Keys as required, Mostly the Endpoint with the default value, Project Key will differ for all programs
  ![[Pasted image 20250203230219.png]]