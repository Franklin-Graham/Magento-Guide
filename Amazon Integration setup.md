This setup needs to be configured if Amazon products are within the scope.

How to Configure:
STORES -> Configuration -> select website scope -> AMAZON BUSINESS

** General Config **
	*mode: should be set to Sandbox during testing and only enabled when the product goes live.![[Pasted image 20250124011241.png]]
	*Leave the other settings at their default values.
** Product Search API **
		Enable the 'Search For Offers Of A Specific Product Service'
		 ![[Pasted image 20250124011907.png]]
		*Leave the other settings at their default values.
** Ordering API **
		* Enable the 'Place Order Service'
		 ![[Pasted image 20250124012130.png]]
		* Set Trial Mode to "Yes" only when the program goes live.
		 ![[Pasted image 20250124012249.png]]
		*Leave the other settings at their default values.
** Sales Config **
		 * Leave the settings at their default values.
		   
Other Notes **
		* Ensure that the 'Unique Identifier Code' is added for Amazon products under the product-level configuration (the code should be the SKU of the specific product). This setting falls under the product-level configuration.![[Pasted image 20250124012922.png]]
		 