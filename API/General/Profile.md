# Profile

---

### Create Profile

* Endpoint : `/profiles`
* Method : `POST`
* Request Body :

  - first_name (String, Required)
  - last_name (String, Required)
  - nim (Number, Required)
  - birth_date (Date, Required)
  - region (String, Required)
  - faculty (String, Required)
  - major (String, Required)
  - line_id (String, Optional)

* Response Body :

```json
{
  "status": 200,
  "message": "Success",
  "data": {
    "first_name": "john",
    "last_name": "doe",
    "nim": "123456",
    "birth_date": "1995-05-05",
    "region": "Bandung",
    "faculty": "Engineering",
    "major": "Computer Science",
    "line_id": "john_doe123"
  }
}
```

### Get Regions

* Endpoint : `/profiles/options/regions`
* Method : `GET`

* Response Body :

```json
{
  "status": 200,
  "msg": "Success",
  "data": [
    {
      "id": 1,
      "label": "Kemanggisan"
    },
    {
      "id": 2,
      "label": "Alam Sutera"
    },
    {
      "id": 3,
      "label": "Bandung"
    },
    {
      "id": 4,
      "label": "Malang"
    }
  ]
}
```

### Get Faculties

* Endpoint : `/profiles/options/regions/:regionId/faculties`
* Method : `GET`

* Response Body :

```json
{
  "status": 200,
  "msg": "Success",
  "data": [
    {
      "id": 1,
      "label": "SOCS"
    },
    {
      "id": 2,
      "label": "SOIS"
    },
    {
      "id": 3,
      "label": "SOD (School of Design)"
    },
    {
      "id": 4,
      "label": "BINUS Business School Undergraduate Programs"
    },
    {
      "id": 5,
      "label": "School of Accounting"
    },
    {
      "id": 6,
      "label": "Faculty of Digital Communication and Hotel & Tourism"
    },
    {
      "id": 7,
      "label": "Faculty of Humanities"
    },
    {
      "id": 8,
      "label": "Faculty of Engineering"
    },
    {
      "id": 9,
      "label": "Double Programs"
    },
    {
      "id": 10,
      "label": "Master Track Programs"
    }
  ]
}
```

### Get Majors

* Endpoint : `/profiles/options/regions/:regionId/faculties/:facultyId/majors`
* Method : `GET`

* Response Body :

```json
{
  "status": 200,
  "msg": "Success",
  "data": [
    {
      "id": 1,
      "label": "Artificial Intellegence"
    },
    {
      "id": 2,
      "label": "Cyber Security"
    },
    {
      "id": 3,
      "label": "Game Application and Technology"
    },
    {
      "id": 4,
      "label": "Computer Science"
    },
    {
      "id": 5,
      "label": "Data Science"
    }
  ]
}
```
