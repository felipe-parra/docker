# Run Databases with Docker Compose

Choose what database your require and start your service

## PostgreSQL <img src="https://skillicons.dev/icons?i=postgres" height="30" alt="postgresql logo"  />

Create a database server & admin for PostgreSQL

### Prerequisites

Make sure you have Docker installed on your system before proceeding.

### Getting started

Follow these steps to start running your database:

1. **Clone this repository:**

    ```sh
    git clone
    ```

2. **Move to the right directory:**

    ```sh
    cd postgresql/postgresql-runner
    ```

3. **Set your environment variables:**

    Create a file named `.env` in the `postgresql-runner` directory and add the following variables:

    ```sh
    # PostgreSQL
    POSTGRES_DB=your_database_name
    POSTGRES_USER=your_username
    POSTGRES_PASSWORD=your_password
    POSTGRES_PORT=5432
    # PgAdmin
    PGADMIN_DEFAULT_EMAIL=your_email@example.com
    PGADMIN_DEFAULT_PASSWORD=your_pgadmin_password
    PGADMIN_DEFAULT_PORT=8080
    ```

    Replace `your_database_name`, `your_username`, `your_password`, `your_email@example.com`, and `your_pgadmin_password` with your desired values.

4. **Build up the server:**

    Run the following command to build up the PostgreSQL server and PgAdmin interface:

    ```sh
    docker-compose up -d
    ```

5. **Access the admin interface:**

    Once the server is up and running, you can access the PgAdmin interface by visiting [http://localhost:8080](http://localhost:8080) in your web browser.

### Example usage

Once you've accessed the PgAdmin interface, you can use it to manage your PostgreSQL database. You can create new databases, tables, and execute SQL queries as needed.

### Troubleshooting

- If you encounter any issues during setup, ensure that Docker is properly installed and running on your system.
- Double-check your environment variables in the `.env` file to ensure they are correctly configured.

---

<br/>
<br/>

## MongoDB <img src="https://skillicons.dev/icons?i=mongodb" height="30" alt="mongodb logo"  />

Create a database server & admin for MongoDB

### Prerequisites

Make sure you have Docker installed on your system before proceeding.

### Getting Started 🚀

Follow these steps to start running your database:

1. **Clone this repository:**

    ```sh
    git clone
    ```

2. **Move to the right directory:**

    ```sh
    cd mongodb/mongo-runner
    ```

3. **Set your environment variables:**

    Create a file named `.env` in the `mongo-runner` directory and add the following variables:

    ```sh
    # MongoDB
    ME_CONFIG_MONGODB_SERVER=your_mongodb_server
    ME_CONFIG_MONGODB_PORT=your_mongodb_port
    # Admin
    ME_CONFIG_BASICAUTH_USERNAME=your_admin_username
    ME_CONFIG_BASICAUTH_PASSWORD=your_admin_password
    ```

    Replace `your_mongodb_server`, `your_mongodb_port`, `your_admin_username`, and `your_admin_password` with your desired values.

4. **Build up the server:**

    Run the following command to build up the MongoDB server and admin interface:

    ```sh
    docker-compose up -d
    ```

5. **Access the admin interface:**

    Once the server is up and running, you can access the admin interface by visiting [http://localhost:8081](http://localhost:8081) in your web browser.

### Example Usage

Once you've accessed the admin interface, you can use it to manage your MongoDB databases, collections, and documents. You can create, read, update, and delete data as needed.

### Troubleshooting

- If you encounter any issues during setup, ensure that Docker is properly installed and running on your system.
- Double-check your environment variables in the `.env` file to ensure they are correctly configured.


---

## MySQL <img src="https://skillicons.dev/icons?i=mysql" height="30" alt="mysql logo"  />

Create a database server & admin for MySQL

### Prerequisites

Make sure you have Docker installed on your system before proceeding.

### Getting Started 🚀

Follow these steps to start running your MySQL database and phpMyAdmin interface:

1. **Clone this repository:**

    ```sh
    git clone
    ```

2. **Move to the right directory:**

    ```sh
    cd mysql/mysql-runner
    ```

3. **Set your environment variables:**

    Modify the `.env` file in the `mysql-mysqladmin-runner` directory and set the following variables:

    ```sh
    # MySQL
    MYSQL_DATABASE=your_database_name
    MYSQL_USER=your_mysql_username
    MYSQL_PASSWORD=your_mysql_password
    MYSQL_ROOT_PASSWORD=your_mysql_root_password
    MYSQL_PORT=your_mysql_port
    # phpMyAdmin
    PHPMYADMIN_PORT=your_phpmyadmin_port
    ```

    Replace `your_database_name`, `your_mysql_username`, `your_mysql_password`, `your_mysql_root_password`, `your_mysql_port`, and `your_phpmyadmin_port` with your desired values.

4. **Build up the server:**

    Run the following command to build up the MySQL server and phpMyAdmin interface:

    ```sh
    docker-compose up -d
    ```

5. **Access the phpMyAdmin interface:**

    Once the server is up and running, you can access the phpMyAdmin interface by visiting [http://localhost:your_phpmyadmin_port](http://localhost:your_phpmyadmin_port) in your web browser.

### Example Usage

Once you've accessed the phpMyAdmin interface, you can use it to manage your MySQL databases, tables, and data. You can create, read, update, and delete data as needed.

### Troubleshooting

- If you encounter any issues during setup, ensure that Docker is properly installed and running on your system.
- Double-check your environment variables in the `.env` file to ensure they are correctly configured.

