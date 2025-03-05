# Auth Manager

This repository contains the Docker setup for running a standalone Keycloak authentication service.

## Prerequisites

Ensure you have the following installed on your system before proceeding:

- [Docker](https://docs.docker.com/get-docker/)

## How to Run Keycloak

To start the Keycloak container, simply run:

```sh
docker-compose up -d
```

## Custom Themes

The custom themes are located in:

`/keycloak/themes/library-management-theme`

They are automatically copied to the Keycloak instance during the build process.

## Accessing Keycloak

Once the container is running, open your browser and navigate to:

- **Admin Console:** [http://localhost:8045/admin](http://localhost:8045/admin)
- **User Authentication:** [http://localhost:8045/realms/master/account](http://localhost:8045/realms/master/account)

### Admin Credentials

- **Username:** admin
- **Password:** YourPassword

## Stopping and Removing the Container

To stop the running container:

```sh
docker-compose down
```

## Logs and Debugging

To view the logs of the running container:

```sh
docker-compose logs -f
```