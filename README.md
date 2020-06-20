# OAuth 2.0 Client

Sample OAuth 2.0 Client using Flask.

Server: https://github.com/ameyrupji/python-flask-oauth2-server

You will need to create the Client with the following configurations: 
```
{
    "client_name": "127.0.0.1:5001", 
    "client_uri": "http://127.0.0.1:5001/", 
    "grant_types": ["authorization_code", "password"], 
    "redirect_uris": ["http://127.0.0.1:5001/auth"], 
    "response_types": ["code", "id_token"], 
    "scope": "openid email profile", 
    "token_endpoint_auth_method": "client_secret_basic"
}

```

### Commands
```
python3 -m venv venv
source venv/bin/activate
pip3 install -r requirements.txt

# Disable SSL (only for development)
export AUTHLIB_INSECURE_TRANSPORT=1

export FLASK_APP=website/run.py
flask run --port=5001

# to exit from venv
deactivate
```


http://127.0.0.1:5001/

## Useful Links

- https://github.com/authlib/demo-oauth-client/tree/master/flask-google-login
- Flask (Python) - Google oAuth 2.0 (Authlib) -https://www.youtube.com/watch?v=BfYsdNaHrp
