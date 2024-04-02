# face-recognition-web-app (FRONTEND)
It is a full-stack working web application using Clarifai Web API for face detection in an image,using a website with frontend designed completely using React.js, server using Node.js and Express.js and PostgreSQL for database. Frontend of the application has been deployed to Vercel, backend to Heroku and for database I've used elephantSQL which is a hosted service for PostgreSQL.


### Steps to start:

1. Run `npm install`
    This will install all the dependencies.

2. Go to face-recognition-web-app/face-recognition-api
    This is the server i.e. the back-end for the application
    
3. Run `npm install`
    This will install all the dependencies.
    
4. We must add our own API key and Databse URI in the `face-recognition-web-app/face-recognition-api/.env` file to connect to Clarifai and our database. The name of the variables are available in .example.env file.

    
5. Run `npm start`
    This will run the server, on port 8000
    
6. Go to face-recognition-web-app/face-recognition-webapp and run `npm start`
    This will run the frontend, on port 3000
    
### Configuring Database:
I've used [ElephantSQL](https://www.elephantsql.com/) which is a hosted service for postgreSQL but you can create you local database as well.
1. Create a database face-recog (Or any other name you prefer)
2. Create a table named users, with following structure:
```
CREATE TABLE users (id SERIAL PRIMARY KEY, email TEXT UNIQUE NOT NULL, password TEXT NOT NULL, entries BIGNINT DEFAULT O);
```
3. Enter your server details in `face-recognition-web-app/face-recognition-api/.env` file.

#### Modules used:
1. [React](https://www.npmjs.com/package/react)
2. [Clarifai](https://www.npmjs.com/package/clarifai)
3. [Tachyons](https://www.npmjs.com/package/tachyons)
4. [Bcrypt](https://www.npmjs.com/package/bcrypt-nodejs)
5. [Cors](https://www.npmjs.com/package/cors)
6. [Express](https://www.npmjs.com/package/express)
7. [pg](https://www.npmjs.com/package/pg)
8. [Nodemon (devDependency)](https://www.npmjs.com/package/nodemon)
9. [React-particles-js](https://www.npmjs.com/package/react-particles-js)
