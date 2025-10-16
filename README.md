# README APCV 405 Class Project

This project is an automated pipleine using Jenkins that uses code from the apcv_405_app repository. This project does the following:

1. Pulls code from the apcv_405_app GitHub repository.
2. Runs the automated tests.
3. Builds a Docker image.
4. Pushes the created image to DockerHub.
5. Deploys the container on the users local machine.
6. Finally it performs health checks.

### Manual Deployment
```bash
docker pull jzarnold/jzarnold-apcv_405_app:latest
docker run -p 9090:8080 jzarnold/jzarnold-apcv_405_app:latest
