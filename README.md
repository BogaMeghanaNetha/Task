# Node.js CI/CD App

This is a simple Node.js application demonstrating a CI/CD pipeline with Docker.

## Description

A basic Express app that responds with a friendly message, showing the CI/CD pipeline is working correctly.

## Features

- Built with Node.js and Express
- Containerized with Docker
- Listens on port 3000
- Responds with "Hello Meghana! Your CI/CD pipeline works 🚀"

## Prerequisites

- Docker installed on your machine or server
- (Optional) Docker Hub account to push/pull images
- AWS EC2 instance or any cloud server for deployment

## How to Run Locally with Docker

1. **Clone the repo**  
   ```bash
   git clone https://github.com/BogaMeghanaNetha/Task.git
   cd <repo-folder>
````

2. **Build the Docker image**

   ```bash
   docker build -t meghananetha/nodejs-cicd-app .
   ```

3. **Run the Docker container**

   ```bash
   docker run -d -p 3000:3000 meghananetha/nodejs-cicd-app
   ```

4. **Access the app**
   Open your browser and visit:

   ```
   http://localhost:3000
   ```

   or if running on EC2:

   ```
   http://<your-ec2-public-ip>:3000
   ```

## Docker Hub

The image is published on Docker Hub at:

```
docker pull meghananetha/nodejs-cicd-app
```

## Troubleshooting

* Ensure port `3000` is open in your firewall or EC2 security group.
* Confirm the app listens on `0.0.0.0` for external access.
* Check container logs with:

  ```bash
  docker logs <container-id>
  ```
