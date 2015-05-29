# What it inside
This is a simple example of a dockerized web app in python.

# How to Execute
- Build the image: `docker build -t my-web-app .`
- Run the container: `docker run -p 80:8080 -v $(pwd)/app:/usr/app --name app-instance my-web-app`
- Inspect inside the container: `docker exec -ti app-instance /bin/bash`

# Use the app
Browse http://<docker-host-ip>
