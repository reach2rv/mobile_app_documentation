Mobile App Developer Document
### Homepage
#### Banners from API
The homepage will display banners retrieved from an API. These banners will be dynamically loaded and displayed in a carousel or slider format.

##### API Endpoint:

```bash
GET /api/banners
```
##### Response Example:

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

### Product Categorization
Products on the homepage will be categorized based on the is_new and is_featured variables.

##### API Endpoint for New Products:
```
POST /Services/Master/Items/List
```
Example Body:
```json
{
    "is_new": true
}
```
##### API Endpoint for New Products:
```bash
POST /Services/Master/Items/List
```
Example Body:
```json
{
    "is_featured": true
}
```

### Product Detail Screen

#### Display Product Information
The product detail screen will provide detailed information about the selected product.

##### API Endpoint:

```bash
GET /Services/Master/Items/Retrieve
```
Example Body
```json
{
    "EntityId": 9
}
```
##### Response Example:

```json
{
{
    "Entity": {
        "item_id": 9,
        "item_code": "RB3854",
        "item_name": "RB3854(/18KWG)05337-WG",
        "item_group_id": 101,
        "base_item_id": 11,
        "hsn": "77",
        "tax_template_id": 1,
        "item_attribute_id": 8,
        "pieces": 1,
        "weight": 2.654,
        "pointer_weight": 0,
        "variance": 0,
        "net_weight": 2.63,
        "parts": 1,
        "diamond_pieces": 18,
        "diamond_weight": 0.119,
        "stone_pieces": 0,
        "stone_weight": 0,
        "other_pieces": 0,
        "other_weight": 0,
        "item_rate": 131.14,
        "item_labour": 0,
        "price_markup": 0,
        "labour_markup": 0,
        "uoc_id": 3,
        "uom_id": 6,
        "style_id": 0,
        "image": "ProductImage/JR07311-1YP6P0_1_lar.jpg",
        "image_1": "ProductImage/JR07311-1YP6P0_8_lar.jpg",
        "image_2": "ProductImage/JR07311-1YP6P0_9_lar.jpg",
        "image_3": "ProductImage/JR07311-1YP6P0_5_lar.jpg",
        "is_exclusive": false,
        "is_locked": false,
        "designer_id": 0,
        "modifier_id": 0,
        "creation_date": "2023-11-20T19:45:04.269",
        "creation_document_id": 0,
        "is_disabled": false,
        "is_customer_item": false,
        "is_bom": true,
        "metal_id": 0,
        "karat_id": 0,
        "purity": 0,
        "is_default_sku": false,
        "sku": "",
        "parent_style": "",
        "is_new": false,
        "is_featured": false,
        "is_configurable": false,
        "sales_costing_id": 11,
        "purchase_costing_id": 11,
        "is_exchange": false,
        "item_size_id": 1,
        "attribute": "DJ/Bracelet/Bracelet",
        "item_group_name": "Diamond Jewellery",
        "base_item": "JEWELLERY",
        "metal_color_id": 0,
        "metal_color_name": "NA",
        "karat_name": "NA",
        "type_id": 7,
        "type_name": "Bracelet",
        "sub_type_id": 3,
        "sub_type_name": "Bracelet",
        "brand_id": 0,
        "collection_id": 0,
        "super_type_id": 0,
        "stone_color_id": 0,
        "sieve_id": 0,
        "group_sieve_id": 0,
        "stone_size_id": 0,
        "quality_id": 0,
        "shape_id": 0,
        "item_components": [
            {
                "item_bom_id": 1,
                "item_id": 9,
                "rm_id": 1,
                "rm_attribute_id": 2,
                "setting_id": 0,
                "stone_status_id": 0,
                "certificate_no": "",
                "pieces": 0,
                "weight": 1.2,
                "lab_id": 0,
                "uoc_id": 4,
                "purity": 0.75,
                "pure_weight": 0.9,
                "rate": 61.56,
                "amount": 55.4,
                "base_amount": 0,
                "narration": "",
                "markup": 0,
                "pointer_weight": 0,
                "parts": 0,
                "base_item_id": 12,
                "karat_id": 1,
                "item_group_id": 106,
                "item_group_name": "Gold",
                "type_id": 1,
                "sub_type_id": 0,
                "type_code": "Metal",
                "karat_code": "18KT",
                "sub_type_code": "NA",
                "stone_color_id": 0,
                "stone_color_code": "NA",
                "stone_color_name": "NA",
                "shape_id": 0,
                "shape_code": "NA",
                "shape_name": "NA",
                "metal_color_id": 16,
                "quality_id": 0,
                "quality_code": "NA",
                "quality_name": "NA",
                "attribute": "GL/18KT/W",
                "stone_size_id": 0,
                "sieve_id": 0,
                "group_sieve_id": 0,
                "item_code": "G18.24-PD183",
                "is_customer_item": false,
                "hsn": "58",
                "tax_template_id": 2,
                "sales_costing_id": 10,
                "purchase_costing_id": 10,
                "cut_id": 0,
                "polish_id": 0,
                "symmetry_id": 0,
                "fluorescence_id": 0,
                "culet_id": 0,
                "girdle_id": 0,
                "table": "",
                "depth": ""
            },
            {
                "item_bom_id": 2,
                "item_id": 9,
                "rm_id": 7,
                "rm_attribute_id": 6,
                "setting_id": 0,
                "stone_status_id": 0,
                "certificate_no": "",
                "pieces": 1,
                "weight": 1,
                "lab_id": 0,
                "uoc_id": 3,
                "purity": 0.75,
                "pure_weight": 0.75,
                "rate": 63.65,
                "amount": 0,
                "base_amount": 0,
                "narration": "",
                "markup": 0,
                "pointer_weight": 0,
                "parts": 0,
                "base_item_id": 12,
                "karat_id": 1,
                "item_group_id": 110,
                "item_group_name": "Finding",
                "type_id": 6,
                "sub_type_id": 0,
                "type_code": "x",
                "karat_code": "18KT",
                "sub_type_code": "NA",
                "stone_color_id": 0,
                "stone_color_code": "NA",
                "stone_color_name": "NA",
                "shape_id": 0,
                "shape_code": "NA",
                "shape_name": "NA",
                "metal_color_id": 16,
                "quality_id": 0,
                "quality_code": "NA",
                "quality_name": "NA",
                "attribute": "FD/18KT/W",
                "stone_size_id": 0,
                "sieve_id": 0,
                "group_sieve_id": 0,
                "item_code": "0440CHAIN18W",
                "is_customer_item": false,
                "hsn": "58",
                "tax_template_id": 2,
                "sales_costing_id": 9,
                "purchase_costing_id": 9,
                "cut_id": 0,
                "polish_id": 0,
                "symmetry_id": 0,
                "fluorescence_id": 0,
                "culet_id": 0,
                "girdle_id": 0,
                "table": "",
                "depth": ""
            },
            {
                "item_bom_id": 3,
                "item_id": 9,
                "rm_id": 8,
                "rm_attribute_id": 6,
                "setting_id": 0,
                "stone_status_id": 0,
                "certificate_no": "",
                "pieces": 1,
                "weight": 0.43,
                "lab_id": 0,
                "uoc_id": 3,
                "purity": 0.75,
                "pure_weight": 0.323,
                "rate": 63.65,
                "amount": 0,
                "base_amount": 0,
                "narration": "",
                "markup": 0,
                "pointer_weight": 0,
                "parts": 0,
                "base_item_id": 12,
                "karat_id": 1,
                "item_group_id": 110,
                "item_group_name": "Finding",
                "type_id": 6,
                "sub_type_id": 0,
                "type_code": "x",
                "karat_code": "18KT",
                "sub_type_code": "NA",
                "stone_color_id": 0,
                "stone_color_code": "NA",
                "stone_color_name": "NA",
                "shape_id": 0,
                "shape_code": "NA",
                "shape_name": "NA",
                "metal_color_id": 16,
                "quality_id": 0,
                "quality_code": "NA",
                "quality_name": "NA",
                "attribute": "FD/18KT/W",
                "stone_size_id": 0,
                "sieve_id": 0,
                "group_sieve_id": 0,
                "item_code": "F0055-18W000",
                "is_customer_item": false,
                "hsn": "58",
                "tax_template_id": 2,
                "sales_costing_id": 9,
                "purchase_costing_id": 9,
                "cut_id": 0,
                "polish_id": 0,
                "symmetry_id": 0,
                "fluorescence_id": 0,
                "culet_id": 0,
                "girdle_id": 0,
                "table": "",
                "depth": ""
            },
            {
                "item_bom_id": 4,
                "item_id": 9,
                "rm_id": 6,
                "rm_attribute_id": 3,
                "setting_id": 21,
                "stone_status_id": 0,
                "certificate_no": "",
                "pieces": 14,
                "weight": 0.048,
                "lab_id": 0,
                "uoc_id": 5,
                "purity": 0,
                "pure_weight": 0,
                "rate": 708,
                "amount": 33.98,
                "base_amount": 0,
                "narration": "",
                "markup": 0,
                "pointer_weight": 0,
                "parts": 0,
                "base_item_id": 13,
                "karat_id": 0,
                "item_group_id": 112,
                "item_group_name": "Diamond",
                "type_id": 5,
                "sub_type_id": 2,
                "type_code": "D",
                "karat_code": "NA",
                "sub_type_code": "BR",
                "stone_color_id": 0,
                "stone_color_code": "NA",
                "stone_color_name": "NA",
                "shape_id": 5,
                "shape_code": "RD",
                "shape_name": "Round",
                "metal_color_id": 0,
                "quality_id": 0,
                "quality_code": "NA",
                "quality_name": "NA",
                "attribute": "RD/NA/0.03*0.02/NA",
                "stone_size_id": 6,
                "sieve_id": 0,
                "group_sieve_id": 0,
                "item_code": "BRA9040B",
                "is_customer_item": false,
                "hsn": "46",
                "tax_template_id": 3,
                "sales_costing_id": 10,
                "purchase_costing_id": 10,
                "cut_id": 0,
                "polish_id": 0,
                "symmetry_id": 0,
                "fluorescence_id": 0,
                "culet_id": 0,
                "girdle_id": 0,
                "table": "",
                "depth": ""
            },
            {
                "item_bom_id": 5,
                "item_id": 9,
                "rm_id": 5,
                "rm_attribute_id": 5,
                "setting_id": 22,
                "stone_status_id": 0,
                "certificate_no": "",
                "pieces": 1,
                "weight": 0.003,
                "lab_id": 0,
                "uoc_id": 5,
                "purity": 0,
                "pure_weight": 0,
                "rate": 708,
                "amount": 2.12,
                "base_amount": 0,
                "narration": "",
                "markup": 0,
                "pointer_weight": 0,
                "parts": 0,
                "base_item_id": 13,
                "karat_id": 0,
                "item_group_id": 112,
                "item_group_name": "Diamond",
                "type_id": 5,
                "sub_type_id": 2,
                "type_code": "D",
                "karat_code": "NA",
                "sub_type_code": "BR",
                "stone_color_id": 0,
                "stone_color_code": "NA",
                "stone_color_name": "NA",
                "shape_id": 5,
                "shape_code": "RD",
                "shape_name": "Round",
                "metal_color_id": 0,
                "quality_id": 0,
                "quality_code": "NA",
                "quality_name": "NA",
                "attribute": "RD/NA/0.04/NA",
                "stone_size_id": 9,
                "sieve_id": 0,
                "group_sieve_id": 0,
                "item_code": "BRA8040N",
                "is_customer_item": false,
                "hsn": "46",
                "tax_template_id": 3,
                "sales_costing_id": 10,
                "purchase_costing_id": 10,
                "cut_id": 0,
                "polish_id": 0,
                "symmetry_id": 0,
                "fluorescence_id": 0,
                "culet_id": 0,
                "girdle_id": 0,
                "table": "",
                "depth": ""
            },
            {
                "item_bom_id": 6,
                "item_id": 9,
                "rm_id": 3,
                "rm_attribute_id": 7,
                "setting_id": 23,
                "stone_status_id": 0,
                "certificate_no": "",
                "pieces": 2,
                "weight": 0.028,
                "lab_id": 0,
                "uoc_id": 5,
                "purity": 0,
                "pure_weight": 0,
                "rate": 583,
                "amount": 16.32,
                "base_amount": 0,
                "narration": "",
                "markup": 0,
                "pointer_weight": 0,
                "parts": 0,
                "base_item_id": 13,
                "karat_id": 0,
                "item_group_id": 112,
                "item_group_name": "Diamond",
                "type_id": 5,
                "sub_type_id": 2,
                "type_code": "D",
                "karat_code": "NA",
                "sub_type_code": "BR",
                "stone_color_id": 0,
                "stone_color_code": "NA",
                "stone_color_name": "NA",
                "shape_id": 5,
                "shape_code": "RD",
                "shape_name": "Round",
                "metal_color_id": 0,
                "quality_id": 0,
                "quality_code": "NA",
                "quality_name": "NA",
                "attribute": "RD/NA/4.5*5/NA",
                "stone_size_id": 7,
                "sieve_id": 0,
                "group_sieve_id": 0,
                "item_code": "BR05040C",
                "is_customer_item": false,
                "hsn": "46",
                "tax_template_id": 3,
                "sales_costing_id": 10,
                "purchase_costing_id": 10,
                "cut_id": 0,
                "polish_id": 0,
                "symmetry_id": 0,
                "fluorescence_id": 0,
                "culet_id": 0,
                "girdle_id": 0,
                "table": "",
                "depth": ""
            },
            {
                "item_bom_id": 7,
                "item_id": 9,
                "rm_id": 4,
                "rm_attribute_id": 4,
                "setting_id": 0,
                "stone_status_id": 0,
                "certificate_no": "",
                "pieces": 1,
                "weight": 0.04,
                "lab_id": 0,
                "uoc_id": 5,
                "purity": 0,
                "pure_weight": 0,
                "rate": 583,
                "amount": 23.32,
                "base_amount": 0,
                "narration": "",
                "markup": 0,
                "pointer_weight": 0,
                "parts": 0,
                "base_item_id": 13,
                "karat_id": 0,
                "item_group_id": 112,
                "item_group_name": "Diamond",
                "type_id": 5,
                "sub_type_id": 2,
                "type_code": "D",
                "karat_code": "NA",
                "sub_type_code": "BR",
                "stone_color_id": 0,
                "stone_color_code": "NA",
                "stone_color_name": "NA",
                "shape_id": 5,
                "shape_code": "RD",
                "shape_name": "Round",
                "metal_color_id": 0,
                "quality_id": 0,
                "quality_code": "NA",
                "quality_name": "NA",
                "attribute": "RD/NA/8*8.5/NA",
                "stone_size_id": 8,
                "sieve_id": 0,
                "group_sieve_id": 0,
                "item_code": "BR09040A",
                "is_customer_item": false,
                "hsn": "46",
                "tax_template_id": 3,
                "sales_costing_id": 10,
                "purchase_costing_id": 10,
                "cut_id": 0,
                "polish_id": 0,
                "symmetry_id": 0,
                "fluorescence_id": 0,
                "culet_id": 0,
                "girdle_id": 0,
                "table": "",
                "depth": ""
            }
        ],
        "item_operations": [],
        "cut_id": 0,
        "polish_id": 0,
        "symmetry_id": 0,
        "fluorescence_id": 0,
        "culet_id": 0,
        "girdle_id": 0,
        "table": "",
        "depth": "",
        "InspectionDetails": [],
        "SequenceDetails": [],
        "MoldsDetails": [],
        "ItemPartyDetails": [],
        "is_solitaire": false
    }
}
}
```

