# go-gin-api
A RESTful API using Go and Gin following the tutorial at https://golang.org/doc/tutorial/web-service-gin.


## Running the API

Start the API with:

```
$ go run .
```

## Endpoints

### GET `/albums`
Get all albums.
```
$ curl http://localhost:8080/albums
```

### GET `/albums/:id`
Get an album by `id`.
```
$ curl http://localhost:8080/albums/2
```

### POST `/albums`
Add a new album.
```
$ curl http://localhost:8080/albums \
    --include \
    --header "Content-Type: application/json" \
    --request "POST" \
    --data '{"id": "4","title": "The Modern Sound of Betty Carter","artist": "Betty Carter","price": 49.99}'
```
