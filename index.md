# Show Index page configuration

Show all configuration api needed to generate to render index-page.

**URL** : `/index-page-config`

**Method** : `GET`

**Params** : `{page:1}`

**Auth required** : NO

**Permissions required** : --

## Success Responses

**Content** : In this example , response is a object with banners ie.(slider) and configurations:
banners is a array of object. Configurations are the configuration of each layout rendered after banner

**Explaination of RESPONSE**:
| DataElement | Description |
| -- | -- |
| banners | is array of sliders with details of slider (link should be absolute path to a page which is intended to be redirected )|
|configurations| configurations is a paginated response with object "data,pagination"|
| configurations.data | is array of layout configuration which will render content on the layout |
|configurations.pagination | this is paginated response which consists of total, currentPage and lastPage

**Explanation of configurations.data[i]**

```json
{
  "type": "component type availabe are .[product-row,deal-row,event-row,category-gallery]",
  "config": {
    "category": "featured",
    "special": true,
    "title": "Heading title which will be used to define the title of layout",
    // to refers to the vue router to object. according to this each layout will be redirected.
    "to": {
      "path": "/filter",
      "query": {
        "category": "featuredProducts"
      }
    }
  },
  "data": {
    // data of the product , event , or anything that will render, the item-card
    "data": [
      {
        "id": "6bba15e0-b1a0-4bc1-b18e-17cedae7eb6c",
        "title": "Small Rubber Ball",
        "isOnSale": false,
        "image": "http://localhost:3000/assets/240_F_178906893_MNw7D7DAoUbcozipesGlb0SdTZnRScOf.jpg",
        "isOnWishList": false,
        "rating": 4,
        "regularPrice": 1017,
        "specialPrice": 402
      }
    ],
    //   pagination to track the pagination of every layout
    "pagination": {
      "total": 10,
      "currentPage": 1,
      "lastPage": 10
    }
  }
}
```

**_Example Response_**

```json
{
  "banners": [
    {
      "id": 1,
      "title": "Something",
      "link": "product/14e7aad5-6e5a-4cfd-9850-8e7343a35da4",
      "img": "http://localhost:3000/assets/banner-one.png"
    },
    {
      "id": 2,
      "title": "Something",
      "link": "product/14e7aad5-6e5a-4cfd-9850-8e7343a35da4",
      "img": "http://localhost:3000/assets/banner-three.png"
    }
  ],
  "configurations": {
    "data": [
      {
        "type": "product-row",
        "config": {
          "category": "featured",
          "special": true,
          "title": "Featured Products",
          "to": {
            "path": "/filter",
            "query": {
              "category": "featuredProducts"
            }
          }
        },
        "data": {
          "data": [
            {
              "id": "6bba15e0-b1a0-4bc1-b18e-17cedae7eb6c",
              "title": "Small Rubber Ball",
              "isOnSale": false,
              "image": "http://localhost:3000/assets/240_F_178906893_MNw7D7DAoUbcozipesGlb0SdTZnRScOf.jpg",
              "isOnWishList": false,
              "rating": 4,
              "regularPrice": 1017,
              "specialPrice": 402
            }
          ],
          "pagination": {
            "total": 10,
            "currentPage": 1,
            "lastPage": 10
          }
        }
      },
      {
        "type": "event-row",
        "config": {
          "title": "Specials Event",
          "to": {
            "path": "/deal"
          }
        },
        "data": {
          "data": [
            {
              "id": "b4bf3a13-916e-477b-9a02-c8a1042a7150",
              "image": "http://localhost:3000/assets/240_F_354056455_jYs8QYuRbouxglTyUCVvTkUYpluTYVo8.jpg",
              "title": "Get40per off",
              "referral": "https://garland.biz"
            }
          ],
          "pagination": {
            "total": 10,
            "currentPage": 1,
            "lastPage": 10
          }
        }
      },
      {
        "type": "deal-row",
        "config": {
          "title": "Special Deals For You",
          "to": {
            "path": "/deal"
          }
        },
        "data": {
          "data": [
            {
              "id": "725a095c-5b3e-4fb5-be8d-fed0773d3be0",
              "image": "http://localhost:3000/assets/240_F_103165670_r5PEYdER7rQ3ip80Ker5L7Ihgl7CV7eC.jpg",
              "title": "Get39per off",
              "deadline": "2021-04-20T06:36:51.023Z",
              "referral": "https://buford.biz"
            }
          ],
          "pagination": {
            "total": 10,
            "currentPage": 1,
            "lastPage": 3
          }
        }
      },
      {
        "type": "category-gallery",
        "config": {
          "title": "Shop by category",
          "to": {
            "path": "/categories"
          }
        },
        // category gallery is fixed and does not paginate.
        // TODO: Revirify.
        "data": [
          {
            "id": "a8439b4e-acdf-43d3-bef8-363303156ae9",
            "img": "http://localhost:3000/assets/240_F_211954868_1dmCON8HfdXwVoAMisWgSq7Yn4Z6mpMd.jpg",
            "title": "Health",
            "link": "http://brant.org"
          },
          {
            "id": "b10dc66b-25a3-46bd-a6e4-6bec90949581",
            "img": "http://localhost:3000/assets/240_F_241082075_G2aJ7dzwwNJPeYSIptz5Z2fpUEw5gnpm.jpg",
            "title": "Electronics",
            "link": "https://dax.biz"
          }
        ]
      },
      {
        "type": "product-row",
        "config": {
          "category": "recommended",
          "special": true,
          "title": "Recommended for you",
          "to": {
            "path": "/filter",
            "query": {
              "category": "recommended"
            }
          }
        },
        "data": {
          "data": [
            {
              "id": "97f3a453-9faf-43cd-9ced-a265ff3537ad",
              "title": "Rustic Fresh Mouse",
              "isOnSale": true,
              "image": "http://localhost:3000/assets/240_F_242762993_Mvhy8RdXdKUBMOjXMR009QdUUFKbCWnO.jpg",
              "isOnWishList": false,
              "rating": 4,
              "regularPrice": 1361,
              "specialPrice": 483
            }
          ],
          "pagination": {
            "total": 10,
            "currentPage": 1,
            "lastPage": 10
          }
        }
      }
    ],
    // paginate over all confuguration as well.
    "pagination": {
      "total": 100,
      "currentPage": 1,
      "lastPage": 2
    }
  }
}
```
