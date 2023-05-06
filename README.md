AirBnB Clone: Phase # 3
: API with Swagger

Description

Project attempts to clone the the AirBnB application and website, including the database, storage, RESTful API, Web Framework, and Front End. Currently the application is designed to run with 2 storage engine models:

File Storage Engine:

/models/engine/file_storage.py
Database Storage Engine:

/models/engine/db_storage.py

To Setup the DataBase for testing and development, there are 2 setup scripts that setup a database with certain privileges: setup_mysql_test.sql & setup_mysql_test.sql (for more on setup, see below).

The Database uses Environmental Variables for tests. To execute tests with the environmental variables prepend these declarations to the execution command:

$ HBNB_MYSQL_USER=hbnb_test HBNB_MYSQL_PWD=hbnb_test_pwd \
HBNB_MYSQL_HOST=localhost HBNB_MYSQL_DB=hbnb_test_db HBNB_TYPE_STORAGE=db \
[COMMAND HERE]
Environment

OS: Ubuntu 14.04 LTS
language: Python 3.4.3
web server: nginx/1.4.6
application server: Flask 0.12.2, Jinja2 2.9.6
web server gateway: gunicorn (version 19.7.1)
database: mysql Ver 14.14 Distrib 5.7.18
documentation: Swagger (flasgger==0.6.6)
style:
python: PEP 8 (v. 1.7.0)
web static: W3C Validator
bash: ShellCheck 0.3.3

