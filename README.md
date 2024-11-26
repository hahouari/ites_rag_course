# ITES RAG Course

By Hocine Abdellatif Houari, [@hahouari](https://github.com/hahouari).

## Steps to run

### Setup Project

1. Copy `.env.example` to `.env` and fill the variables.
2. If not using surrealdb through docker, [install it to your system](https://surrealdb.com/docs/surrealdb/installation).

### Start the database

```sh
# if you are using docker
docker compose up
# or using local installation
surreal start -A --user root --pass root --bind 127.0.0.1:28900 surrealkv:data.db
```
