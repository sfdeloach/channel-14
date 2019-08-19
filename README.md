# channel-14

Intranet site based on Wordpress

## Setup

Create two directories in the working project folder. Docker will map to these directories as
volumes for persisent data:

```bash
  $ mkdir wordpress-volume
  $ mkdir mysql-volume
```

Edit the placeholder passwords in the `docker_compose.yml` file.

Build the images:

```bash
  $ docker-compose --build --project-name channel-14
```

Start the containers and detach:

```bash
  $ docker-compose -d up
```

### Wordpress

### MyPhpAdmin

### MySQL
