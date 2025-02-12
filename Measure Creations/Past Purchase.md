Check the [[Past Purchase Flow]]
## How to Create a Past Purchase product:

 Go to CATALOG -> Products (create a new Virtual product)
	 ![[Screenshot 2025-01-22 193419.png]] 
 ** Attribute Set: cr_past_purchase
 ** Product Name and SKU (Provide as reuired)
 ** Price (Not required for past purchase products, provide '0')
 ** is Drafted?: Enable (if 'My Saved Application' requirement is in scope)
	 ![[Pasted image 20250131155732.png]]

---
# Content:
 ** Implement the product description in this section as required.

---
# Clrearesult Config**
 ** Inventory Service: select "rebate"
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
	  The ID will provide by Pimcore Team (use for measure incentive and other savings calculations)
  ** Pimcore Product ID: 
	  provide by pimcore Team (configure if its needed)
  ** Incentive Category Group: (add if needed)
	  The sub-category needs to be configured as per the sub-category set in Pimcore, which will be used for the past-participation check and [[Cart Stacking Limit]].
  ** Incentive Count: 
	  (Give default as "1", will vary based on Pac-Size)
  ** Related Incentive SKUs:
      Link the other products with the respective SKU's 
  ** Incentive Type: 
	  select 'rebate'
  ** Rebate Type:
	  select 'past purchase'
  ** [[Measure Config JSON]]:
	  Config the JSON as required
  ** Measure Class ID: 
	  Configure as required (Used for Account validation check)
  ** Incentive Text:
	  Configure it if required (Price Text will reflect in Product Tile on front-end)
  ** Program Id:
	  config the PRJ as per the program

---

# Note: 
** Always try to update the Product level config under store view scope.	![[Screenshot 2025-01-24 195200 4.png]]

---