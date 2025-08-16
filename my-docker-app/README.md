# My Docker App

This project is a simple Python application packaged in a Docker container. Below are the instructions on how to build and run the Docker image.

## Project Structure

```
my-docker-app
├── src
│   └── app.py
├── Dockerfile
├── requirements.txt
└── README.md
```

## Prerequisites

- Docker installed on your machine.

## Building the Docker Image

To build the Docker image, navigate to the project directory and run the following command:

```
docker build -t my-docker-app .
```

## Running the Docker Container

After building the image, you can run the Docker container using the following command:

```
docker run -p 5000:5000 my-docker-app
```

This will start the application and map port 5000 of the container to port 5000 on your host machine.

## Additional Information

For any additional information regarding the application logic, please refer to the `src/app.py` file. The dependencies required for the application are listed in the `requirements.txt` file.