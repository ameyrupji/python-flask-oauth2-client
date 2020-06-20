# OAuth 2.0 Client

Sample OAuth 2.0 Client using Flask.

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