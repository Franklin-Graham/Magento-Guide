### **Magento Configurable Product Setup Guide**

A **Configurable Product** in Magento allows customers to choose options (e.g., color) while managing inventory separately for each variation.

---

### **Step 1: Navigate to Product Creation**

1. **Go to Admin Panel** → **Catalog** → **Products**
2. Click **Add Product** → Select **Configurable Product**

---

### **Step 2: Fill in Basic Product Details**

- **Product Name**: Enter the product title
- **SKU**: Set a unique identifier (e.g., `smartThermostat-Config`)
- **Price**: Leave blank (each variation will have its own price)
- **Tax Class**: Select applicable tax
- **Stock Status**: Choose **In Stock**
- **Categories**: Assign to relevant category
- **Description & Short Description**: Add product details

---

### **Step 3: Configure Attributes (Variations)**

1. **Scroll to the "Configurations" section** → Click **Create Configurations**
2. Select the attribute(s) (e.g., **Color, Size**)
    - If missing, create new attributes under **Stores → Attributes → Product**
      [[Visual Swatch Color]]
3. Choose available values (e.g., Red, Blue, silver)

---

### **Step 4: Generate Variations**

1. Click **Next**, Magento will generate individual **Simple Products**
2. Assign:
    - **Images** (Use same or different per variation)
    - **Prices** (Set different prices if needed)
    - **Inventory** (Each variant has its own stock)
3. Click **Next** and **Generate Products**