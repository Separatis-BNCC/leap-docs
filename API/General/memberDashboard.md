# Member Dashboard

---

### Get Member Profile

* Endpoint : `/members/profiles`
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
            "id": 2,
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

### Edit Member Profile

* Endpoint : `/members/profiles`
* Method : `PUT`

* Response Body :

```json
{
    "status": 200,
    "msg": "Success",
    "data": "Success edit profile with id 1!"
}
```
