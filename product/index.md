# Get Detail of Product

Get all configuration of product detail page.

**URL** : `/products/{id}`

**URL Parameters** : where "id" the id of product

**Method** : `GET`

**Auth required** : YES/NO

**Permissions required** : --

## Success Responses

**Code** : `200 OK`

**Content** : Will get all the configurations including product descriptions and any other required of that page.

```json
{
  "id": "fec9e6e7-b3fb-4fb7-91a7-eb71f0e582bd",
  "title": "Licensed Granite Towels",
  "isOnSale": true,
  "images": [
    {
      "id": "feecb5be-da05-413c-8aeb-20985dd58644",
      "url": "http://localhost:3000/assets/240_F_286828963_tqoyi8LSW4qqyytYWju45eetylWUhrSR.jpg"
    },
    {
      "id": "694e0345-c5e8-4852-83e3-3a0781a1f89f",
      "url": "http://localhost:3000/assets/screen.jpg"
    },
    {
      "id": "395cebef-7f6b-4ac9-bd01-065e9dbf1f4d",
      "url": "http://localhost:3000/assets/500_F_213447172_toWrR5eZq00ogDS3UVAm2nobBl9EDOpw.jpg"
    },
    {
      "id": "1abdb2b7-1cac-4209-b406-96ac4330759c",
      "url": "http://localhost:3000/assets/stationery.jpg"
    },
    {
      "id": "e381e1c1-8788-490a-889b-5c55886c636a",
      "url": "http://localhost:3000/assets/240_F_214254276_MGgdX4C9McEiIsxMZCASLN07HK0G3sEF.jpg"
    },
    {
      "id": "7602193c-13b7-4c17-b2ac-110fc6d41ddc",
      "url": "http://localhost:3000/assets/500_F_241483481_oRi5hgejYBLD4gFR7PpJJOatZpaVGbVv.jpg"
    },
    {
      "id": "98d577ed-e069-4815-8876-3922886b66b3",
      "url": "http://localhost:3000/assets/240_F_357910720_k9ycvZwytwOiBM4RTvaJA63rmu2FwWnX.jpg"
    }
  ],
  "isOnWishList": false,
  "productDetail": [
    {
      "componentType": "product-rating",
      "data": {
        "totalReviews": 100,
        "avgRating": 3,
        "rating": [
          {
            "rating": 5,
            "review": 50
          },
          {
            "rating": 4,
            "review": 20
          },
          {
            "rating": 3,
            "review": 10
          },
          {
            "rating": 2,
            "review": 5
          },
          {
            "rating": 1,
            "review": 15
          }
        ]
      }
    },
    {
      "componentType": "exchange-policy-list-item",
      "data": {
        "days": 5,
        "policyUrl": "/exchange-policy/90d6a3b6-cd16-4208-9c36-9cfc645ed133"
      }
    }
  ],
  "regularPrice": 1360,
  "specialPrice": 896,
  "defaultAttribute": {
    "Brand": "APPLE",
    "MaterialType": "cotton",
    "Color": "green"
  },
  "productInfoBundle": [
    {
      "componentType": "article-attribute",
      "title": "Description",
      "content": {
        "data": "<span style='font-size: 1em;'>Check out the two different types of dropdowns in each of the 'Align' buttons.fasdfadfasdf</span><span style='font-size: 1em;'>fasdfaf</span></blockquote><pre><span style='font-size: 1em;'><a href='https://'>fasdf</a>fas</span></pre><pre><span style='font-size: 1em;'><br></span></pre><pre><span style='font-size: 1em;'>fasdfasdffasdfadsffasd string = var -- 12;</span></pre>"
      }
    },
    {
      "componentType": "video-attribute",
      "title": "videos",
      "content": {
        "data": [
          {
            "id": "a313698f-267c-4110-90fd-8a8bc4d202e8",
            "url": "https://www.youtube.com/embed/ycZshUhdukI"
          },
          {
            "id": "a313698f-267c-4110-90fd-8a8bc4d202e8",
            "url": "https://www.youtube.com/embed/ycZshUhdukI"
          }
        ]
      }
    },
    {
      "componentType": "customer-review",
      "title": "Customer Review"
    },
    {
      "componentType": "product-faq",
      "title": "FAQ"
    }
  ],
  "attributes": [
    {
      "name": "Color",
      "componentType": "product-attribute-color",
      "items": [
        {
          "enable": false,
          "id": "red",
          "title": "red"
        },
        {
          "enable": false,
          "id": "blue",
          "title": "blue"
        },
        {
          "enable": true,
          "id": "green",
          "title": "green"
        },
        {
          "enable": false,
          "id": "black",
          "title": "black"
        }
      ]
    },
    {
      "name": "Brand",
      "componentType": "product-attribute-box",
      "items": [
        {
          "enable": false,
          "id": "APPLE",
          "title": "APPLE"
        },
        {
          "enable": false,
          "id": "BALL",
          "title": "BALL"
        }
      ]
    },
    {
      "name": "MaterialType",
      "componentType": "product-attribute-box",
      "items": [
        {
          "enable": true,
          "id": "cotton",
          "title": "cotton"
        },
        {
          "enable": false,
          "id": "nylon",
          "title": "nylon"
        },
        {
          "enable": true,
          "id": "soft-fabric",
          "title": "soft-fabric"
        },
        {
          "enable": false,
          "id": "hard-fabric",
          "title": "hard-fabric"
        }
      ]
    }
  ],
  "isOnStock": false,
  "categoryAncestor": [
    {
      "id": "5f15ccda-3408-48c6-991e-700efb3a3433",
      "label": "Computers"
    },
    {
      "id": "6252bd3d-bd6a-4cdf-b81a-53a9336257d6",
      "label": "Clothing"
    },
    {
      "id": "644af2b1-9a5e-462d-84ab-23d26f4b8fef",
      "label": "Movies"
    },
    {
      "id": "cebe5f79-2df5-4c40-b23b-223ca484828c",
      "label": "Garden"
    },
    {
      "id": "ad1d295e-3205-45ff-800c-7cd1c2c8ce1a",
      "label": "Music"
    }
  ]
}
```

