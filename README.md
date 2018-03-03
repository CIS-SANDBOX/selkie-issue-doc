# selkie-issue-doc

**Available Issues**

1. [Get the API up and running](https://github.com/CIS-SANDBOX/selkie-issue-doc/issues/1)
2. [Implement POST /users](https://github.com/CIS-SANDBOX/selkie-issue-doc/issues/2)
3. [Enforce Password Policies](https://github.com/CIS-SANDBOX/selkie-issue-doc/issues/3)
4. [Add property mobile to User](https://github.com/CIS-SANDBOX/selkie-issue-doc/issues/4)
5. [Add property role to User](https://github.com/CIS-SANDBOX/selkie-issue-doc/issues/5)
6. [Send the password to the user upon registration](https://github.com/CIS-SANDBOX/selkie-issue-doc/issues/6)
7. [Integrate Swagger UI](https://github.com/CIS-SANDBOX/selkie-issue-doc/issues/7)
8. [Implement POST /faculties](https://github.com/CIS-SANDBOX/selkie-issue-doc/issues/8)

There is no specific order for completing issues, however it would be much easier if you try complete them in sequence.

**Request/Response Format**

All requests and responses must be in JSON, with the `Content-Type` header set to `application/json`.

**Error Handling**

For API to be consistent, always return error responses in json. JSON schema of the errors returned should be like the following:

```
{
  "status": 401,
  "message": "Invalid username or password.",
  "developerMessage": "Login attempt failed because the specified password is incorrect."
}
```
