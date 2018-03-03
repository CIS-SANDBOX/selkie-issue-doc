HTTP POST request to http://localhost:8090/api/users should create a new user. 

**Request schema 1:**
```
{
    "email": "admin@letmehack.lk",
    "password": "password"
}
```
If the password is not set, you should randomly generate a password in the API backend.

**Response schemas:**

**Status 201:** Return if the user was successfully created.
```
{
    "self": "http://localhost:8090/api/users/{user_id}",
    "email": "admin@letmehack.lk"
}
```	
**Status 400:** Return if email is not set.

**Status 409:** If the user already exists.
```
{
    "status": 409,
    "message": "A user with email: {email} already exists.",
    "developerMessage": "User creation failed because the email: {email} already exists.",
}
```
**Request schema 2**
```
{
    "email": "admin@letmehack.lk"
}
```
Here the password is not set.

**Response schemas**

**Status 201:** Return if the user was successfully created.
```
{
    "self": "http://localhost:8090/api/users/{user_id}",
    "email": "admin@letmehack.lk"
}
```


**Note**
Placeholders {email}, {user_id} should contain actual values.

