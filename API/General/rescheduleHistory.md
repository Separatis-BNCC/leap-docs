# Reschedule History

---

### Create Reschedule History

* Endpoint : `/reschedule-history`
* Method : `POST`
* Request Body :

  - class_session_id (Number, Required)
  - class_id (Number, Required)
  - schedule (Date, Required)

* Response Body :

```json
{
    "status": 200,
    "msg": "Success",
    "data": {
        "id": 7,
        "approved": 0,
        "schedule": "2008-09-17T20:14:07.000Z",
        "class_session_id": 1,
        "class_id": 1
    }
}
```

### Get Reschedule History

* Endpoint : `/reschedule-history/:reschedule-historyId`
* Method : `GET`

* Response Body :

```json
{
    "status": 200,
    "msg": "Success",
    "data": {
        "id": 7,
        "approved": 0,
        "schedule": "2008-09-17T20:14:07.000Z",
        "class_session_id": 1,
        "class_id": 1
    }
}
```

### Edit Reschedule History

* Endpoint : `/reschedule-history/:reschedule-historyId`
* Method : `PUT`
* Request Body :

  - schedule (Date, Required)
  - approved (Number, Required)

* Response Body :

```json
{
    "status": 200,
    "msg": "Success",
    "data": "Reschedule History Updated!"
}
```

### Delete Reschedule History

* Endpoint : `/reschedule-history/:reschedule-historyId`
* Method : `DELETE`

* Response Body :

```json
{
    "status": 200,
    "msg": "Success",
    "data": "Reschedule History with id 6 successfully deleted!"
}
```
