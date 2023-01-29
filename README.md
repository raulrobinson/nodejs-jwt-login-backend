# NodeJS back-end for JWT Login with Token

### Environment variable
Create file in root path with name **.env** and add configuration environment variables.
```text
API_PORT=4001
TOKEN_KEY=AppSecretKeyHere
MONGO_URI=mongodb+srv://....
```

### Register User
- POST - http://localhost:4001/api/v1/auth/register
- @Request Body
```json
{
    "first_name":"firstname",
    "last_name":"lastname",
    "email":"email@correo.com",
    "password":"XXXXXXXX"
}
```

### Login User
- POST - http://localhost:4001/api/v1/auth/login
- @Request Body
```json
{
    "email":"email@correo.com",
    "password":"XXXXXXXX"
}
```

### Access Protected Content with JWT Token

- GET http://localhost:4001/api/v1/user-content
- @Request Header
```json
x-access-token
eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VyX2lkIjoiNjNkNjZhZjM1OGEyYzE1N2M0Y2I4MTQwIiwiZW1haWwiOiJyYXN5c2JveEBob3RtYWlsLmNvbSIsImlhdCI6MTY3NTAwMDQ4NCwiZXhwIjoxNjc1MDA3Njg0fQ.YP0uLuQ6cPBtVnn2gNkdt4D-8pVc2q8Fm5nGMcKj-pI
```

- @Response Status: 200 OK
- Welcome 🙌