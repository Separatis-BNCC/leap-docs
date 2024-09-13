# User

---

### Get Users

* Endpoint : `/users`
* Method : `GET`
* Response Body :

```json
{
    "status": 200,
    "msg": "Success",
    "data": [
        {
            "id": 3,
            "email": "user2@gmail.com",
            "role": 4,
            "active": false,
            "profile": null
        },
        {
            "id": 5,
            "email": "user4@gmail.com",
            "role": 4,
            "active": false,
            "profile": null
        },
        {
            "id": 4,
            "email": "user3@gmail.com",
            "role": 2,
            "active": false,
            "profile": null
        },
        {
            "id": 7,
            "email": "user5@gmail.com",
            "role": 4,
            "active": false,
            "profile": null
        },
        {
            "id": 2,
            "email": "user@gmail.com",
            "role": 4,
            "active": true,
            "profile": {
                "first_name": "Gagaz",
                "last_name": "Manqunazara",
                "nim": "2702254063",
                "birth_date": "2024-08-17T00:00:00.000Z",
                "region": 1,
                "faculty": 1,
                "major": 1,
                "line_id": "aind"
            }
        }
    ]
}
```

### Get User

* Endpoint : `/users/:userId`
* Method : `GET`
* Response Body :

```json
{
    "status": 200,
    "msg": "Success",
    "data": {
        "id": 2,
        "email": "user@gmail.com",
        "role": 4,
        "active": true,
        "profile": {
            "first_name": "Gagaz",
            "last_name": "Manqunazara",
            "nim": "2702254063",
            "birth_date": "2024-08-17T00:00:00.000Z",
            "region": 1,
            "faculty": 1,
            "major": 1,
            "line_id": "aind"
        }
    }
}
```

### Change User Role

* Endpoint : `/users/bulk/role`
* Method : `PUT`
* Request Body :
    - ids (Numbers[], Required)
    - role (Number, Required)

* Response Body :

```json
{
  "status": 200,
  "message": "Success update role!"
}
```

### Change User Active Status

* Endpoint : `/users/bulk/active`
* Method : `PUT`
* Request Body :
    - ids (Numbers[], Required)
    - active (Number, Required)
    
* Response Body :

```json
{
  "status": 200,
  "message": "Success update active!"
}
```