# Show All Comments of a product.

Show all comments or review of a product

**URL** : `/products/{id}/review`

**Method** : `GET`

**Query Params** : `{page:1}`

**Auth required** : NO

**Permissions required** : --

**ResponseExplanation**: Response will be list of paginated reviews sorted by date in decending order.

## Success Responses

**Code** : `200 OK`

**Content** : In this example, user can see reives listed of first page in decending order according to date.

```json
{
  "data": [
    {
      "id": "1bc04157-ff23-4510-8b51-a788fa82e522",
      "name": "Loren Hills",
      "image": "http://localhost:3000/assets/240_F_229877921_CVeSJLLVSp8qxGaiFzLfNNJ0DnPTgEij.jpg",
      "date": "2020-01-01",
      "rating": 4,
      "review": "Consequuntur et nisi sit quia soluta nostrum quia totam. Voluptas id quia quo natus consequatur voluptatem iure sit vero. Nulla velit et sint. Omnis est et ad et voluptas. Doloremque officia omnis quo ut explicabo soluta consequatur.",
      "replies": [
        {
          "id": "cbe83584-5646-4fba-ab01-3e0e6ab946c6",
          "date": "2020-01-01",
          "name": "Desmond Swift",
          "review": "Nihil rerum molestias ut assumenda autem. Ipsa repellendus id ut eius sit ullam qui enim. Iusto nobis qui recusandae temporibus. Minus impedit cumque est aut odio voluptatem et et distinctio. Accusantium dolore qui.",
          "image": "http://localhost:3000/assets/240_F_194838427_258O1EM8215TPZVbrAHyn8XNbA7Sumqm.jpg"
        },
        {
          "id": "250ac93b-a284-4063-a9a1-ee231deeb8e8",
          "date": "2020-01-01",
          "name": "Baby Marvin",
          "review": "Voluptatem et consequatur. Est esse quae adipisci fugit excepturi. Sint dolore voluptatibus totam voluptatibus. Beatae voluptates officiis aut. Est a modi dolorem. Et et deleniti officia aut eaque ut.",
          "image": "http://localhost:3000/assets/240_F_85030606_LWbZt4ltW5wIgbuWsvVZK6rU4srqvaY6.jpg"
        },
        {
          "id": "c9ab8935-fc00-4a61-9738-9b28685c5092",
          "date": "2020-01-01",
          "name": "Mauricio Koss",
          "review": "Aspernatur molestiae accusantium nobis explicabo eveniet. Optio sapiente sint provident doloribus aut necessitatibus blanditiis sit. Adipisci doloremque minus ut qui nobis tenetur architecto. Modi minus explicabo itaque optio dolore. Omnis quia quia nihil et ipsum rerum dolor atque.",
          "image": "http://localhost:3000/assets/240_F_245692031_q0rKTbkw3fl3U0jXwjpDWTezUfxUD61u.jpg"
        },
        {
          "id": "3a56df96-70da-4e50-aa04-7b3da371f551",
          "date": "2020-01-01",
          "name": "Felicia Dicki",
          "review": "Natus in et accusamus itaque aut. Quo quisquam cum itaque reprehenderit adipisci itaque in. Quod veritatis illum. Maiores debitis reprehenderit rem consequatur qui at. Accusamus voluptatem nostrum fugit quam alias eos saepe aspernatur. Mollitia nulla sit cum reiciendis.",
          "image": "http://localhost:3000/assets/240_F_271682471_5suOLRazuKX1VPRV8JQMDo6Y2El9QJ6L.jpg"
        }
      ]
    },
    {
      "id": "3e32e0bb-5e07-47ba-bb9a-ddd7da2c5921",
      "name": "Brenna Kris",
      "image": "http://localhost:3000/assets/240_F_370380_hpL0eScPr9oTuiWxcmaNpydRFBcvaN.jpg",
      "date": "2020-01-01",
      "rating": 1,
      "review": "Et recusandae iste sequi voluptas blanditiis veritatis unde laboriosam. Aut inventore vel sapiente assumenda in corporis sint aliquid quibusdam. Quaerat enim dolores sed qui.",
      "replies": [
        {
          "id": "b8ec8437-85e1-4d3b-8c57-80adcb086c30",
          "date": "2020-01-01",
          "name": "Sophie Feeney",
          "review": "Veniam ut voluptatem eum nemo est est autem est. Voluptatem aut et iste vel. Et ut quo nostrum.",
          "image": "http://localhost:3000/assets/banner-three.png"
        },
        {
          "id": "dcb66bf2-bb54-47eb-bea4-0816df24c2d0",
          "date": "2020-01-01",
          "name": "Breanne Beahan",
          "review": "Voluptatem eum dolorem cumque impedit dicta. Consectetur est nobis unde pariatur. Nemo quo eos. Consequatur nobis dolorem accusantium facere dolorem. Itaque molestias ut nihil ut ut. Aut a occaecati est.",
          "image": "http://localhost:3000/assets/240_F_299514203_AVNwIQEe5Uvuz4gGtcv7LTlrXEZGGnnH.jpg"
        },
        {
          "id": "670977fa-00c9-46fa-ae1a-121de0ecbaf1",
          "date": "2020-01-01",
          "name": "Alisha Schimmel",
          "review": "Modi unde sit maiores aut et perferendis suscipit placeat. Et ut est qui. Est facere ullam tempora aliquid. Quia tempora quisquam error aut commodi dolor omnis saepe.",
          "image": "http://localhost:3000/assets/240_F_299514203_AVNwIQEe5Uvuz4gGtcv7LTlrXEZGGnnH.jpg"
        },
        {
          "id": "b32c835e-1067-46b8-a0f5-831b919df0a6",
          "date": "2020-01-01",
          "name": "Alexander Bogisich",
          "review": "Sint voluptatum aut omnis. Incidunt dolor quos nulla. Quia quos dolores repellat est quasi corrupti neque omnis est. Voluptatum voluptatum id nam.",
          "image": "http://localhost:3000/assets/magicmouse.jpg"
        }
      ]
    },
    {
      "id": "360def6a-82b6-4687-9fcb-ad9b286dd939",
      "name": "Cecelia Gleason",
      "image": "http://localhost:3000/assets/banner-three.png",
      "date": "2020-01-01",
      "rating": 5,
      "review": "Qui cum animi tempora reiciendis natus. Quia tempora neque enim laudantium accusamus culpa. Ipsa soluta voluptatem exercitationem sint repellat dolor quibusdam.",
      "replies": [
        {
          "id": "45b751ca-d694-4ba7-b268-f6b31a11b9d4",
          "date": "2020-01-01",
          "name": "Karina Spencer",
          "review": "Voluptate facilis commodi modi officia sed sunt voluptas iure mollitia. Qui voluptates pariatur. Qui quia id quod est ullam molestias quo quibusdam. Consequatur nobis ut vel velit alias quisquam commodi facere eveniet. Voluptas nihil sit molestias laborum consectetur autem id fugiat. Vel est laborum accusamus rerum.",
          "image": "http://localhost:3000/assets/500_F_60159844_gfS932JFD2KXwsyMFmouZiHMfFPrPzFw.jpg"
        },
        {
          "id": "b4036e32-db38-449d-8a94-2d89341b29e9",
          "date": "2020-01-01",
          "name": "Jessy Altenwerth",
          "review": "Tempore alias magni. Velit quasi ut neque soluta et sequi aut. Voluptatum omnis necessitatibus qui mollitia sed.",
          "image": "http://localhost:3000/assets/mobile.jpg"
        },
        {
          "id": "27bd4b75-86e0-44ef-a2d2-b7ba44946706",
          "date": "2020-01-01",
          "name": "Osvaldo Gleason",
          "review": "Earum alias libero tempora accusantium accusantium odit architecto nesciunt unde. At reprehenderit repellat illum error aut vel ab. Vitae molestiae earum repellendus sapiente quia.",
          "image": "http://localhost:3000/assets/240_F_370380_hpL0eScPr9oTuiWxcmaNpydRFBcvaN.jpg"
        },
        {
          "id": "a1245a16-686c-4596-bcd4-0ecdaa3806e1",
          "date": "2020-01-01",
          "name": "Andy Hintz",
          "review": "Ipsum ullam beatae reiciendis veniam incidunt qui. Est a voluptate. Doloribus ut libero vel iste sed.",
          "image": "http://localhost:3000/assets/500_F_241483481_oRi5hgejYBLD4gFR7PpJJOatZpaVGbVv.jpg"
        }
      ]
    },
    {
      "id": "9ed578b0-9107-46ef-bda5-657f571300a8",
      "name": "Mariano Fahey",
      "image": "http://localhost:3000/assets/240_F_273104017_VEFaFezhGZJQ0hC5spR8q1ghhoTtAdZV.jpg",
      "date": "2020-01-01",
      "rating": 4,
      "review": "Omnis ut fugiat qui voluptate iure dolores saepe perferendis. Fugiat inventore et dolorum eum. Qui aliquid assumenda fuga accusantium reiciendis. Voluptatem qui illo sit asperiores unde.",
      "replies": [
        {
          "id": "b734111e-e683-45ea-a0d6-dfe03b1cc07b",
          "date": "2020-01-01",
          "name": "Roxane Yost",
          "review": "Minus velit minus ea quod omnis quia aut. Reiciendis officiis soluta aut. Deserunt architecto aut quae sit magni ea nisi. Voluptatem atque pariatur.",
          "image": "http://localhost:3000/assets/240_F_185089663_87mLybPDYom0JKTbefhdSjHFhdIm0Qqy.jpg"
        },
        {
          "id": "f151d22e-c86d-4606-b4d6-cad9230cf7fc",
          "date": "2020-01-01",
          "name": "Stan Schmeler",
          "review": "Qui nam sint exercitationem quia harum. Ea aut enim doloribus accusantium laboriosam. Eaque libero explicabo.",
          "image": "http://localhost:3000/assets/240_F_106242291_ZOJeEhJg0ohTzXoB2HabeQ0Ogx1t3ibS.jpg"
        },
        {
          "id": "d8c903bd-8d9f-4708-83ea-041dfa2e90e4",
          "date": "2020-01-01",
          "name": "Julia Ondricka",
          "review": "Neque nobis mollitia perspiciatis officia aspernatur perferendis ea tempore. Repellat impedit possimus odio placeat fuga. Quae aliquam perferendis et enim aut. Dicta veritatis nulla. Consequatur at consequatur magni atque temporibus. Molestiae similique voluptates quos quia sit.",
          "image": "http://localhost:3000/assets/240_F_330088839_8Te8kjQADKFIPtoH4dOCX64dkJgBHVtF.jpg"
        },
        {
          "id": "414fd5cf-bcda-4665-92d4-2ebab10a60d8",
          "date": "2020-01-01",
          "name": "Randal Collier",
          "review": "Voluptatum nesciunt dolorem ducimus autem ut hic voluptas impedit. Ex aliquam eum rerum perferendis quisquam illum vero. Quidem quia rerum laborum quia laboriosam aut. Sint rem perspiciatis vel modi harum eum. Totam aut vitae distinctio.",
          "image": "http://localhost:3000/assets/240_F_371723060_P4KpCFjcOQtnLNIv4rU2jf4mW3wUiRBy.jpg"
        }
      ]
    }
  ],
  "pagination": {
    "total": 100,
    "currentPage": 1,
    "lastPage": 20
  }
}
```

