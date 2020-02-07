**Clean Infrastructure Example**

requirements:
- golang
- docker
- postgresql

run postgres on docker
`docker run --name pgsql-example-1 -p 5432:5432 -e POSTGRES_PASSWORD=example-1 -d -v /var/lib/docker/volumes/example-1_pgdata/_data:/var/lib/postgresql/data postgres`

run go app
`go run main.go`