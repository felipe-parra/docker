# Run Databases with Docker Compose

Choose what database your require and start your service

## PostgreSQL <img src="https://skillicons.dev/icons?i=postgres" height="30" alt="postgresql logo"  />

Create a database server & admin for PostgreSQL

### Getting started

Following this steps to start running your database:

1. Clone this repository

```sh
git clone
```

2. Move to rigth directory

```sh
cd postgresql/postgresql-runner
```

3. Set your environment variables on a file call `.env`

```sh
# PostgreSQL
POSTGRES_DB=POSTGRES_DB
POSTGRES_USER=POSTGRES_USER
POSTGRES_PASSWORD=POSTGRES_PASSWORD
POSTGRES_PORT=5432
# PgAdmin
PGADMIN_DEFAULT_EMAIL=PGADMIN_DEFAULT_EMAIL
PGADMIN_DEFAULT_PASSWORD=PGADMIN_DEFAULT_PASSWORD
PGADMIN_DEFAULT_PORT=8080
PHP_PG_ADMIN_SERVER_HOST="db"
PHP_PG_ADMIN_SERVER_PORT=5432

```

3. Run following command to build up

```sh
docker-compose up -d
```

4. Now it's time to play, go to [http://localhost:8080](http://localhost:8080)

---

<br/>
<br/>

## MongoDB <img src="https://skillicons.dev/icons?i=mongodb" height="30" alt="mongodb logo"  />

Create a database server & admin for MongoDB

### Getting Started 🚀

Following this steps to start running your database:

1. Clone this repository

```sh
git clone
```

2. Move to rigth directory

```sh
cd mongodb/mongo-runner
```

3. Set your environment variables on a file call `.env`

```sh
# MongoDB
ME_CONFIG_MONGODB_SERVER=ME_CONFIG_MONGODB_SERVER
ME_CONFIG_MONGODB_PORT=ME_CONFIG_MONGODB_PORT
# Admin
ME_CONFIG_BASICAUTH_USERNAME=ME_CONFIG_BASICAUTH_USERNAME
ME_CONFIG_BASICAUTH_PASSWORD=ME_CONFIG_BASICAUTH_PASSWORD
```

3. Run following command to build up

```sh
docker-compose up -d
```

4. Now it's time to play, go to [http://localhost:8081](http://localhost:8081)
