The purpose of the this product is to ensure that when the HEAR measure is added to the cart, the product name and product icon will be different. 

Important** : Once the product setup is complete, check the "Cart Page" configuration under [[Multi-Incentive]].
## How to Create this Application:

 Go to CATALOG -> Products (create a new Virtual product)
	 ![[Screenshot 2025-01-22 193419.png]] 
 ** Attribute Set: cr_past_purchase
 ** Product Name and SKU (Provide as required)
 ** Price (Not required, provide '0')
 ** Visibility: Not Visible Individually
 ** is Drafted?: Enable (if 'My Saved Application' requirement is in scope)
	 ![[Pasted image 20250131155732.png]]
# Content:
 ** Implement the product description in this section as required.
# Clrearesult Config**
 ** Inventory Service: rebate
 ** Skip Checkout: Enable
 ** Eligibility Check: Enable
 ** [[Eligibility App URL]]: (Configure the link only if the application is VUE-based; otherwise, leave it blank)
	 QA: https://static-qa.clearesult.io/components/general/product-recommendation-assessment-app.min.js
	 PROD: [https://static.clearesult.com/components/general/product-recommendation-assessment-app.min.js](https://static.clearesult.com/components/general/product-recommendation-assessment-app.min.js "https://static.clearesult.com/components/general/product-recommendation-assessment-app.min.js")
# Product in Websites**
 ** Ensure the correct store is selected to reflect the product in Front-end
# [[Pimcore]]**
  ** Measure id: 
	 Just add a Place Holder Measure ID
  ** Pimcore Product ID: 
	 Not Required
  ** Incentive Category Group: 
	  Not Required
  ** Incentive Count: Not Required
  ** Incentive Type: 
	  select 'rebate'
  ** Rebate Type:
	  select 'Rebate Reservation'
  ** [[Measure Config JSON]]:
	  Not Required
  ** Measure Class ID: 
	  Configure as required (Used for Account validation check)
  ** Incentive Text:
	  Not Required
  ** Program Id:
	  config the PRJ as per the program
	  Eg: ![[Pasted image 20250131225934.png]]

# Note: 
** Always try to update the Product level config under store view scope.	![[Screenshot 2025-01-24 195200 4.png]]