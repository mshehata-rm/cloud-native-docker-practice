FROM golang:1.16.5-alpine as build
WORKDIR /code

#    HOST <CONTAINER-PATH>
COPY . /code

RUN go build src/app.go
# generate "app"

## Option 1
# ENTRYPOINT [ "go" ]
# CMD [ "run", "/code/src/app.go" ]

## Option 2
# CMD [ "go", "run", "/code/src/app.go" ]

FROM alpine:3.14 as runtime
COPY --from=build /code/app .
CMD ["./app"]
# COPY build (previous build) to /code/app (absolute path)


#  FROM base-builder  as build
#  COPY . .
#  RUN <build-compile-package>
#  ......

# FROM base-runtime  as runtime
# COPY --from=build /code/artifact /path
# ENTRYPOINT /path/app
