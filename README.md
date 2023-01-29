# NodeJS back-end for JWT Login with Token

### Environment variable
Create file in root path with name **.env** and add configuration environment variables.
```text
API_PORT=4001
TOKEN_KEY=AppSecretKeyHere
MONGO_URI=mongodb+srv://....
```

### Register User
- POST - http://localhost:4001/register
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
- POST - http://localhost:4001/login
- @Request Body
```json
{
    "email":"email@correo.com",
    "password":"XXXXXXXX"
}
```