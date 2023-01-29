# NodeJS back-end for JWT Login with Token

Create file in root path with name **.env** and add configuration environment variables.
```text
API_PORT=4001
TOKEN_KEY=AppSecretKeyHere
MONGO_URI=mongodb+srv://....
```

```json
POST - http://localhost:4001/register

@Request Body

{
    "first_name":"firstname",
    "last_name":"lastname",
    "email":"email@correo.com",
    "password":"XXXXXXXX"
}
```

```json
POST - http://localhost:4001/login

@Request Body
        
{
    "email":"email@correo.com",
    "password":"XXXXXXXX"
}
```