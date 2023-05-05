# Cinema API Installation via GitHub:

- Clone the repository:

        git clone https://github.com/VladyslavCherkashyn/cinema-drf-api
## Set up a virtual environment:
	
- For Windows OS:
        python -m venv venv
        source venv/Scripts/activate

- For macOS:
        python3 -m venv venv
        source venv/bin/activate

- Install the dependencies:
        pip install -r requirements.txt
        Set up environment variables for the database connection and secret key:

set DB_HOST= your_db_hostname  
set DB_NAME= your_db_name  
set DB_USER= your_db_username  
set DB_PASSWORD= your_db_user_password  
set SECRET_KEY= your_secret_key  

## Run database migrations:

    python manage.py migrate
	
## Start the development server:

    python manage.py runserver

# Cinema API Installation via Docker:
- just run this two commands:

        docker-compose build
        docker-compose up

# Getting Access
- To get access to Cinema Service API, you need to create a user account and obtain an access token.

**User creating** - send a POST request to /api/user/register/  
**Obtain token** - send a POST request to /api/user/token/


## Features
- JWT authenticated
- Documentation is located at /api/doc/swagger/
- Managing orders and tickets
- Creating movies with genres, actors, cinema halls
- Adding movie sessions
- Filtering movies and movie sessions

