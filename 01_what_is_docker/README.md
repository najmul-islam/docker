### What is Docker and Why Use It?
Docker is an open platform that enables developers to build, ship, and run applications inside containers. It ensures consistency across different environments, eliminating issues like "it works on my machine." Containers allow applications to run in isolation, packaging software along with its dependencies.

### Advantages of Docker
Docker provides several benefits:
- **Portability**: Applications packaged in containers can run across various environments consistently.
- **Efficiency**: Containers are lightweight compared to virtual machines (VMs), making them more efficient in terms of system resources.
- **Consistency**: It ensures that code behaves the same way across development, testing, and production environments.
- **Fast Deployment**: Containers are quick to create and deploy, enabling faster continuous integration and delivery (CI/CD) pipelines.

### Dockerfile
A Dockerfile is a script that defines the steps to build a Docker image. It includes the necessary instructions to set up the environment and dependencies required for an application to run in a container.

### Docker Image
A Docker image serves as a template for creating containers. It is a read-only file containing the application code and all necessary dependencies for the container.

### Docker Container
A Docker container is a running instance of a Docker image. It encapsulates the application, ensuring it runs with the required dependencies in an isolated environment.

### Docker Compose
Docker Compose is a tool used to define and manage multi-container Docker applications. By using a YAML configuration file (`docker-compose.yml`), you can manage services, networks, and volumes for applications that run across multiple containers.

### Container Registry
A container registry is a repository where Docker images are stored and distributed. Popular registries like Docker Hub allow you to store, share, and retrieve images to be used in different environments.

### Docker Container Registry
Docker Hub is an example of a container registry that serves as a central location for users to upload and download Docker images.

### Base Image
A base image is the foundational layer for creating a Docker image. It usually contains the minimal operating system or framework required to build an application, which can then be layered with custom components.

### Creating Docker Images and Containers
Docker images are built using a Dockerfile with the `docker build` command. Once built, containers can be created and run using the `docker run` command.

### Docker Containers vs Virtual Machines
The main difference between Docker containers and virtual machines lies in resource usage and efficiency. Containers share the host OS kernel, making them lighter and faster to start, while virtual machines run their own OS, requiring more resources and creating additional overhead.