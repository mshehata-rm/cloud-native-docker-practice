# Static Website

Simple website

# Prerequisites

- docker compose reference v3 (Google it): https://docs.docker.com/reference/compose-file/services/
- docker

# Getting Started

dockerhub example dummy-data-example: https://hub.docker.com/r/abdennour/dummy-rest-api-example

```bash
# Add
curl -X POST -d '{"id": "a1234", "name": "name 1234", "inPark": "park 1234", "manufacturer": "man 1234", "height": 12}' http://localhost:8080/coasters -H "content-type: application/json"

# List
curl http://localhost:8080/coasters
```

`docker compose up -d`

`docker compose up -d --build --remove-orphans`

Navigate to http://localhost:7070

# Authors

- mshehata-rm