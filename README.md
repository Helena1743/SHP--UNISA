# Smart Health Predictive
## Getting Started
### Prerequisites
- Python 3 or higher
- Node.js v22.x or higher
- npm
- Docker Desktop

### Installing Required Modules
1. Navigate to the server directory.
2. Run the following command to install the necessary modules.  
```pip3 install -r requirements.txt```

### Server Setup
1. Navigate to the server directory and run:    
```fastapi dev main.py```
2. Go to http://127.0.0.1:8000/docs to interact with API

### Running the Client
1. Navigate to the client directory.
4. Install packages with npm and run the client.  
```npm install```  
```npm start```

### Database Setup (Docker Compose + Alembic)
1. Have Docker running in the background.
2. Navigate to the root directory.
3. Create the container with:      
```docker compose up -d```
4. Navigate to the server directory.      
5. Update your database to the latest version with the following command:   
```alembic upgrade head```

*ADDITIONAL NOTES*:    
 Run the following command to downgrade the database:     
**Warning**: This command will drop *ALL* existing tables and their associated data    
```alembic downgrade base```  
```alembic upgrade head```  
