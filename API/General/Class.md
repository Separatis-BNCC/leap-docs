# Assignment

---

### Create Class

* Endpoint : `/classes`
* Method : `POST`
* Request Body :

  - `name` (String, Required)
  - `day_of_week` (Date, Required)
  - `hour` (Number, Required)
  - `minute` (Number, Required)
  - `course_id` (Number, Required)

* Response Body :

```json
{
  "status": 200,
  "message": "Success",
  "data": {
    "id": 1,
    "name": "Example Class",
    "day_of_week": 2,
    "hour": 10,
    "minute": 30
  }
}
```

---

### Edit Class

* Endpoint : `/classes/:classId`
* Method : `PUT`
* Request Body :

  - `name` (String, Optional)
  - `day_of_week` (Number, Optional)
  - `hour` (Number, Optional)
  - `minute` (Number, Optional)

* Respones Body :

```json
{
  "status": 200,
  "message": "Success edit class with id 1!"
}
```

### Get Classes

* Endpoint : `/classes`
* Method : `GET`

* Respones Body :

```json
{
  "status": 200,
  "message": "Success",
  "data": [
    {
      "id": 1,
      "name": "Example Class",
      "day_of_week": 2,
      "hour": 10,
      "minute": 30,
      "member_count": 15,
      "course": {
        "name": "Course Name"
      }
    }
  ]
}
```

### Get Classes

* Endpoint : `/classes/:classId`
* Method : `GET`

* Respones Body :

```json
{
    "status": 200,
    "msg": "Success",
    "data": {
        "id": 2,
        "name": "UI/UX - B",
        "day_of_week": null,
        "hour": null,
        "minute": null,
        "status": 1,
        "course_id": 1,
        "members": [
            {
                "id": 2,
                "email": "user@gmail.com",
                "role": 4,
                "active": false,
                "profile": {
                    "first_name": "Gagaz",
                    "last_name": "Manqunazara"
                }
            }
        ],
        "courses": {
            "id": 1,
            "name": "UI/UX",
            "region": 1,
            "total_sessions": 13,
            "status": 1,
            "assignments": []
        },
        "sessions": [
            {
                "id": 1,
                "week": 1,
                "description": "UI/UX week 1 description",
                "status": 1,
                "course_id": 1
            },
            {
                "id": 2,
                "week": 2,
                "description": "UI/UX week 2 description",
                "status": 1,
                "course_id": 1
            }
        ]
    }
}
```

### Delete Class

* Endpoint : `/classes/:classId`
* Method : `DELETE`

* Respones Body :

```json
{
  "status": 200,
  "message": "Course with id 1 deleted successfully!"
}
```

### addMembers

* Endpoint : `/classes/:class_id/members`
* Method : `POST`
* Request Body :

  - `ids` (Numbers[], Required)

* Respones Body :

```json
{
    "status": 200,
    "msg": "Success",
    "data": {
        "warningMsg": [
            "Members with id 10, 20 not found!",
            "Members with id 2 already in class with id 1"
        ],
        "successMsg": "Success add member with id 3 to class with id 1"
    }
}
```

### Add Praetorian

* Endpoint : `/classes/:class_id/praetorian`
* Method : `POST`
* Request Body :

  - `id` (Number, Required)

* Respones Body :

```json
{
  "status": 200,
  "message": "Success add praetorian to class with id 1"
}
```

### Remove Member

* Endpoint : `/classes/:class_id/members/:credentialId`
* Method : `DELETE`

* Respones Body :

```json
{
  "status": 200,
  "message": "Success remove member with id 1 from class with id 1"
}
```

### Remove Praetorian

* Endpoint : `/classes/:class_id/praetorian/:credentialId`
* Method : `DELETE`

* Respones Body :

```json
{
  "status": 200,
  "message": "Success remove praetorian with id 1 from class with id 1"
}
```
