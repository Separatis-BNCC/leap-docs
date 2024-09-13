# Content

---

### Create Content

* Endpoint : `/contents`
* Method : `POST`
* Request Body :
  - `content_type` (String, Required)
  - `url` (String, Required)
  - `desc` (String)
  - `session_id` (Number, Required)

* Response Body :

```json
  {
    "status": 200,
    "msg": "Success",
    "data": {
        "content_type": "link",
        "url": "kwemdm",
        "desc": "smqid",
        "id": 6,
        "session_id": 1
    }
}
```

---

### Get Content

* Endpoint : `/contents/:contentId`
* Method : `GET`

* Respones Body :

```json
  {
    "status": 200,
    "msg": "Success",
    "data": {
        "id": 2,
        "content_type": "link",
        "url": "gagaz anjeng",
        "desc": "gagaz anjeng",
        "session_id": 1
    }
}
```

### Edit Content

* Endpoint : `/contents/:contentId`
* Method : `PUT`
* Request Body :
  - `content_type` (String, Required)
  - `url` (String, Required)
  - `desc` (String)
  - `session_id` (Number, Required)

* Response Body :

```json
  {
    "status": 200,
    "msg": "Success",
    "data": "Content updated!"
    }
```

### Delete Content

* Endpoint : `/contents/:contentId`
* Method : `DELETE`

* Response Body :

```json
  {
    "status": 200,
    "msg": "Success",
    "data": "Content with id 2 deleted successfully!"
}
```