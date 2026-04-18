FROM golang:1.16.5-alpine
# WORKDIR /code
#    HOST <CONTAINER-PATH>
COPY . /code


ENTRYPOINT [ "go" ]
CMD [ "run", "/code/src/app.go" ]