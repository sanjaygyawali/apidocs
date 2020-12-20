# Search for Product in search Bar.

Will fetch the matching content according to search

**URL** : `search`

**Query Params**: `{productName:sample product name}`

**Method** : `GET`

**Auth required** : NO

**Permissions required** : --

## Success Responses

**Code** : `200 OK`

**Condition 1**: when matching products are found.

**Content** : Resp wonse will include list of related products,

```json
{
  "recommendedProducts": [],
  "results": [
    {
      "id": "fdc1dec1-3634-46f1-88dc-9ca966509d28",
      "title": "Sleek Wooden Pizza",
      "image": "http://192.168.0.105:3000/assets/240_F_371723060_P4KpCFjcOQtnLNIv4rU2jf4mW3wUiRBy.jpg"
    },
    {
      "id": "9565634d-64a9-4e63-9ead-d9c6ae8dd94b",
      "title": "Unbranded Concrete Bacon",
      "image": "http://192.168.0.105:3000/assets/240_F_266260297_2uqq8awE8CY9BPQeLiISdDNAe3x53yav.jpg"
    },
    {
      "id": "87fbeb03-9631-406e-8312-5e5f915a7688",
      "title": "Sleek Frozen Fish",
      "image": "http://192.168.0.105:3000/assets/stationery.jpg"
    },
    {
      "id": "cf33acb1-980c-4e36-b232-bbf5cdd97b76",
      "title": "Handcrafted Concrete Computer",
      "image": "http://192.168.0.105:3000/assets/240_F_266260297_2uqq8awE8CY9BPQeLiISdDNAe3x53yav.jpg"
    },
    {
      "id": "66d5c159-6cee-4e7c-80f3-1ec4364646b0",
      "title": "Rustic Steel Gloves",
      "image": "http://192.168.0.105:3000/assets/240_F_275092746_2L89P1BUJRqu9beE6HySTEKJ1ZwBeIgX.jpg"
    },
    {
      "id": "5592b584-3e3d-4183-9a59-d37840dde24e",
      "title": "Licensed Fresh Pizza",
      "image": "http://192.168.0.105:3000/assets/240_F_222184023_JlkYL4hIYVHJkrBPLyeBIoqHO4sqESGO.jpg"
    },
    {
      "id": "cf9f0bcb-b063-45cc-a376-13dffa598e8a",
      "title": "Small Rubber Pizza",
      "image": "http://192.168.0.105:3000/assets/240_F_67781523_mmztUlxrqjESP7OzR6SqwbqjL3MQADvm.jpg"
    },
    {
      "id": "aa78ded8-9eaf-4b87-a4ac-8fcdbecf32bd",
      "title": "Generic Plastic Shoes",
      "image": "http://192.168.0.105:3000/assets/500_F_47418080_eAUAEaiDN9YvTyo5cIMniGFhXLtDGCxl.jpg"
    },
    {
      "id": "72763587-6cf0-4f5b-9017-7b4305f45eb6",
      "title": "Incredible Metal Pizza",
      "image": "http://192.168.0.105:3000/assets/magicmouse.jpg"
    },
    {
      "id": "f22f0338-76a3-4d68-8bc4-10d2fb645c8f",
      "title": "Awesome Concrete Shoes",
      "image": "http://192.168.0.105:3000/assets/laptop-mock-up_1310-197.jpg"
    }
  ]
}
```

**Condition 1**: when matching products are not found.

**Content** : Response will contain some recommended products instead.

```json
{
  "results": [],
  "recommendedProducts": [
    {
      "id": "fdc1dec1-3634-46f1-88dc-9ca966509d28",
      "title": "Sleek Wooden Pizza",
      "image": "http://192.168.0.105:3000/assets/240_F_371723060_P4KpCFjcOQtnLNIv4rU2jf4mW3wUiRBy.jpg"
    },
    {
      "id": "9565634d-64a9-4e63-9ead-d9c6ae8dd94b",
      "title": "Unbranded Concrete Bacon",
      "image": "http://192.168.0.105:3000/assets/240_F_266260297_2uqq8awE8CY9BPQeLiISdDNAe3x53yav.jpg"
    },
    {
      "id": "87fbeb03-9631-406e-8312-5e5f915a7688",
      "title": "Sleek Frozen Fish",
      "image": "http://192.168.0.105:3000/assets/stationery.jpg"
    },
    {
      "id": "cf33acb1-980c-4e36-b232-bbf5cdd97b76",
      "title": "Handcrafted Concrete Computer",
      "image": "http://192.168.0.105:3000/assets/240_F_266260297_2uqq8awE8CY9BPQeLiISdDNAe3x53yav.jpg"
    },
    {
      "id": "66d5c159-6cee-4e7c-80f3-1ec4364646b0",
      "title": "Rustic Steel Gloves",
      "image": "http://192.168.0.105:3000/assets/240_F_275092746_2L89P1BUJRqu9beE6HySTEKJ1ZwBeIgX.jpg"
    },
    {
      "id": "5592b584-3e3d-4183-9a59-d37840dde24e",
      "title": "Licensed Fresh Pizza",
      "image": "http://192.168.0.105:3000/assets/240_F_222184023_JlkYL4hIYVHJkrBPLyeBIoqHO4sqESGO.jpg"
    },
    {
      "id": "cf9f0bcb-b063-45cc-a376-13dffa598e8a",
      "title": "Small Rubber Pizza",
      "image": "http://192.168.0.105:3000/assets/240_F_67781523_mmztUlxrqjESP7OzR6SqwbqjL3MQADvm.jpg"
    },
    {
      "id": "aa78ded8-9eaf-4b87-a4ac-8fcdbecf32bd",
      "title": "Generic Plastic Shoes",
      "image": "http://192.168.0.105:3000/assets/500_F_47418080_eAUAEaiDN9YvTyo5cIMniGFhXLtDGCxl.jpg"
    },
    {
      "id": "72763587-6cf0-4f5b-9017-7b4305f45eb6",
      "title": "Incredible Metal Pizza",
      "image": "http://192.168.0.105:3000/assets/magicmouse.jpg"
    },
    {
      "id": "f22f0338-76a3-4d68-8bc4-10d2fb645c8f",
      "title": "Awesome Concrete Shoes",
      "image": "http://192.168.0.105:3000/assets/laptop-mock-up_1310-197.jpg"
    }
  ]
}
```

