# An Introduction to Docker LIVE: WordPress installation

A local WordPress development envrironment which uses:

1. the latest [WordPress image from Docker Hub](https://hub.docker.com/_/wordpress), and
1. the latest [MySQL 5 image from Docker Hub](https://hub.docker.com/_/mysql).

Complete the `docker-compose.yml` file:

1. Add all containers to a `wpnet` Docker network.
1. Create a new WordPress database named `wpdb` which can be accessed by the MySQL user `wpuser` with a password `wpsecret`. (Remember to set the root user password).
1. Mount a `wpdata` Docker volume for a persistent database.
1. Expose the MySQL port.
1. Define the database credentials for WordPress.
1. Mount a `wpfiles` Docker volume to the Apache root at `/var/www/html`.
1. Mount the host `wp-content` directory into `/var/www/html/wp-content`
1. Expose the Apache port.

Launch the environment and complete the WordPress installation.

If necessary, allow WordPress to modify host files:

```bash
chmod 777 ./wp-content -R
```

Configure the WordPress environment and add a few pages or posts. Download or develop a new theme.

Practise stopping and restarting the environment.


## Bonus points

Add an [Adminer](https://hub.docker.com/_/adminer) container for MySQL administration.

Consider options for backing up your database.
