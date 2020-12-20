# Get user info

Get detail of current authenticateed user, including basic information to detailed.

**URL** : `/me`

**Method** : `GET`

**Auth required** : YES

**Permissions required** : --

## Success Responses

**Code** : `200 OK`

**Content** : Response will include current user details

```json
{
  "fullname": "Sanjay Gyawali",
  "username": "sanjay",
  "email": "isanjay48@gmail.com",
  "phone": "9844776371",
  "image": "http://localhost:3000/assets/240_F_185089663_87mLybPDYom0JKTbefhdSjHFhdIm0Qqy.jpg",
  "unreadNotificationCount": 7
}
```
