Magento allows you to manage multiple websites, stores, and store views from a single admin panel. The "All Stores" section in Magento lets you configure and organize these entities efficiently.
## **1️⃣ Navigate to "All Stores"**

1. **Log in** to your Magento Admin Panel.
2. Go to **Stores** > **Settings** > **All Stores**.
3. You will see a list of all existing **Websites, Stores, and Store Views**.

---

## **2️⃣ Understanding Magento Store Hierarchy**

Magento has a **4-level structure**:

### **1️⃣ Global** - The top level that applies to all stores.

### **2️⃣ Website** - Represents a separate business entity (e.g., different domains).

### **3️⃣ Store** - A website can have multiple stores, each with unique categories.

### **4️⃣ Store View** - Different store views can be used for different languages or themes.

---

## **3️⃣ Add a New Website**

1. Click **Create Website**.
2. Fill in the details:
    - **Name**: Enter a name for the website.
    - **Code**: Unique identifier (The store code will provided during requirement).
	    Eg:![[Pasted image 20250130205225.png]]
    - **Sort Order**: Set the order in the admin panel.
3. Click **Save Website**.

---

## **4️⃣ Add a New Store**

1. Click **Create Store**.
2. Fill in the details:
    - **Website**: Select the parent website.
    - **Name**: Enter a store name.
    - Code: Unique identifier(The store code will provided during requirement)
    - **Root Category**: Choose a category for this store.
	    ![[Pasted image 20250130213156.png]]
3. Click **Save Store**.

---

## **5️⃣ Add a New Store View**

1. Click **Create Store View**.
2. Fill in the details:
    - **Store**: Select the store it belongs to.
    - **Name**: Enter a name 
    - **Code**: Unique identifier(instead of 'main' replace with 'view' Eg: view_entergytx).
    - **Status**: Choose **Enabled**.
    - **Sort Order**: Defines display order in the admin panel.
3. Click **Save Store View**.
		![[Pasted image 20250130213305.png]]

---

## **6️⃣ Assign a Store View to a Domain**

If you have multiple store views (e.g., for different languages), update the **Base URL**:

1. Go to **Stores** > **Configuration**.
2. Under **General**, select **Web**.
3. Change **Scope** (top-left dropdown) to the store view you want to edit.
4. Expand **Base URLs** and update the URL.
5. Click **Save Config** and **Flush Cache**.

---

## **7️⃣ Verify the Store Setup**

1. Open a new browser and enter the store URL.
2. Ensure the correct store view loads.