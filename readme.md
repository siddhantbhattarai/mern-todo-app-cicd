# Installation
Run the following command to clone the repository
```
git clone https://github.com/siddhantbhattarai/mern-todo-app-cicd.git
```

# Configuration
Create ```.env``` file inside ```backend``` directory and copy the following code
```
MONGO_URI=Your mongodb URI
GMAIL_USERNAME=your gmail address 
GMAIL_PASSWORD=password created inside 'App Password' section under google accounts setting
PORT=8000
JWT_SECRET=a random secret key eg. thisisasecretkey
```

# Build the frontend
```
docker build -t mern-todo-app-frontend .
```

# Run the frontend app
```
docker run -p 3000:3000 mern-todo-app-frontend
```

# Build the backend
```
docker build -t mern-todo-app-backend .
```

# Run the backend app
```
docker run -p 8000:8000 mern-todo-app-backend
```

OR

# Run the container via docker compose
```
docker-compose up -d
```