# Get all attributes for search.

To fetch all the atriibutes that are required to render the advance filter box in search page.

**URL** : `attribute/search`

**Query Params**:

```json
{
  "searchType": "",
  "searchContent": ""
}
```

**Method** : `GET`

**Auth required** : NO

**Permissions required** : --

## Success Responses

**Code** : `200 OK`

**Condition 1**: when matching products are found.

**Content** : Response will include list of related products,
**Explanation of attribute**: Each object in the response represents the search attribute , range, rating, color and checkbox.

- Range: `g-range` is used for range filter of item.
- Rating: `g-rating-group` is used for rating selection
- Checkbox: `g-filter-search` is used for group of checkbox and the checkbox will be grouped in system.
- Color: this is extension of `g-filter-search` with extra attribute `color:true` should be attached in the object. to show color as well in the selection.

| attribute          | description                                                      |
| ------------------ | ---------------------------------------------------------------- |
| response[i].search | The attribute name by which will search to get options in return |

```json
[
  {
    "label": "Categories",
    "search": "category",
    "componentType": "g-filter-search",
    "placeholder": "Please Enter Category",
    "options": [
      { "value": "53129eea-69a1-4612-be82-12497423ddf8", "label": "Clothing" },
      { "value": "8863b864-cee1-463f-852e-d828b8ba75e2", "label": "Sports" },
      {
        "value": "2566e0cd-e29d-4539-a824-ebb5cfb676b6",
        "label": "Industrial"
      },
      {
        "value": "ccc207be-a0e8-40c8-853e-37242a227fa9",
        "label": "Electronics"
      },
      { "value": "f7303b84-1b54-40b9-8f6e-7cb01a424e56", "label": "Tools" }
    ]
  },
  {
    "label": "Color",
    "placeholder": "Search color",
    "componentType": "g-filter-search",
    "color": true,
    "options": [
      { "label": "magenta", "value": "magenta" },
      { "label": "salmon", "value": "salmon" },
      { "label": "violet", "value": "violet" },
      { "label": "black", "value": "black" },
      { "label": "turquoise", "value": "turquoise" }
    ]
  },
  {
    "label": "Brands",
    "search": "brand",
    "componentType": "g-filter-search",
    "placeholder": "Please Enter Brand",
    "options": [
      {
        "value": "02b85087-9744-403d-a456-ed4a5b9cfa80",
        "label": "Kshlerin - Kuhlman"
      },
      {
        "value": "2f1cc41f-a9f0-4b13-8d58-8c97fe0e2a02",
        "label": "Okuneva, Schamberger and Feest"
      },
      {
        "value": "cc002545-53d2-49d0-ba9e-aec6e69aade3",
        "label": "Mante - Emard"
      },
      {
        "value": "18618b9f-aee3-48d3-a1b0-1294e5d081b5",
        "label": "Purdy and Sons"
      },
      {
        "value": "89d30569-920f-472a-8056-35390c78d5f5",
        "label": "Schimmel - Luettgen"
      }
    ]
  },
  {
    "label": "Range",
    "componentType": "g-range",
    "min": 97,
    "max": 970,
    "prefix": "Npr"
  },
  {
    "label": "Rating",
    "componentType": "g-rating-group",
    "placeholder": "Please Enter Filter Rating"
  }
]
```

# Get all the related product according to search.

Will respond all the product according to the advanceFilter attributes.

**URL** : `products`

**Query Params**:

```json
{
  "page": 1,
  "advanceFilter": {
    "Categories": [
      { "value": "de795fa7-5dd4-4bba-ab0c-e2bc19cac201", "label": "Tools" },
      {
        "value": "4a6e6208-10e4-451c-bce6-b19c742cc7c2",
        "label": "Electronics"
      }
    ],
    "Color": [
      { "label": "cyan", "value": "cyan" },
      { "label": "grey", "value": "grey" },
      { "label": "orange", "value": "orange" },
      { "label": "turquoise", "value": "turquoise" }
    ],
    "Range": { "min": 303, "max": 759 },
    "Rating": 5
  },
  "sortBy": "gm"
}
```

