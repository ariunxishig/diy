# README

/bitool_front

#FRONT_END
#React Typescript

/bitool_server

#SERVER_SIDE
#Django, Postgre, Rest API

## Manual build

### Start the Django API

```bash
cd bitool_server
# Create a virtual environment
virtualenv venv
source venv/Script/activate # For Windows
source venv/bin/activate #For Mac
# Install modules
pip install -r requirements.txt
#only support 3.6+ : Set new SECRET_KEY to your environment file by generating with below command, copy the output then paste it in your .env
python -c "import secrets; print(secrets.token_urlsafe())"
# Set Up the Database
python manage.py makemigrations
python manage.py migrate

# Set up the application tables
python manage.py makemigrations <name>
python manage.py migrate <name>


# Start the API
python manage.py runserver
```
