# Product Accordion Metafield Setup

To use the dynamic accordion feature, you need to create a metafield in your Shopify admin:

## Steps to create the metafield:

1. **Go to Shopify Admin > Settings > Custom data**

2. **Click "Products" and then "Add definition"**

3. **Configure the metafield:**

   - **Name:** `Accordion Items`
   - **Namespace and key:** `custom.accordion_items`
   - **Description:** `Dynamic accordion items for product pages`
   - **Type:** `List of mixed references` or `JSON`

4. **If using JSON type, the structure should be:**

```json
[
  {
    "title": "Size guide",
    "description": "This product comes in multiple sizes. Please refer to our sizing chart for the best fit."
  },
  {
    "title": "Model's size",
    "description": "The model is wearing size S and is 175cm tall."
  },
  {
    "title": "Care guide",
    "description": "Machine wash cold. Do not bleach. Tumble dry low. Iron on low heat."
  }
]
```

5. **Alternative: Create individual metafields for each accordion item:**
   - `custom.accordion_item_1_title` (Single line text)
   - `custom.accordion_item_1_description` (Multi-line text)
   - `custom.accordion_item_2_title` (Single line text)
   - `custom.accordion_item_2_description` (Multi-line text)
   - `custom.accordion_item_3_title` (Single line text)
   - `custom.accordion_item_3_description` (Multi-line text)

## Features:

- ✅ Only shows accordion if metafield has content
- ✅ Empty title/description pairs are automatically hidden
- ✅ Configure single vs multiple open items via section settings
- ✅ Fully responsive and accessible
- ✅ Smooth animations
