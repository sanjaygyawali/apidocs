# Show All Categories.

Show all Top Level Categories.

**URL** : `/categories`

**Method** : `GET`

**Auth required** : NO

**Permissions required** : --

**ResponseExplanation**: Response will be object containing the count of categours and array of categories.

## Success Responses

**Code** : `200 OK`

**Content** : In this example, user can see all the categories listed.

```json
{
  "children": 5,
  "categories": [
    {
      "id": "08b8a78a-9fe9-4fb3-84cc-0063f9df81ae",
      "label": "Toys",
      "children": 8
    },
    {
      "id": "50cef54c-034b-4005-be3d-4047bd5ecc06",
      "label": "Beauty",
      "children": 3
    },
    {
      "id": "37c46702-4c14-4354-8a07-66fce2c428d7",
      "label": "Computers",
      "children": 8
    },
    {
      "id": "78ff9cfd-ffbf-4f79-99c7-0e3dfa746f6b",
      "label": "Shoes",
      "children": 13
    },
    {
      "id": "ed484bf0-447e-4ba9-bccf-956e203907af",
      "label": "Automotive",
      "children": 20
    }
  ]
}
```

# Show All Children of a Category.

Show all Top Level Categories.

**URL** : `/categories/{id}`

**URL Parameters** : where "id" the id or primary key of category.

**Method** : `GET`

**Auth required** : NO

**Permissions required** : --

## Success Responses

**Code** : `200 OK`

**Content** : Response will be object with id: own id, children count ,parent_id and array of categories.

```json
{
  "id": "78a08b8a-9fe9-b34f-cc84-f9df006381fe",
  "children": 5,
  "parent_id": "8b8a78a0-b34f-9fe9-cc84-f9df006381fe",
  "categories": [
    {
      "id": "08b8a78a-9fe9-4fb3-84cc-0063f9df81ae",
      "label": "Toys",
      "children": 8
    },
    {
      "id": "50cef54c-034b-4005-be3d-4047bd5ecc06",
      "label": "Beauty",
      "children": 3
    },
    {
      "id": "37c46702-4c14-4354-8a07-66fce2c428d7",
      "label": "Computers",
      "children": 8
    },
    {
      "id": "78ff9cfd-ffbf-4f79-99c7-0e3dfa746f6b",
      "label": "Shoes",
      "children": 13
    },
    {
      "id": "ed484bf0-447e-4ba9-bccf-956e203907af",
      "label": "Automotive",
      "children": 20
    }
  ]
}
```

# Get Ansestor chain of a category.

Show all category for cages.

**URL** : `/categories/{id}/ansestor`

**URL Parameters** : where "id" the id or primary key of category.

**Method** : `GET`

**Auth required** : NO

**Permissions required** : --

## Success Responses

**Code** : `200 OK`

**Content** : Response will be array of objects with id and label of category.

```json
[
  {
    "id": "af2ae030-f08f-41d6-9d22-9446524d8c73",
    "label": "Shoes"
  },
  {
    "id": "4aa07904-8890-482b-9455-f5e0703dad0b",
    "label": "Jewelery"
  },
  {
    "id": "d502ac9b-98d2-4f40-895f-f78c2dad47b4",
    "label": "Outdoors"
  },
  {
    "id": "ddccdcaa-25ef-4c25-aad8-40bad6a52989",
    "label": "Electronics"
  },
  {
    "id": "ecad5749-04db-490c-a891-5c32cbdfc233",
    "label": "Books"
  }
]
```
