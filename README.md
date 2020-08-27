# FastAPI simple demo

A dockerized FastAPI simple demo

## Deploy

```
$ docker build --tag fastapi:latest .
```

### Run

```
$ docker run --name fastapi-test -p 5000:80 fastapi:latest

```

### Stop

```
$ docker ps

$ docker stop fastapi-test
```

### Test

Test using cURL

```
$ curl http://localhost:5000/

$ curl http://localhost:5000/items/1

$ curl -X PUT "http://localhost:5000/items/2" -d "{\"name\":\"string\",\"price\":500,\"is_offer\":true}"
```

### Swagger UI

http://localhost:5000/docs


### OpenAPI specification

http://localhost:5000/redoc




