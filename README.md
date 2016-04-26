# Dockerfiles
A collection of my favorite Dockerfiles for quick app deployment

### Running a Dockerfile:

All Dockerfiles are built to be executed via the following commands:

```sh
docker build -t my-docker-app
docker run -d -P my-docker-app
```

If running locally, you can visit the Docker Container by running the following command:

```sh
# Displays the list of running apps
docker ps -a
```

Under the column for `PORTS`, you will find the PORT value. Replace the domain with the IP of your currently running `docker-machine`. This can be found by running the following command:

```sh
# Replace VM_NAME with the name of the running VM (i.e. default)
docker-machine ip VM_NAME
```
