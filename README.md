# Go REST API Test Example

This repo is the completed code of the tutorial [Building and Testing a REST API in Go with Gorilla Mux and PostgreSQL](https://semaphoreci.com/community/tutorials/building-and-testing-a-rest-api-in-go-with-gorilla-mux-and-postgresql)

## How to run

### Install PostgreSQL with Docker

```
docker run -it -p 5432:5432 -d postgres
```

### Add environment variables for PostgreSQL connection

Add following lines to `~/.bashrc`

```
export APP_DB_USERNAME=postgres
export APP_DB_PASSWORD=
export APP_DB_NAME=postgres
```

### Run the test

```
go test -v
```

or with the following command if you don't want to export the previous variables

```
APP_DB_USERNAME=postgres APP_DB_PASSWORD= APP_DB_NAME=postgres go test -v
```