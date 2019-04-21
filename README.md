# Login App

This is a login app using Google oAuth 

# Tech Stack

- NodeJS 
- ExpressJS
- PassportJS
- MongoDB 
- Mongoose
- React 
- Redux

# Demo

https://glacial-basin-46981.herokuapp.com/

### Getting Started

## Prerequisites
Make sure you installed these on your machine
- Node (https://nodejs.org/en/)
- NPM (https://www.npmjs.com/get-npm)
- Nodemon (https://www.npmjs.com/package/nodemon)

And create accounts to get acceess to the required Keys mentiond in config/prod.js

- Google Devlopers account and Enable Google+ Api (https://console.developers.google.com)
- Create a new cluster and get the connection string (https://www.mongodb.com/cloud/atlas)

## Set Up
Clone and install:

```bash
git clone https://github.com/hemanth09/login-oauth.git
cd login-oauth
npm install

cd client
npm install
```

## Setup enviornment variables
Once you create the acounts on Google and cluster in MongoDb Atlas, You need to create a new dev.js file in config folder with respective keys

```bash
cd config
touch dev.js
```

Add the code below in dev.js with your keys
```
module.exports = {
    googleClientID: '',
    googleClientSecret: '',
    mongoURI: '',
    cookieKey: 'type any long random key with letters and numbers'
}
```

### Running the Application

Run it using:

Go to your root directory and

```bash
npm run dev
```
This will concurrently runs both your server and client

And in browser App will running on http://localhost:3000/

Api server is on http://localhost:5000/