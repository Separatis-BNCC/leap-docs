# Attendance

---

### Create Attendance

* Endpoint : `/attendances`
* Method : `POST`
* Request Body :
  - `class_session_id` (Number, Required)
  - `proof` (String, Required)
 
* Response Body :

```json
  {
  "status": 200,
  "message": "Success",
  "data": {
    "approved": 0,
    "proof": "https://res.cloudinary.com/example-proof-url.jpg",
    "credential_id": 1,
    "class_session_id": 1
  }
}
```

### Get Assignment

* Endpoint : `/attendances/:attendanceId`
* Method : `GET`

* Response Body :

```json
  {
  "status": 200,
  "message": "Success",
  "data": {
    "id": 1,
    "approved": 0,
    "proof": "https://res.cloudinary.com/example-proof-url.jpg",
    "credential_id": 1,
    "class_session_id": 1
  }
}
```

### Edit Assignment

* Endpoint : `/attendances/:attendanceId`
* Method : `PUT`
* Request Body :
  - `proof` (String, Required)

* Response Body :

```json
  {
  "status": 200,
  "message": "Attendance updated!"
}
```