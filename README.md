### .Env variables

In the `.env` file, insert the following environment variables, in order to allow the database creation. You can insert any value of your preference, except for `PG_HOST`

```js
  PG_CONTAINER_NAME=
  PG_HOST=localhost
  POSTGRES_DB=
  POSTGRES_USER=
  POSTGRES_PASSWORD=
  IMAGE_NAME=
  POSTGRES_PORT=
```

# Creates the volume

`docker volume create db_pam_militares`

As a reminder, the "volume name" is defined as `db_pam_militares` in the `docker-compose.yml` file

<br>

# Creates the image

`docker build -t <IMAGE_NAME> .`

# Runs the docker container

`docker compose up`
