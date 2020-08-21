# udacity-microservice-project

In this repo, there are 4 services with containerization and kubernetes incorporated. 

They are:
- Frontend application
- Backend user service
- Backend feed service
- Reverse Proxy


2. Update the following configuration files
- [aws-secret.yaml](/udacity-c3-deployment/k8s/aws-secret.yaml)
- [env-configmap.yaml]/udacity-c3-deployment/k8s/env-configmap.yaml)
- [env-secret.yml](/udacity-c3-deployment/k8s/env-secret.yaml)


3. Update your .profile or .bash_profile with the values for the following environment variables
  - POSTGRESS_USERNAME 
  - POSTGRESS_PASSWORD
  - POSTGRESS_DB
  - POSTGRESS_HOST
  - URL=http://localhost:8100
  - AWS_REGION
  - AWS_PROFILE
  - AWS_BUCKET
  - JWT_SECRET
  - AWS_ACCESS_KEY_ID
  - AWS_SECRET_ACCESS_KEY

**Running the application**

1. Change working directory to the application e.g. `cd udacity-restapi-feed`

2. Install the dependencies for each project  `npm install` 


====================================================================================

1. Build the docker images

` docker-compose -f udacity-c3-deployment/docker/docker-compose-build.yaml build --parallel`

2. Run the container

`docker-compose up`