**Method** : `GET`

**Auth required** : NO

**Permissions required** : --

## Success Responses

**Code** : `200 OK`

**Condition 1**: when matching products are found.

**Content** : Response will include list of related products,

```json
{
  "data": [
    {
      "id": "729c5cf9-4ffc-46a3-bbd0-b68baea3704e",
      "title": "Gorgeous Fresh Chair",
      "isOnSale": false,
      "image": "http://192.168.43.112:3000/assets/240_F_106242291_ZOJeEhJg0ohTzXoB2HabeQ0Ogx1t3ibS.jpg",
      "isOnWishList": true,
      "rating": 2,
      "regularPrice": 1021,
      "specialPrice": 223
    },
    {
      "id": "3211fe5b-4d4e-4190-a81f-94757ed08d5c",
      "title": "Unbranded Steel Car",
      "isOnSale": true,
      "image": "http://192.168.43.112:3000/assets/500_F_114765839_LMyN9PBEl9GaHFjztUql0csPkzNtTMsf.jpg",
      "isOnWishList": true,
      "rating": 5,
      "regularPrice": 1170,
      "specialPrice": 390
    },
    {
      "id": "788d427e-ee8d-4274-8655-91781add62c3",
      "title": "Awesome Steel Computer",
      "isOnSale": false,
      "image": "http://192.168.43.112:3000/assets/240_F_338827506_XqavlYfR58OkHhyvi4aNdI1wCoPjW7gu.jpg",
      "isOnWishList": true,
      "rating": 2,
      "regularPrice": 1030,
      "specialPrice": 361
    },
    {
      "id": "53d7d5ad-bace-4d63-98e6-59898e20c559",
      "title": "Sleek Steel Hat",
      "isOnSale": true,
      "image": "http://192.168.43.112:3000/assets/240_F_86542099_bP0359YevWiJ20O7pTrCqOLaYHIuuWGM.jpg",
      "isOnWishList": false,
      "rating": 4,
      "regularPrice": 1329,
      "specialPrice": 509
    },
    {
      "id": "35cbdc1b-8978-4dfc-ac50-8c3d8beb71a8",
      "title": "Intelligent Metal Salad",
      "isOnSale": true,
      "image": "http://192.168.43.112:3000/assets/240_F_242762993_Mvhy8RdXdKUBMOjXMR009QdUUFKbCWnO.jpg",
      "isOnWishList": true,
      "rating": 2,
      "regularPrice": 1104,
      "specialPrice": 425
    },
    {
      "id": "dd0c1bc1-ba87-4463-ab5e-402ed5967270",
      "title": "Licensed Steel Computer",
      "isOnSale": false,
      "image": "http://192.168.43.112:3000/assets/240_F_225384645_NcDcLSv5LQTPjMRyr17PmLNEey20kGQy.jpg",
      "isOnWishList": false,
      "rating": 2,
      "regularPrice": 1081,
      "specialPrice": 773
    },
    {
      "id": "4f068d11-087b-4612-b2ce-b4ac4567ee46",
      "title": "Generic Wooden Car",
      "isOnSale": false,
      "image": "http://192.168.43.112:3000/assets/240_F_227332917_kZ6cfJMjICYjBOcTZLfeBx7vfu46H3vr.jpg",
      "isOnWishList": false,
      "rating": 4,
      "regularPrice": 1241,
      "specialPrice": 180
    },
    {
      "id": "254fe1b3-1b4b-461a-98c1-eca99d50138d",
      "title": "Refined Rubber Tuna",
      "isOnSale": false,
      "image": "http://192.168.43.112:3000/assets/guitar.jpg",
      "isOnWishList": false,
      "rating": 5,
      "regularPrice": 1233,
      "specialPrice": 799
    },
    {
      "id": "8983dc5c-a194-478f-bb41-bbb26dcf5b93",
      "title": "Sleek Fresh Table",
      "isOnSale": true,
      "image": "http://192.168.43.112:3000/assets/240_F_286828963_tqoyi8LSW4qqyytYWju45eetylWUhrSR.jpg",
      "isOnWishList": false,
      "rating": 4,
      "regularPrice": 1489,
      "specialPrice": 260
    },
    {
      "id": "691a4796-d65b-4c57-a22b-2bc2b4504ea6",
      "title": "Small Concrete Hat",
      "isOnSale": true,
      "image": "http://192.168.43.112:3000/assets/240_F_240538990_8x6sCQFvwIQTwS1NXS2ZvqfLopxTjRDh.jpg",
      "isOnWishList": true,
      "rating": 2,
      "regularPrice": 1072,
      "specialPrice": 740
    }
  ],
  "pagination": {
    "total": 100,
    "currentPage": 1,
    "lastPage": 3
  }
}
```
