# Assignment

---

### Create Assignment

* Endpoint : `/assignments`
* Method : `POST`
* Request Body :
  - `url` (String, Required)
  - `deadline` (Date, Required)
  - `status` (Number, Required)
  - `course_id` (Number, Required)

* Response Body :

```json
  {
    "status": 200,
    "msg": "Success",
    "data": {
        "id": 1,
        "url": "sasssssssss",
        "deadline": "2024-08-10T00:00:00.000Z",
        "status": 1,
        "course_id": 1
    }
  }
```

### Get Assignment

* Endpoint : `/assignments/:assignmentId`
* Method : `GET`

* Response Body :

```json
  {
    "status": 200,
    "msg": "Success",
    "data": {
        "id": 1,
        "url": "sasssssssss",
        "deadline": "2024-08-10T00:00:00.000Z",
        "status": 1,
        "course_id": 1
    }
  }
```

### Edit Assignment

* Endpoint : `/assignments/:assignmentId`
* Method : `PUT`
* Request Body :
  - `url` (String, Required)
  - `deadline` (Date, Required)
  - `status` (Number, Required)
  - `course_id` (Number, Required)

* Response Body :

```json
  {
  "status": 200,
  "message": "Assignment updated!"
  }
```

### Delete Assignment

* Endpoint : `/assignments/:assignmentId`
* Method : `DELETE`

* Response Body :

```json
  {
  "status": 200,
  "message": "Assignment with id {id} deleted successfully!"
  }
```