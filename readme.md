# Laravel with Passport Authentication

Basically this is a starter kit for you to integrate Laravel with Passport Authentication

## Quick Start

- Clone this repo or download it's release archive and extract it somewhere
- You may delete .git folder if you get this code via git clone
- Run composer install
- Configure your .env file for authenticating via database
- Run docker-compose build
- Run docker-compose up -d
- Run the following command to populate database tables.

	```bash
	$ docker-compose exec php php artisan migrate
	```

- Visit `localhost:9008`

> **Note:**
- You can now use:

- ```POST /api/auth/signup``` –> Create user 

    ```json
    {
    	"name" : "Test User ",
    	"email" : "test@gmail.com",
    	"password" : "secret",
    	"password_confirmation" : "secret"
    
    }

     ```
     
     
- ```POST /api/auth/login``` –> with email and password, obtain a access token

      

- ```GET /api/auth/user``` –> Get user info



And remember, Passport requires you to provide the token as a header.