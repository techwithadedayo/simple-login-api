Step 1: Install Docker

Step 2: Create Dockerfile
https://docs.docker.com/desktop/setup/install/windows-install/

Step 3: Change the connection string to this: This works for windows desktop alone: config/db.js
await mongoose.connect('mongodb://host.docker.internal:27017/simpleLoginDB');

Step 3: Build Docker Image
docker build -t simple-login-api:v1.0 .

Step 4: Run Container
docker run --rm -p 5000:5000 simple-login-api:v1.0

