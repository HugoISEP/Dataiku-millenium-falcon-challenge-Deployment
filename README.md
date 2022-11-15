# Dataiku challenge: Deployment

The aim of this project is to manage the deployment of the frontend and backend to the server using [Docker](https://www.docker.com/)


## Frontend

To launch the frontend developed with react, we need to copy the build directory (built during the CI) and thanks to the `serve` dependency launch the web server on the port 3000

## Backend

For the backend, the .jar file containing all the code is used to launch the docker container with the resources files

## Deployment

The docker compose file will then launch the frontend and the backend and attach its two services to the `"global-network"` where the reverse proxy managing the incoming requests of the server is present

