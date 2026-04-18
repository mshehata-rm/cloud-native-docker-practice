# Go Simple App

This is a webapp with 2 simple endpoints:
- /hello
- /headers

# Prerequisites:

<!-- - Go (1.16 or above) -->
- Docker (20.10)

# Getting Started

<!-- `go run src/app.go` -->

`docker-compose up -d`

For building the image for the app service

`docker-compose build app`

We use `docker-compose build app`:
  - you changed Dockerfile
  - you want to rebuild only one service
  - you’re debugging build issues

then run docker-compose

`docker-compose up -d`

For debugging and see our dokcer shell inside of the container (ignore entrypoint)

`docker run -it --entrypoint sh go-hello-app`

For hot reload or hot debug:

`docker-compose restart app`

<!-- Then navigate to http://localhost:8090 -->
Then navigate to http://localhost:8099