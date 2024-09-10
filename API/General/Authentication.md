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

### Login

(Bikin sendiri set)