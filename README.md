# Voi docker-relay-node guide

## Steps:

Clone the Repository: Open your terminal and run:

```
git clone https://github.com/VoiNetwork/docker-relay-node.git
cd docker-relay-node
```

Build the Docker Image: Inside the project directory, build the Docker image:

```
docker build -t voi-relay-node .
```

Run the Container: Start the relay node by running the container:

```
docker run -d --name voi-relay-node -p 30303:30303 voi-relay-node
```

This command runs the relay node in detached mode, exposing the required ports.

Verify the Node: Ensure the node is running correctly by checking the logs:

```
docker logs -f voi-relay-node
```

The logs should indicate successful connections.

## Docker Commands Explained:
- docker build: Compiles the Docker image using the provided Dockerfile.
- docker run: Runs the container based on the image.
- docker logs: Shows real-time logs from the running container.
  
Customization:

You can modify environment variables or network settings as needed by editing the Dockerfile or passing options to the docker run command.