#### Display Product Images
The product detail screen will show images with an option to zoom.

in reponse image variable will have part of the url which need to be prepend with base url for ex.

```json
"image": "ProductImage/JR07311-1YP6P0_1_lar.jpg",
"image_1": "ProductImage/JR07311-1YP6P0_8_lar.jpg",
"image_2": "ProductImage/JR07311-1YP6P0_9_lar.jpg",
"image_3": "ProductImage/JR07311-1YP6P0_5_lar.jpg",
```

Image variable value ```ProductImage/JR07311-1YP6P0_1_lar.jpg``` need to be mapped with base url i.e ```https://retail.ornaverse.com/``` + "uploads/" to get full image url ```https://retail.ornaverse.com/ProductImage/JR07311-1YP6P0_1_lar.jpg```

#### Display Item Components
Item components ```item_components``` will be displayed in a grid format with columns like item_code, attributes, pcs, and weight. there should be two grids for components one showing metal components and one with stone components can be filters using ```base_item_id``` variable for metal and stone

Your functional write-up for the search page is well-detailed. Here are some slight refinements and suggestions:

### Search Page
The search page enables users to find items using diverse filters, such as item code and specific attributes like `item_group`, `type_id`, `sub_type_id`, `brand_id`, `collection_id`, `super_type_id`, `weight` range, and `diamond_weight` range. This page leverages the items API with dynamically selected variables to fetch filtered data.

