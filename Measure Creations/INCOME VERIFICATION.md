This product tile will not be listed on the front end. It is designed to open an EW popup on the Pre-Qualification page.
## How to Create a "INCOME VERIFICATION" Application:

 Go to CATALOG -> Products (create a new Virtual product)
	 ![[Screenshot 2025-01-22 193419.png]] 
 ** Attribute Set: cr_verification
 ** Product Name and SKU (Provide as required)
 ** Price (Not required for INCOME products, provide '0')
 ** is Drafted?: Enable (if 'My Saved Application' requirement is in scope)
	 ![[Pasted image 20250131155732.png]]
# Content:
 ** Implement the product description in this section as required.
# Clrearesult Config**
 ** Inventory Service: leave blank
 ** Skip Checkout: Enable
 ** Eligibility Check: Enable
 ** [[Eligibility App URL]]: (Configure the link only if the application is VUE-based; otherwise, leave it blank)
	 QA: https://static-qa.clearesult.io/components/general/product-recommendation-assessment-app.min.js
	 PROD: [https://static.clearesult.com/components/general/product-recommendation-assessment-app.min.js](https://static.clearesult.com/components/general/product-recommendation-assessment-app.min.js "https://static.clearesult.com/components/general/product-recommendation-assessment-app.min.js")
# Product in Websites**
 ** Ensure the correct store is selected to reflect the product in Front-end
# [[Pimcore]]**
  ** Measure id: 
	  Not required
  ** Pimcore Product ID: 
	  Not required
  ** Incentive Category Group: 
	  Not required
  ** Incentive Count: 
	  Not required
  ** Incentive Type: 
	  select 'cr_verification'
  ** Rebate Type:
	  Not required
  ** [[Measure Config JSON]]:
	  JSON Structure for Income verification:
	  ![[Pasted image 20250131231615.png]]
	  {"stepsFile": "incomeQualificationV2"}
	 
  ** Measure Class ID: 
		Not Required
  ** Incentive Text:
		 Not Required
  ** Program Id:
	  config the PRJ as per the program
	  Eg: ![[Pasted image 20250131225934.png]]

# Note: 
** Always try to update the Product level config under store view scope.	![[Screenshot 2025-01-24 195200 4.png]]