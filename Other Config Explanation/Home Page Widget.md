By doing this setup, we can enable product tiles on Home page
![[Pasted image 20250206150458.png]]

How to setup?
- Content -> Pages -> Create or Edit a Home page 
- Click 'Insert Widget' from the top menu. (Before that, place the cursor where you want to insert the widget.)
  ![[Pasted image 20250206150714.png]]
  Setup the settings as below or as required: 
  ![[Pasted image 20250206151407.png]]
  
  Are use this below code instead of Widget setting by changing few changes:
	  products_count: number of products to display
	  value: set the SKU as required
		  
	 <p>{{widget type="Magento\CatalogWidget\Block\Product\ProductsList" show_pager="0" products_count="3" template="Magento_CatalogWidget::product/widget/content/grid.phtml" conditions_encoded="^[`1`:^[`type`:`Magento||CatalogWidget||Model||Rule||Condition||Combine`,`aggregator`:`all`,`value`:`1`,`new_child`:``^],`1--1`:^[`type`:`Magento||CatalogWidget||Model||Rule||Condition||Product`,`attribute`:`sku`,`operator`:`()`,`value`:`CONF-GNT,CONF-STST,CONF-GNLT`^]^]"}}</p>
		  