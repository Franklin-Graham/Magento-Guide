The Shipment info should be synced back to Magento (as we are doing with Legacy fulfillment vendors) AND The system should automatically update the order status to 'Complete' once the ordered quantity is shipped.

## Configuration for Syncing Shipment Information from Amazon to Magento**

 This feature allows you to synchronize shipment information from Amazon to Magento  

 To add this feature it was necessary:  

- Add the Order Details operation as a service in the Atlas_AmazonBusiness module  

- Add the Helper that allows it to create the Shipment for the Order based on the response from the Order Details service  

- Add the cron job to automatically run the Order Details service and create the shipment for the order  

## **What do I need to do?**  

_Order Details Service_  

Go to Magento admin > STORES > Settings: Configuration > Scope: Default or Website > AMAZON BUSINESS: Ordering API > Order Details Service  

Enable**
- Description: this field allows you to enable or disable the Order Details service
- Options: Yes, No
- Default: No

API URI**
- Description: the following fields are used to establish the API REST connection with the Amazon Business Order Details service
- Method:
- Description: Defines the HTTP method used for the Order Details service
- Options: GET, POST, PUT
- Default: GET

Endpoint **
- Description: Defines the endpoint used for the Order Details service
- Default: This field depends on the option configured in Magento Admin > STORES > Settings: Configuration > AMAZON BUSINESS > General Config > Scope: Website > General > Store Located.

Path**
- Description: Defines the path used for the Order Details service
- Default: /ordering/2022-10-30/orders/{externalId}

- Header: x-amz-user-email:

- Description: The email address of the customer requesting this resource.
- Default: atlas.platform@clearesult.com
![[Pasted image 20250129152333.png]]

  

_Cron Job_  

Go to Magento admin > STORES > Settings: Configuration > Scope: Default or Website > AMAZON BUSINESS: Sales Config > Sales Shipments > Cron Settings  

Enable**
- Description: this field allows you to enable or disable the Cron Job
- Options: Yes, No
- Default: No

Schedule**
- Description: this field allows you to schedule the cron job
- Default: 0 0 * * *

Attempts**
- Description: Number of times it will try to get a response from Order Details Service for the same order
- Default: 10
![[Pasted image 20250129152406.png]]
  

Shipment**
Go to Magento admin > STORES > Settings: Configuration > Scope: Default or Website > AMAZON BUSINESS: Sales Config > Sales Shipments > Shipment Settings  

Notify**
- Description: this field allows you to establish whether or not the notification is sent to the customer via email when the shipment is created
- Options: Yes, No
- Default: Yes

Append Comment**
- Description: this field allows you to establish whether or not a custom comment is added to the created shipment
- Options: Yes, No
- Default: Yes

Comment**
- Description: this field allows you to define the comment for the shipment
- Default: Your order has shipped

- Is Comment Visible on Storefront

- Description: this field allows you to establish whether the comment is visible in the storefront. It also depends on the theme the store uses.
- Options: Yes, No
- Default: Yes

![[Pasted image 20250129152433.png]]
