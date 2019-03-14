Deployed on heroku:
https://young-taiga-72177.herokuapp.com

Endpoints:
POST /api/users
```
body: {
  "user": {
    "email": "diogo@mail.com",
    "password": "passwrd"
  }
}
...
response: {
    "user": {
        "_id": "5c8a85800da7dd0030f9473d",
        "email": "diogo@mail.com",
        "token": ...
    }
}
```

GET /api/users/current
```
headers: {
    "Authorization": "Token [token from previous response]",
    "Content-Type": "application/json"
}
...
response: {
    "user": ...
}
```
