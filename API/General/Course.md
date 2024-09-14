# Course

---

### Create Course

* Endpoint : `/courses`
* Method : `POST`
* Request Body :
  - `name` (String, Required)
  - `region` (Number, Required)

* Response Body :

```json
  {
  "status": 200,
  "message": "Success",
  "data": {
    "id": 1,
    "name": "JavaScript Basics",
    "region": 1
  }
}
```

### Get Courses

* Endpoint : `/courses`
* Method : `GET`

* Response Body :

```json
  {
  "status": 200,
  "message": "Success",
  "data": [
    {
      "id": 1,
      "name": "JavaScript Basics",
      "region": 1
    }
  ]
}
```

### Get Course

* Endpoint : `/courses/:courseId`
* Method : `GET`

* Response Body :

```json
{
    "status": 200,
    "msg": "Success",
    "data": {
        "id": 1,
        "name": "UI/UX",
        "region": 1,
        "total_sessions": 13,
        "status": 1,
        "classes": [
            {
                "id": 1,
                "name": "UI/UX - A",
                "day_of_week": null,
                "hour": null,
                "minute": null,
                "status": 1
            },
            {
                "id": 2,
                "name": "UI/UX - B",
                "day_of_week": null,
                "hour": null,
                "minute": null,
                "status": 1
            }
        ],
        "sessions": [
            {
                "id": 1,
                "week": 1,
                "description": "UI/UX week 1 description",
                "status": 1
            },
            {
                "id": 2,
                "week": 2,
                "description": "UI/UX week 2 description",
                "status": 1
            },
            {
                "id": 3,
                "week": 3,
                "description": "UI/UX week 3 description",
                "status": 1
            },
            {
                "id": 4,
                "week": 4,
                "description": "UI/UX week 4 description",
                "status": 1
            },
            {
                "id": 5,
                "week": 5,
                "description": "UI/UX week 5 description",
                "status": 1
            },
            {
                "id": 6,
                "week": 6,
                "description": "UI/UX week 6 description",
                "status": 1
            },
            {
                "id": 7,
                "week": 7,
                "description": "UI/UX week 7 description",
                "status": 1
            },
            {
                "id": 8,
                "week": 8,
                "description": "UI/UX week 8 description",
                "status": 1
            },
            {
                "id": 9,
                "week": 9,
                "description": "UI/UX week 9 description",
                "status": 1
            },
            {
                "id": 10,
                "week": 10,
                "description": "UI/UX week 10 description",
                "status": 1
            },
            {
                "id": 11,
                "week": 11,
                "description": "UI/UX week 11 description",
                "status": 1
            },
            {
                "id": 12,
                "week": 12,
                "description": "UI/UX week 12 description",
                "status": 1
            },
            {
                "id": 13,
                "week": 13,
                "description": "UI/UX week 13 description",
                "status": 1
            }
        ],
        "assignments": [
            {
                "id": 1,
                "url": "sasssssssss",
                "deadline": "2024-08-10T00:00:00.000Z",
                "status": 1
            }
        ]
    }
}
```

### Edit Course

* Endpoint : `/courses/:courseId`
* Method : `PUT`
* Request Body :
  - `name` (String, Required)
  - `region` (Number, Required)

* Response Body :

```json
{
    "status": 200,
    "msg": "Success",
    "data": [
        1
    ]
}
```

### Change Course Status

* Endpoint : `/courses/status/:courseId"`
* Method : `PUT`
* Request Body :
  - `status` (Number, Required)

* Response Body :

```json
{
    "status": 200,
    "msg": "Success",
    "data": [
        1
    ]
}
```

### Delete Course

* Endpoint : `/courses/:courseId`
* Method : `DELETE`

* Response Body :

```json
{
  "status": 200,
  "message": "Course with id {id} deleted successfully!"
}
```