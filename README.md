Updated Dockerfile from [shipbeat/woocommerce](https://hub.docker.com/r/shipbeat/woocommerce/) to run WordPress 4.9.2 with Woocommerce 3.2.6

Example `docker-compose.yml` file to run woocommerce with mariadb:

    version: '2'

    services:
      woocommerce:
        image: woocommerce
        environment:
          WORDPRESS_DB_PASSWORD: password

      mysql:
        image: mariadb
        environment:
          MYSQL_ROOT_PASSWORD: password
