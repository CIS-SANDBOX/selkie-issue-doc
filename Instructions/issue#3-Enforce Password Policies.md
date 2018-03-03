Passwords sent to the backend must meet the following complexity requirements.

- Use a password length of minimum 6 and maximum of 8 characters.
- Password must contain both lowercase and uppercase characters.
- Password must contain at least one of the following  non alphanumeric characters:
         ~!@#$%^&*_-+=`|\(){}[].?

- Password must be hashed before save

If the password is not set, you should randomly generate a password, that meet the above complexity requirements.

**Response schema**

**400 Bad Request:** If the password complexity requirement is not met.

```
{
    "status": 400,
    "message": "Password complexity requirement not met",
    "developerMessage": "User creation failed because password complexity requirement not met"
}
```
