Mobile App Developer Document
1. Homepage
1.1 Banners from API
The homepage will display banners retrieved from an API. These banners will be dynamically loaded and displayed in a carousel or slider format.

API Endpoint:

```bash
GET /api/banners
```
Response Example:

```json
{
  "banners": [
    {
      "id": 1,
      "image_url": "https://example.com/banner1.jpg",
      "image_url": "https://example.com/banner1.jpg",
      "image_url": "https://example.com/banner1.jpg",
      "image_url": "https://example.com/banner1.jpg",
      "image_url": "https://example.com/banner1.jpg",
    },
  ]
}
```

1.2 Product Categorization
Products on the homepage will be categorized based on the is_new and is_featured variables.

API Endpoint:
```
GET /api/products?category=new
```
```bash
GET /api/products?category=featured
```

2. Product Detail Screen

2.1 Display Product Information
The product detail screen will provide detailed information about the selected product.

API Endpoint:

```bash
GET /api/products/{product_id}
```
Response Example:

```json
{
  "item_code": "ABC123",
  "item_name": "Product Name",
  "item_group": "Group Name",
  "type": "Category",
  "sub_type": "Subcategory",
  "brand": "Brand Name",
  "collection": "Collection Name",
  "super_type": "Super Type",
  "weight": "500g",
  "net_weight": "480g",
  "color_quality": "High",
  "item_size": "Medium",
  // Additional product information...
}
```

2.2 Display Product Images
The product detail screen will show images with an option to zoom.

2.3 Display Item Components
Item components will be displayed in a grid format with columns like item_code, attributes, pcs, and weight.

API Endpoint:
```bash
GET /api/products/{product_id}/components
```
Response Example:
```json
{
  "components": [
    {
      "item_code": "COMP001",
      "attributes": "Attribute 1",
      "pcs": 5,
      "weight": "200g"
    },
    // Additional components...
  ]
}
```

3. Search Page Overview
The search page allows users to search for items using various filters, including item code and specific attributes like item_group, type, sub_type, brand, collection, super_type, weight range, and diamond weight range. The page leverages the items API with dynamically selected variables to fetch filtered data.

4. Search Functionality
4.1 Search by Item Code
Allow users to input the item code directly to retrieve a specific item.

  4.2 Filter Options
Provide a user-friendly interface for users to select filters for refining their search. The available filters include:
```
item_group
type
sub_type
brand
collection
super_type
weight range
diamond weight range
```

  4.3 Items API Endpoint
The search page will utilize the existing items API for fetching filtered data based on user-selected variables.

API Endpoint:
```bash
GET /api/items?item_code={item_code}&item_group={item_group}&type={type}&sub_type={sub_type}&brand={brand}&collection={collection}&super_type={super_type}&min_weight={min_weight}&max_weight={max_weight}&min_diamond_weight={min_diamond_weight}&max_diamond_weight={max_diamond_weight}

```
Example Request:
```bash
GET /api/items?item_code=ABC123&type=Necklace&brand=BrandXYZ&min_weight=200g&max_weight=500g&min_diamond_weight=0.5ct&max_diamond_weight=2ct
```

Example Response:
```json
{
  "items": [
    {
      "item_code": "ABC123",
      "item_name": "Product Name",
      "item_group": "Group Name",
      "type": "Necklace",
      "sub_type": "Pendant",
      "brand": "BrandXYZ",
      "collection": "Collection Name",
      "super_type": "Premium",
      "weight": "300g",
      "diamond_weight": "1.2ct",
      // Additional item information...
    },
    // Additional items...
  ]
}
```
4.4 User Interface
Implement an intuitive user interface that allows users to easily input search criteria, view applied filters, and see the search results.
