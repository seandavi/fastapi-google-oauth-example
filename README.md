## fastapi-google-oauth-example

1. set up your Google OAuth2.0 credentials
2. clone this repository
3. add your credentials to the `.env` file
4. run the app with `uvicorn main:app --reload`
5. visit `http://localhost:8000/` and click the "Login with Google" button
6. after successful authentication, you will be redirected to `http://localhost:8000/auth/callback` with the user information displayed


## Oauth2.0 authentication result
```json
{
  "message": "Authentication successful!",
  "user_info": {
    "sub": "112087074803117476966",
    "name": "Sean Davis",
    "given_name": "Sean",
    "family_name": "Davis",
    "picture": "https://lh3.googleusercontent.com/a/ACg8ocI2hyxWJy5zCcvl8iYri3gcVXgtz9qvVJag6toZoeHe6WH0PA=s96-c",
    "email": "sean.2.davis@cuanschutz.edu",
    "email_verified": true,
    "hd": "cuanschutz.edu"
  }
}
```