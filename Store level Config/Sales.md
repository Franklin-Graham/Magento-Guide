
Go to - Stores -> Configuration -> select website scope -> SALES -> Atlas Abandoned Carts
## Atlas Abandoned Carts:
Customer reminder email, when the product added to Cart and it was not placed
- Enable the module
	![[Pasted image 20250131170338.png]]
- Set time interval by using 'Send After' option
  ![[Pasted image 20250131170630.png]]
---
## Sales Emails:
Go to - Stores -> Configuration -> select website scope -> SALES -> Sales Emails
- Order:
  leave as default ![[Pasted image 20250131163635.png]]

- Order Comments:
	Configure the order update Email
	  ![[Pasted image 20250131163813.png]]

  - Shipment:
     Configure the Shipment Email
      ![[Pasted image 20250131164346.png]]
      
- Credit Memo:
    Configure the credit memo Email
    ![[Pasted image 20250131164715.png]]
---
## TAX:
Go to - Stores -> Configuration -> select website scope -> SALES -> Tax
Avalara Tax:
- Extension mode : leave default
  ![[Pasted image 20250203145451.png]]
- Sales Tax:
  Tax mode: Estimate Tax (QA Environment)
  ![[Pasted image 20250203150136.png]]
  Tax mode: Estimate Tax & Submit Transaction to AvaTax (default) -> Enable only when the product is LIVE
  ![[Pasted image 20250203150223.png]]
  Taxable Countries: Configure the required country
  ![[Pasted image 20250203150406.png]]
  *leave other as default
- Address Validation:
  *leave as default
- VAT: default
- Cross-Border: default
- Exemption Certificate Management: default
- Error, Logs and Queue: default
- Advance: default
- AvaTax - General:
	Use Original Amount for Tax Calculation: Yes
		![[Pasted image 20250203150902.png]]
- Tax Classes: default
- Calculation Settings:
  Tax Calculation Method Based On: Unit Price
  Tax Calculation Based On: Default
  Catalog Prices: Excluding Tax
  other settings: leave as default
- Default Tax Destination Calculation: leave as default
- Price Display Setting
  Display Product Prices in catalog: Excluding Tax
  Display Shipping Prices: Excluding Tax
  ![[Pasted image 20250203151416.png]]
- Shopping Cart Display Settings: (Cart page Tax setting)
  Display Prices: Excluding Tax
  Display Subtotal: Excluding Tax
  Display Shipping Amount: Excluding Tax
  Include Tax in Order Total: Yes
  Additionally Show Order Total Excl. Tax: No
  Display Full Tax Summary: Yes
  Display Zero Tax Subtotal: No
  ![[Pasted image 20250203151610.png]]
- Orders, Invoices, Credit Memos Display Settings:
  Display Prices: Excluding Tax
  Display Subtotal: Excluding Tax
  Display Shipping Amount: Excluding Tax
  Additionally Show Order Total Without Tax: Yes
  Display Full Tax Summary: Yes
  Display Zero Tax Subtotal: No
  ![[Pasted image 20250203151804.png]]
- Fixed Product Taxes: 
  Enable FPT: No (default)
  ![[Pasted image 20250203151853.png]]
---
## Checkout:
Go to - Stores -> Configuration -> select website scope -> SALES -> Checkout
- Checkout Option: configure as below image
	![[Pasted image 20250203153638.png]]
- Shopping Cart: 
  Grouped Product Image: Product Thumbnail Itself
  Configurable Product Image: Parent Product Thumbnail
  Continue Shopping Button URL Path: Continue Shopping Button URL Path to be added after base URL.
  *Leave other as default*
  ![[Pasted image 20250203154027.png]]
- Restrict Add to Cart for Service Products: 
  Enable: Yes/No (to restrict in Cart)
  ![[Pasted image 20250203154212.png]]
- Restrict Shipping Address Editing At Checkout: This will allow customer to Edit the Address in My Account page in the portal  ![[Pasted image 20250203154246.png]]
- *Leave other as Default*


---
  
## Delivery Methods:
Go to - Stores -> Configuration -> select website scope -> SALES -> Delivery Methods
- Flat Rate: 
  Enable : No
- Free Shipping:
  Enable: No
- Table rates
  Enable: Yes
  Title: As Required
  Method Name: As Required
  Condition: Select the condition based on shipping requirement
  Include Virtual Products in Price Calculation: Yes
  Import: import the Xcel file
  for Eg:  If the condition is "price vs destination" the details of Xcel should contain Country, Region/State, Zip/Postal Code, Order Subtotal (and above), Shipping Price
  ![[Pasted image 20250203155253.png]] *In this sheet the price of the product $1 to $34 have a shipping price of $9.99 and price above $35 its free shipping.
* Leave all other config as Default*

---

## Payment Method:
Go to - Stores -> Configuration -> select website scope -> SALES -> Payment Method
Under Stripe Configuration:
- Basic Settings:
  Mode: Test(QA Environment), Live(PROD Environment)
  Live Publishable API Key: Configure the respective API token 
  Live Secret API Key: Configure the respective API token Key
  ![[Pasted image 20250203160002.png]]
- Card Payment:
  Enabled: Yes
  Title : As Required
  Save Customer Cards: Save without asking
  *leave other as Default*
  ![[Pasted image 20250203160159.png]]
  
- *other settings Leave default*

---

## Success Page: 
This is the configuration to show the block after the order placement in the portal
Go to - Stores -> Configuration -> select website scope -> SALES ->success Page
Configuration:
- Continue Button Label: As Required 
- Gratitude Text Inside Image: As Required
- Gratitude Text: As Required
- Info Text: As Required
- Banner image: update the image as required