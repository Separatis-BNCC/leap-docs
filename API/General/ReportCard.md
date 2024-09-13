# Report Card

---

### Create Report Card

* Endpoint : `/report-card`
* Method : `POST`
* Request Body :

  - credential_id (Number, Required)
  - document_url (String, Required)
  - desc (String, Required)

* Response Body :

```json
{
  "status": 200,
  "message": "Success",
  "data": {
    "id": 3,
    "document_url": "http://example.com/document.pdf",
    "desc": "Report card for semester 1",
    "credential_id": 1
  }
}
```

### Get Report Card

* Endpoint : `/report-card/:reportCardId`
* Method : `GET`

* Response Body :

```json
{
  "status": 200,
  "message": "Success",
  "data": {
    "id": 3,
    "document_url": "http://example.com/document.pdf",
    "desc": "Report card for semester 1",
    "credential_id": 1
  }
}
```

### Edit Report Card

* Endpoint : `/report-card/:reportCardId`
* Method : `PUT`
* Request Body :
  - document_url (String, Required)
  - desc (String)

* Response Body :

```json
{
  "status": 200,
  "message": "Report Card Updated"
}
```

### Delete Report Card

* Endpoint : `/report-card/:reportCardId`
* Method : `DELETE`

* Response Body :

```json
{
  "status": 200,
  "message": "Report Card with id {id} successfully deleted!"
}
```
