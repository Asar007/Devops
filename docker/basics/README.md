# Docker Hello-World Basics

This directory contains a minimal example to introduce Docker container basics using a lightweight Alpine Linux image.

## 1. What this Dockerfile does

* **`FROM alpine:latest`**: Pulls the Alpine Linux image (approx. 5MB) from the Docker Hub to act as the base OS.
* **`CMD [...]`**: Defines the default command that runs when the container starts. Here, it simply prints a welcome message to the terminal.

## 2. How to Build and Run

### Step 1: Build the Image
Navigate to the `docker/basics/` directory and run the following command to package the Dockerfile into an image named `hello-docker`:

```bash
docker build -t hello-docker 
```
### Step 2: Run the Container
Once the build is complete, run an instance of the image:
```bash
docker run hello-docker
```
### Expected Output<br>
You should see the following message in your terminal:
```Plaintext
Hello, World! Welcome to your first Docker container.
```
