# Session

---

### Get Session

* Endpoint : `/sessions/:sessionId`
* Method : `GET`
* Response Body :

```json
{
  "status": 200,
  "message": "Success",
  "data": {
    "id": 1,
    "week": 5,
    "description": "This week's focus is on front-end basics.",
    "contents": [
      {
        "id": 1,
        "content_type": "video",
        "url": "https://example.com/video",
        "desc": "Introduction to HTML"
      },
      {
        "id": 2,
        "content_type": "document",
        "url": "https://example.com/document",
        "desc": "HTML and CSS basics"
      }
    ]
  }
}
```

### Edit Session

* Endpoint : `/session/:sessionId`
* Method : `PUT`
* Request Body :
  - week (Number, Optional)
  - description (String, Optional)

* Response Body :

```json
{
  "status": 200,
  "message": "Session updated!"
}
```
