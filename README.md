# Nginx load balancer example

This repo contains a simple python app, scaled up to multiple instances, which load is balanced by Nginx between different servers built on Docker containers.

## Usage:

After cloning the repo, run the following command to build the image and up the compose wih three instances of the app:

```bash	
docker-compose up -d --build --scale app=3
```

After that, you would be able to check the app on any browser, accessing localhost. It then will show the Container ID the load balancer has picked to serve the app.