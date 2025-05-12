Step 1: Install Docker: https://docs.docker.com/desktop/setup/install/windows-install/

Step 2: Create Dockerfile

Step 3: Change the connection string to this: This works for windows desktop alone: config/db.js
await mongoose.connect('mongodb://host.docker.internal:27017/simpleLoginDB');

Step 3: Build Docker Image
docker build -t techwithadedayo/simple-login-api:v1 .

Step 4: Run Container
docker run --rm -p 5000:5000 simple-login-api:v1

Step 5: sign up on DockerHub and create a repository

https://app.docker.com/signup?returnTo=https%3A%2F%2Fhub.docker.com%2Fsubscription%3Fplan%3Dindividual%26paid%3Dtrue

Step 5: Push image to DockerHub

docker push repository/image:tag