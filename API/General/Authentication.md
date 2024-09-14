# Authentication

---

### Login

* Endpoint : `/login`
* Method : `POST`
* Request Body :
  - `email` (String, Required)
  - `password` (String, Required)

* Response Body :

```json
  {
    "status": 200,
    "message": "Success",
    "error": "",
    "data": {
      "token": "my-token-here",
      "role": 1,  
      "email": "example@gmail.com"
    },
  }
```

---

### Register

* Endpoint : `/register`
* Method : `POST`
* Request Body :
  - `email` (String, Required)
  - `Password` (String Required)

* Respones Body :

```json
  {
    "status": 200,
    "msg": "Success",
    "data": {
        "email": "user5@gmail.com",
        "role": 4,
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6InVzZXI1QGdtYWlsLmNvbSIsInJvbGUiOjQsImlhdCI6MTcyNjA1ODM3OX0.nU1uAbn72VLs-xg5jgHQMSSz8mwyK7DElQiwcdXNNhQ"
    }
  }