Step1: Install Mongodb community Server Edition

Step 2: Connect 


Step 3: Install npm and node js

Step 4: Install dependencies
- npm init -y
- npm install express mongoose bcryptjs jsonwebtoken dotenv
- npm install --save-dev nodemon


Step 5: Start application
- npm start → runs your app normally with Node.js (ideal for production or Docker)

- npm run dev → runs your app with nodemon (ideal for local development)

Step 6:

Install postman
https://www.postman.com/downloads/

Step 7: Test in Postman
- Register

POST http://localhost:5000/api/auth/register

{
  "email": "test@example.com",
  "password": "123456"
}

- Login: You should get a JWT Token on successful login

POST http://localhost:5000/api/auth/login

{
  "email": "test@example.com",
  "password": "123456"
}






