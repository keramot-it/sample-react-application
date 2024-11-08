# Deploying sample React with Docker:

## Building a Docker Image


```bash
docker build -t react-application .
```

## Running the Docker Container


```bash
docker run -d -p 3000:3000 react-application
```

This command starts a Docker container and maps port 3000 from the container to port 3000 on your local machine. The `react-application` parameter specifies the name of the Docker image that we want to run.

With the `-d` flag, the command returns the ID of the container once it's started.

You can also use the `docker ps` command to see a list of running containers, including the ID of the container running your React application.

To stop the container, you can use the `docker stop` command followed by the container ID

```bash
docker stop <container_id>
docker stop 004e442ec862
```