# Getting Started


## Install Dependencies

- To get started, first install yarn from npm using `npm install --global yarn`.

- Once installed,  run `yarn install` to install all packages and dependencies.


## Database Setup

- Our MongoDB database is going to be running locally for the development of this project. First, open Docker Desktop and wait for Docker engine to initialise.

- With Docker running, enter the following command in the terminal; `docker run -p 127.0.0.1:27017:27017 --name mymongo -d mongo`

- Docker will now spin up a new instance on MongoDB.

- The connection string for MongoDB is `mongodb://localhost:27017`


## Running the API

- With the database connection setup, create a copy of the .env.example file and rename it to .env.

- Inside the .env file, set `MONGODB_URI=mongodb://localhost:27017` and `PORT=8000`

- In the terminal, run the command `yarn dev`

That's it!