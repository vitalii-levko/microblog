# microblog
Advanced microblog app with Flask

## Prerequisites
* Python 3.7.0
* Flask 0.12.4
* flask-sqlalchemy
* flask-migrate
* flask-login
* flask-mail
* pyjwt
* flas-bootstrap

## Getting Started
### Linux
```bash
cd microblog
export FLASK_APP=microblog.py
flask run
```

### Windows
```bash
cd microblog
set FLASK_APP=microblog.py
flask run
```

Username/Password
* susan/cat
* john/dog

## Error Handling
Use `export` on Linux instead of `set` on Windows.

### Debug Mode
```bash
set FLASK_DEBUG=1
flask run
```

### SMTP Debug Server
Open separate terminal window and run
```bash
python -m smtpd -n -c DebuggingServer localhost:8025
```

In the main terminal window run
```bash
set MAIL_SERVER=localhost
set MAIL_PORT=8025
set FLASK_DEBUG=0
flask run
```

### SMTP-server
```bash
set MAIL_SERVER=smtp.googlemail.com
set MAIL_PORT=587
set MAIL_USE_TLS=1
set MAIL_USERNAME=<your-gmail-username>
set MAIL_PASSWORD=<your-gmail-password>
flask run
```

Note: make sure to be aware of [Google account access](https://support.google.com/accounts/answer/6010255?hl=en).
