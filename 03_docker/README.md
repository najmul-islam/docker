### 1. **Check Docker Version**
```bash
docker --version
```
Displays the installed Docker version.

### 2. **Pull an Image from Docker Hub**
```bash
docker pull <image_name>
```
Downloads an image from Docker Hub. For example, to pull the Ubuntu image:
```bash
docker pull ubuntu
```

### 3. **List Docker Images**
```bash
docker images
```
Displays a list of all the Docker images available on your system.

### 4. **Run a Docker Container**
```bash
docker run <image_name>
```
Starts a new container from an image. For example, to run a container with the Ubuntu image:
```bash
docker run ubuntu
```

- To run a container interactively with a terminal session, use:
  ```bash
  docker run -it <image_name>
  ```

### 5. **List Running Containers**
```bash
docker ps
```
Shows the currently running containers. To list all containers (running and stopped):
```bash
docker ps -a
```

### 6. **Stop a Running Container**
```bash
docker stop <container_id>
```
Stops a running container. The container ID can be obtained from `docker ps`.

### 7. **Start a Stopped Container**
```bash
docker start <container_id>
```
Starts a container that was previously stopped.

### 8. **Restart a Container**
```bash
docker restart <container_id>
```
Restarts a running or stopped container.

### 9. **Remove a Container**
```bash
docker rm <container_id>
```
Deletes a stopped container.

### 10. **Remove an Image**
```bash
docker rmi <image_name_or_id>
```
Deletes an image from your local system.

### 11. **View Container Logs**
```bash
docker logs <container_id>
```
Displays the logs of a running or stopped container.

### 12. **Execute a Command Inside a Running Container**
```bash
docker exec -it <container_id> <command>
```
Allows you to run a command inside a running container. For example, to open a bash shell inside a container:
```bash
docker exec -it <container_id> bash
```

### 13. **Build an Image from a Dockerfile**
```bash
docker build -t <image_name> <path_to_dockerfile>
```
Builds a Docker image from a Dockerfile. For example:
```bash
docker build -t my-image .
```
The `.` specifies the current directory as the build context.

### 14. **Tag an Image**
```bash
docker tag <image_id> <new_image_name>:<tag>
```
Tags an image with a new name or version.

### 15. **Push an Image to Docker Hub**
```bash
docker push <image_name>
```
Pushes an image from your local system to Docker Hub (you must be logged in with `docker login`).

### 16. **Login to Docker Hub**
```bash
docker login
```
Logs you into your Docker Hub account to push or pull images.

### 17. **Inspect a Container**
```bash
docker inspect <container_id>
```
Displays detailed information about a container.

### 18. **Remove All Stopped Containers**
```bash
docker container prune
```
Deletes all stopped containers.

### 19. **Remove All Unused Images**
```bash
docker image prune
```
Deletes all unused Docker images from your local system.