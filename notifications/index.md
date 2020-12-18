# Show All Notification.

Show all Notifications.

**URL** : `/notifications`

**Method** : `GET`

**Auth required** : YES

**Permissions required** : --

**ResponseExplanation**: Response will be list of paginated notifications

## Success Responses

**Code** : `200 OK`

**Content** : In this example, user can see notification listed of first page in decending order according to date.

```json
{
  "unreadNotification": 2,
  "data": [
    {
      "id": "e86f6418-4855-4f95-8f00-27f2eb94bdba",
      "title": "Lorem ipsum",
      "image": "https://t4.ftcdn.net/jpg/02/66/65/73/240_F_266657349_5QMR6FiWIk0VAZHojNd7cdClDR5V6Ph2.jpg",
      "description": " Secondary line text. Lorem ipsum dolor sit amet consectetur adipiscit elit.",
      "date": "21 Jul 2020, Tuesday",
      "read": true,
      "link": ""
    },
    {
      "id": "6aaaffbb-bd83-4974-9757-b0193a62565e",
      "title": "Lorem ipsum",
      "image": "https://t4.ftcdn.net/jpg/02/66/65/73/240_F_266657349_5QMR6FiWIk0VAZHojNd7cdClDR5V6Ph2.jpg",
      "description": " Secondary line text. Lorem ipsum dolor sit amet consectetur adipiscit elit.",
      "date": "21 Jul 2020, Tuesday",
      "read": false,
      "link": ""
    },
    {
      "id": "ce362a07-5955-4cae-aeb9-211d46f2b382",
      "title": "Lorem ipsum",
      "image": "",
      "description": " Secondary line text. Lorem ipsum dolor sit amet consectetur adipiscit elit.",
      "date": "21 Jul 2020, Tuesday",
      "read": true,
      "link": "/product/938f010c-ded0-438d-8fe5-77230298be09"
    }
  ],
  "pagination": {
    "total": 100,
    "currentPage": 1,
    "lastPage": 3
  }
}
```

**Explanation**

```json
{
  "id": "id of notification",
  "title": "title of notification",
  "image": "image url of notification",
  "description": "description of notification",
  "date": "date formattted as '21 Jul 2020, Tuesday'",
  "read": "Boolean valut to determine if notification is read",
  "link": "frontend url to redirect "
}
```

# Mark a Notification as read.

Mark particular notification as read.

**URL** : `/notifications/{id}/read`

**URL Parameters** : where "id" the id of notification needed to be marked as read.

**Method** : `PUT`

**Auth required** : YES

**Permissions required** : --

**ResponseExplanation**: Response will we if operation was success !

## Success Responses

**Code** : `200 OK`

**Content** : --

```json
{ "success": true }
```

# Mark All Notification as read.

Mark all notification as read.

**URL** : `/mark-all-notification-as-read`

**Method** : `PUT`

**Auth required** : `YES`

**Permissions required** : --

**ResponseExplanation**: Response will we if operation was success !

## Success Responses

**Code** : `200 OK`

**Content** : --

```json
{ "success": true }
```
