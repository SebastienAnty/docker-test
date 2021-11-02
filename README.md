# Simple Express App wrapped in Docker

This was to demonstrate how to create a Docker image and container from a simple app.

## Docker commands:

`docker ps`
Show containers that are running.

`docker build -t myimagename:1.0.1 .`
Builds a docekr image from the Dockerfile in the current folder using tag "myimagename:1.0.1" .

`docker run -p 5050:8080 myimagename:1.0.1`
Runs the docker image

`docker run - p 5050:8080 -v /Users/myuser/code/myproject/:/src/ myimagename:1.0.1`
Runs docker image with volume mapped to local folder.

`docker kill (first three characters)`
Kills the container with the Container ID beginning with (first three characters).