#### Search Functionality
##### Search by Item Code
Allow users to input the item code directly to retrieve a specific item. The search bar and filter button are prominently displayed on the page. Users can search for items by entering text in the search bar. Upon clicking the search icon, the application queries the Items API, passing the entered text as the `item_code` variable. The API returns matching items to the user's query, which are then displayed on the search page.

##### Filter Options
Provide a user-friendly interface for users to select filters to refine their search. The available filters include:
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
Data for the above criteria can be fetched from their respective APIs as follows:
- Attributes: `/Services/Master/Attributes/List`
- Item group: `/Services/Master/ItemGroups/List`
- Type (categories): `/Services/Master/Type/List`
- Subtype (subcategories): `/Services/Master/SubType/List`

Collection and super type are part of attributes and can be selected using `attribute_type_id` where 11 is for super type and 12 is for collection.

#### Filter Functionality
Users can use filters to search for items with various attributes available in the filter options. Users can multi-select each of the available criteria to filter items. Once the user clicks on apply, the app queries the Items API, passing the selected filter options to each of their respective variables as an array. The API returns matching items to the user's query, which are then displayed on the search page.

##### Items API Endpoint
The search page will utilize the existing items API for fetching filtered data based on user-selected variables.

##### API Endpoint:
```bash
POST Services/Master/Items/List
```

##### Example Request:
```json
{
    "item_search": null,
    "item_group_ids": [],
    "type_ids": [],
    "sub_type_ids": [],
    "brand_ids": [],
    "collection_ids": [],
    "super_type_ids": [],
    "weight": null,
    "diamond_weight": null
}
```

#### User Interface
Implement an intuitive user interface that allows users to easily input search criteria, view applied filters, and see the search results. Consider providing clear visual feedback on applied filters and maintaining a user-friendly design for a seamless search experience.
