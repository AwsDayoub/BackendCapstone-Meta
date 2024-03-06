# Assignment for Meta Backend Capstone
project for the Meta Back-End course with main focus on testing and connecting django with mysql server


## Commands

# create virtual environment
py -m venv venv
venv\Scripts\activate
# install all requirements
pip install -r requirements.txt
cd littlelemon



## Mysql server
```
create database littlelemon;
use littlelemon;
CREATE USER 'user1'@'localhost' IDENTIFIED BY '123';
GRANT ALL PRIVILEGES ON littlelemon.* TO 'user1'@'localhost';
```

## cmd
```
python3 manage.py migrate 
python3 manage.py makemigrations
python manage.py createsuperuser
#user:super
#password: 123
```

## APIs

http://localhost:8000/api/menu/1

http://localhost:8000/api/menu

http://localhost:8000/api/menu/

http://localhost:8000/api/booking/tables

http://localhost:8000/api/api-token-auth/

http://127.0.0.1:8000/auth/token/login/

# Testing
```
python manage.py test
```
# Mysql
```
GRANT ALL PRIVILEGES ON `test_littlelemon`.* TO 'user1'@'localhost';
FLUSH PRIVILEGES;```