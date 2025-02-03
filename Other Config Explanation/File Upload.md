### **Magento Setup Guide for Image and File Upload (Media Gallery)**

#### **Accessing the Media Gallery**

1. **Navigate to the Media Gallery:**
    
    - Go to **Magento Admin Panel**
    - Click on **Content** → **Media Gallery**
2. **Uploading Images & Files:**
    
    - Click the **Upload** button
    - Select the image or file from your local system
    - Magento will store the media files in **pub/media** directory

#### **Using Uploaded Images in Magento**

##### **1. For Product Images:**

- Navigate to **Catalog** → **Products** → Select a Product
- Under **Images and Videos**, click **Add Image**
- Select an image from the **Media Gallery** or upload a new one

##### **2. For CMS Pages and Blocks:**

- Go to **Content** → **Pages** or **Blocks**
- Edit the page/block and use the **Insert Image** option
- Choose an image from the **Media Gallery**

##### **3. Using Image Path in Code (HTML):**
- For CMS blocks/pages:
    `<img src="{{media url='wysiwyg/sample.jpg'}}" alt="CMS Image">`