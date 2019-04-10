# cnj-docker-keycloak

A pre-configured KeyCloak instance packaged as a ready-to-go Docker image for the CloudTrain showcases using OpenID Connect Security.

## Build this Docker image 

### Prerequisites

In order to run the build, you have to install the following tools locally:
* Docker
* Docker Compose 
* Maven
* Java JDK 8

### Run Maven

You can build the Docker images by running Maven:
```
mvn clean install 
```

The Maven build will create a Docker image named __hmfwpcnj/cnj-docker-keycloak__.

## Run this Docker image

Since the whole Docker container stack required to run a pre-configured KeyCloak instance consists of three Docker containers
plus one Docker volume, it is recommended to run the KeyCloak instance using docker-compose.

A sample docker-compose file is provided [here](src/test/docker/cnj-docker-keycloak/docker-compose.yml) 
