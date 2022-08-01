# docker-local-mysql
A [docker-compose](https://docs.docker.com/compose/) sample to start `MySQL` database.


# How to use?

1. Clone the project:

  ```shell
    $ git clone https://github.com/destiny0114/docker-local-mysql.git
  ```

2. Start `MySQL` via [docker-compose](https://docs.docker.com/compose/) in terminal:

  ```shell
    $ cd ./docker-local-mysql
    // Please add path "/usr/local/var/mysql" as the sharing folder for your Docker before
    $ docker-compose up -d
  ```

3. Connect to the MySQL server:

  ```shell
    # Enter in the docker container
    $ docker exec -it mysql bash
    # Connect to mysql service, and enter in password root
    $ mysql -h 127.0.0.1 -u root -P 3306 -p
  ```

4. Other commands maybe needed:
  ```shell
    # you can stop service by the command
    $ docker stop mysql
    # you can start service by the command
    $ docker start mysql
    # you can restart service by the command
    $ docker restart mysql
  ```

5. View the Adminer at: http://localhost:2035

  ```txt
    server: database
    username: root
    password: root
    database: # you can leave database to empty
  ```

That's it!
----------