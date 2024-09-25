# Troubleshooting
If the app isn't running correctly, there could be several causes. Use the guidance below to troubleshoot these issues.

## Missing 'env.py' file
If the env.py file deletes itself, create a new one and paste the following code into it:

import os

os.environ.setdefault("IP", "0.0.0.0") \
os.environ.setdefault("PORT", "5000") \
os.environ.setdefault("SECRET_KEY", "any_secret_key") \
os.environ.setdefault("DEBUG", "True") // change to 'False' before submitting \
os.environ.setdefault("DEVELOPMENT", "True") \
os.environ.setdefault("DB_URL", "postgresql:///taskmanager")

## Uninstalled Programmes
If the various programmes laid out in requirements.txt uninstall, run each of the following console commands:

pip install blinker==1.8.2

pip install click==8.1.7

pip install Flask==2.2.2

pip install Flask-SQLAlchemy==2.5.1

pip install greenlet==3.1.0

pip install itsdangerous==2.2.0

pip install psycopg2==2.9.9

pip install SQLAlchemy==1.4.46

pip install Werkzeug==2.2.2

## PSQL 
When using PostgreSQL, enter the following console command in the terminal before using psql:

set_pg