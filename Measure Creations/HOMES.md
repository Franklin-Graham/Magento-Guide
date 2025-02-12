Note **:  Once the HOMES product is created, add a related product. The purpose of the related product is to ensure that when the HOME measure is added to the cart, the product name and product icon will be different. [[HOMES Cart Product]]
## How to Create a "HOMES/Modeled Savings" Application:
	 
 Go to CATALOG -> Products (create a new Virtual product)
	 ![[Screenshot 2025-01-22 193419.png]] 
 ** Attribute Set: cr_past_purchase
 ** Product Name and SKU (Provide as required)
 ** Price (Not required for HOME products, provide '0')
 ** is Drafted?: Enable (if 'My Saved Application' requirement is in scope)
	 ![[Pasted image 20250131155732.png]]

---
# Content:
 ** Implement the product description in this section as required.

---
# Clearesult Config**
 ** Inventory Service: leave blank
 ** Skip Checkout: Enable
 ** Eligibility Check: Enable
 ** [[Eligibility App URL]]: (Configure the link only if the application is VUE-based; otherwise, leave it blank)
	 QA: https://static-qa.clearesult.io/components/general/product-recommendation-assessment-app.min.js
	 PROD: [https://static.clearesult.com/components/general/product-recommendation-assessment-app.min.js](https://static.clearesult.com/components/general/product-recommendation-assessment-app.min.js "https://static.clearesult.com/components/general/product-recommendation-assessment-app.min.js")

---
# Product in Websites**
 ** Ensure the correct store is selected to reflect the product in Front-end

---
# [[Pimcore]]**
  ** Measure id: 
	  Measure-Id is just a place-holder, Ensure "Pimcore Program Id" configured in VUE
  ** Pimcore Product ID: 
	  config if required (HOMES its not required)
  ** Incentive Category Group: (add if needed, most cases its not required for HOMES)
  ** Incentive Count: (add if needed, most cases its not required for HOMES)
  ** Incentive Type: 
	  select 'rebate'
  ** Rebate Type:
	  select 'Modeled Savings'
  ** [[Measure Config JSON]]:
	  JSON Structure for HOMES:
	  ![[Pasted image 20250131225831.png]]
	 {"stepsFile":"modeledSavings","rebateType":"HER","accountDetailsEnabledFields":["account_number","account_holder_email_address","account_holder_phone_number","hear_about_us"]}
	 
  ** Measure Class ID: 
	  Configure as required (Used for Account validation check)
  ** Incentive Text:
	  Configure it if required (Price Text will reflect in Product Tile on front-end)
  ** Program Id:
	  config the PRJ as per the program
	  Eg: ![[Pasted image 20250131225934.png]]

---
# Note: 
** Always try to update the Product level config under store view scope.	![[Screenshot 2025-01-24 195200 4.png]]

---