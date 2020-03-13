# channel-14

A WordPress Intranet site running inside docker containers.

## Setup

Create two directories in the working project folder. Docker will map to these directories as
volumes for persistent data:

```bash
  $ mkdir wordpress-volume
  $ mkdir mysql-volume
```

Edit the placeholder passwords in the `docker_compose.yml` file.

This project relies on community images. There are no local images to build.

Start the containers and detach:

```bash
  $ docker-compose up -d
```

Inspect the running containers:

```bash
  $ docker-compose ps
```

Shut the containers down:

```bash
  $ docker-compose down
```

### MySQL

`channel14-mysqldb`

> based on [mysql](https://hub.docker.com/_/mysql)

### MyPhpAdmin

`channel14-phpadmin`

> based on [phpadmin/phpadmin](https://hub.docker.com/r/phpmyadmin/phpmyadmin)

### Wordpress

`channel14-wordpress`

> based on [wordpress](https://hub.docker.com/_/wordpress)

#### Plugins

- All-In-One Intranet (Lever Technology LLC)
- LoginPress (WPBrigage)
