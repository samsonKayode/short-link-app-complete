# ShortLink App

This application is a url shortener. It accepts a long url from the user and returns a shorter url.

There are two projects in this repo. I made them submodules of this main app, but you can download the frontend and the backend individually.

I made them submodules so you can run the app using docker-compose.

Repo for Backend: https://github.com/samsonKayode/url-shortener-backend.git

Repo for Frontend: https://github.com/samsonKayode/url-shortener-ui.git

###Stacks used:

<b><u>Backend</u></b>

1. Spring Boot Java
2. H2 Database (I used H2 for simplicity because I didn't want the startup time to be longer as the docker-compose will have to download a db container if I had used any)
3. Guava was used for the hashing of the long urls

<b><u>Frontend</u></b>

Thymeleaf (Java)

The entry point for a user is a website which is available under the address: ***http://localhost:7001/***

### How To Run The Project

####In order to run this application you need to install two tools: Docker & Docker Compose.

The entire application can be run with a single command on a terminal:

```
$ docker-compose up -d
```

If you want to stop it, use the following command:

```
$ docker-compose down
```

#### Backend (REST API)

This is a Spring Boot (Java) based application that connects with a
database that and expose the REST endpoints that can be consumed by
frontend.

Full list of available REST endpoints could be found in Swagger UI,
which can be accessed via: **http://localhost:8080/api/swagger-ui.html**




