# Passport-Tutorial

Node.js authentication tutorial using Passport.js

### Prerequisites

Make sure you have these installed on your machine

* [Node.js](https://nodejs.org/en/download/)
* [MongoDB](https://www.mongodb.com)
* **npm** This comes with Node.js, but make sure you check if you have it anyway

### Installing packages

Install packages

```
npm i
```

### Set up mongo docker image

```
$ docker pull bitnami/mongodb:latest
$ docker run -p27017:27017 --name mongodb  bitnami/mongodb:latest
```

### Running the app


To run the app (dev. mode)

```
npm start
```

To add a user post a request to the user authentication server

```
Header
Content-type: application/json

Body:
{
  "user": {
    "email": "something@whatever.com",
    "password": "password"
	}
}

```

To use the login page redirect from your client app with the param to redirect back to

e.g.

```
localhost:8000?redirect=localhost:8080/myapp.html
```

## Built With

* [Node.js](https://nodejs.org) - The backend framework used
* [Express.js](https://github.com/expressjs/express) - Node.js framework used
* [MongoDB](https://www.mongodb.com/) - Database platform used


## Authors

* **Antonio Erdeljac** - *Initial work* - [Passport-Tutorial](https://github.com/AntonioErdeljac/Blog-Tutorial)

## Acknowledgments

* This was a tutorial for my [Medium article](https://medium.com/p/4a56ed18e81e)
