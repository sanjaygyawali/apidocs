# Get Items of Cart , (api to populate list in cart sidebar)

Show required items . Items id are sent in the url query params.

**URL** : `/cart/items`

**Query Parameters** : `[{"id":"a7e4fb1d-8707-455e-b7b0-3b9e82926dd3"},{"id":"83c56404-f6fd-429d-bcc5-5de63cdbd71f"},{"id":"c08d2c38-304d-45dd-9c86-637f5d5bfd9e"},{"id":"4160822d-a3e8-493c-adcb-ac6f0a123d5b"},{"id":"d2563b39-d017-4a33-9b53-3eb2d7fdab83"}]`

**Method** : `GET`

**Auth required** : NO

**Permissions required** : --

## Success Responses

**Code** : `200 OK`

**Content** : Response will be array of items object.

```json
[
  {
    "id": "a7e4fb1d-8707-455e-b7b0-3b9e82926dd3",
    "title": "Awesome Frozen Bike",
    "isOnSale": false,
    "image": "http://192.168.0.105:3000/assets/240_F_86542099_bP0359YevWiJ20O7pTrCqOLaYHIuuWGM.jpg",
    "isOnWishList": true,
    "brand": "Waelchi - Bins",
    "rating": 3,
    "regularPrice": 1186,
    "specialPrice": 958,
    "quantity": 25
  },
  {
    "id": "83c56404-f6fd-429d-bcc5-5de63cdbd71f",
    "title": "Unbranded Cotton Bacon",
    "isOnSale": true,
    "image": "http://192.168.0.105:3000/assets/240_F_370380_hpL0eScPr9oTuiWxcmaNpydRFBcvaN.jpg",
    "isOnWishList": false,
    "brand": "Steuber - Collins",
    "rating": 3,
    "regularPrice": 1103,
    "specialPrice": 927,
    "quantity": 7
  },
  {
    "id": "c08d2c38-304d-45dd-9c86-637f5d5bfd9e",
    "title": "Handcrafted Wooden Mouse",
    "isOnSale": true,
    "image": "http://192.168.0.105:3000/assets/240_F_68118716_tTJR338uevfq83IWYBthpqmWD6j2tg8d.jpg",
    "isOnWishList": true,
    "brand": "Oberbrunner - Abshire",
    "rating": 5,
    "regularPrice": 1060,
    "specialPrice": 674,
    "quantity": 1
  },
  {
    "id": "4160822d-a3e8-493c-adcb-ac6f0a123d5b",
    "title": "Incredible Wooden Chips",
    "isOnSale": true,
    "image": "http://192.168.0.105:3000/assets/Sample1.jpg",
    "isOnWishList": false,
    "brand": "Kozey, Dare and Quigley",
    "rating": 1,
    "regularPrice": 1087,
    "specialPrice": 602,
    "quantity": 1
  },
  {
    "id": "d2563b39-d017-4a33-9b53-3eb2d7fdab83",
    "title": "Unbranded Cotton Pants",
    "isOnSale": true,
    "image": "http://192.168.0.105:3000/assets/240_F_257644733_pe2cQRLCF698aaQfmg2NFATJIPTyfKFL.jpg",
    "isOnWishList": false,
    "brand": "Kertzmann - Berge",
    "rating": 1,
    "regularPrice": 1359,
    "specialPrice": 982,
    "quantity": 6
  }
]
```

# Apply for Promotions.

Apply promotion code to get discount. => Client would send promotion code as well as the items in cart to check if the items in cart are eligible for coupons discount.

**URL** : `/promotions/apply`

**Request Payload** :

```json
{
  "code": "fsdfadf",
  "items": [
    { "id": "a7e4fb1d-8707-455e-b7b0-3b9e82926dd3" },
    { "id": "83c56404-f6fd-429d-bcc5-5de63cdbd71f" },
    { "id": "c08d2c38-304d-45dd-9c86-637f5d5bfd9e" },
    { "id": "4160822d-a3e8-493c-adcb-ac6f0a123d5b" },
    { "id": "d2563b39-d017-4a33-9b53-3eb2d7fdab83" }
  ]
}
```

**Method** : `GET`

**Auth required** : YES

**Permissions required** : --

## Success Responses

**Condition**: Failure

**Code** : `200 OK`

**Content** : Response will be a object with detailed response of failure, cases may be the items in the cart may not be sometime eligible for promotion code aplication

```json
{
  "status": "failed",
  "code": "fsdfadf",
  "message": "Promotion code, 'code' failed to apply",
  "discount": 0
}
```

**Condition**: Success

**Code** : `200 OK`

**Content** : Response will be a object with detailed response of success

```json
{
  "status": "success",
  "code": "fasdfasdfadsf",
  "message": "Promotion code fasdfasdfadsf applied",
  "discount": 700
}
```