# Show All FAQs of a product.

Show all FAQs of a product

**URL** : `/products/{id}/faq`

**Method** : `GET`

**Query Params** : `{page:1}`

**Auth required** : NO

**Permissions required** : --

**ResponseExplanation**: Response will be list of paginated reviews sorted by date in decending order.

## Success Responses

**Code** : `200 OK`

**Content** : In this example, user can see FAQs

```json
{
  "data": [
    {
      "question": "Omnis voluptatem in necessitatibus fugit itaque quia assumenda.",
      "answer": "Tempore deserunt libero non hic voluptatibus id cumque eius. Voluptatum quidem at. Esse et vel quos quas hic esse laudantium. Nisi facere et tenetur. Est qui fugit natus magnam amet fugiat aut voluptatibus rerum. Molestiae quis explicabo."
    },
    {
      "question": "Blanditiis provident commodi tempore quo ex asperiores iusto nemo totam.",
      "answer": "Aut reiciendis ducimus sed non. Officia aut dicta tempora totam rerum ea similique."
    },
    {
      "question": "Non voluptatum ratione optio incidunt vero minima nobis laudantium.",
      "answer": "Fugiat blanditiis reiciendis ut autem maiores illo. Sit laborum cum et quibusdam natus molestiae earum nesciunt."
    },
    {
      "question": "Aperiam illum quo quo nihil natus ea sunt iusto.",
      "answer": "Tenetur sequi inventore non. Ad minima eligendi enim est. Voluptatem fuga eligendi impedit."
    }
  ],
  "pagination": {
    "total": 100,
    "currentPage": 1,
    "lastPage": 20
  }
}
```
