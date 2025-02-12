[[buy now explanation]]
Check the Buy Now Flow [[Buy Now Flow]]
## How to Create Buy Now product:
 
 CATALOG -> Products (create a new simple product)
	 ![[Screenshot 2025-01-22 181905.png]]
 ** Attribute Set -> Default
 ** Product Name -> (As Per requirement template) (Ensure there is no any spaces in starting)
 ** SKU -> (As Per requirement template) (Ensure there is no any spaces in starting)
 ** [[Price]]: 
	Need to configure followings,
	** MSRP price: 
	** Customer price:
** Tax Class: Enable the custom Tax Code, otherwise select 'Taxable Goods'
     ![[Pasted image 20250203152509.png]]
 ** Quantity: 0
 ** Weight: provide the weight as required (use to shipping calculation)
 ** Categories: Select the required store category 
 ** Visibility: Hide product in front-end
 ** Model Number: As required
 ** is Drafted?: Enable (if 'My Saved Application' requirement is in scope)
	 ![[Pasted image 20250131155732.png]]

---
# Content:
 ** Implement the product description in this section as required.

---
# Product in Websites: (Important)
 ** Ensure the correct store is selected to reflect the product in Front-end

---
# [[Pimcore]]:
  ** Measure id: 
	  The ID will provide by Pimcore Team (USED for measure calculation)
  ** Pimcore Product ID: 
	  provide by pimcore Team (configure if its needed)
  ** Incentive Category Group: 
	  The sub-category needs to be configured as per the sub-category set in Pimcore, which will be used for the past-participation check and [[Cart Stacking Limit]].
  ** Incentive Count: 
	  (Give default as "1", will vary based on Pac-Size)
  ** Related Incentive SKUs:
      Link the other products with the respective SKU's 
  ** Incentive Type: 
	  none (for Buy Now Products)
  ** Measure Class ID: 
	  Configure as required (Used for Account validation check)
  ** Incentive Text:
	  Configure it if required (Price Text will reflect in Product Tile on front-end)
  ** Program Id:
	  config the PRJ as per the program
  ** [[Eligibility App URL]]: (Configure the link only if the application is VUE-based; otherwise,   leave it blank.)
	 QA: https://static-qa.clearesult.io/components/general/product-recommendation-assessment-app.min.js
	 PROD: [https://static.clearesult.com/components/general/product-recommendation-assessment-app.min.js](https://static.clearesult.com/components/general/product-recommendation-assessment-app.min.js "https://static.clearesult.com/components/general/product-recommendation-assessment-app.min.js")	  

---
# Attributes:
 ** [[Measure Config JSON]]: Config the json as required
 ** Inventory Service: "none" (if 'Buy Now' product)
 ** [[Project Type]]: Set as required
 ** [[Device Manufacturer]]: Set as required

---
# Amazon Product Identifier: 
** If the Product is Amazon Manufacture then add the Unique product identifier, which should be the SKU of the same product. ([[Amazon Integration setup]])![[Pasted image 20250122190434.png]]

---
# Note: 
** Always try to update the Product level config under store view scope.	![[Screenshot 2025-01-24 195200 4.png]]

---