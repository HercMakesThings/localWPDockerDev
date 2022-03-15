Simple Docker Compose yaml file to spin up a Docker environment for local WordPress Development

-Includes the phpmyadmin tool on host port 8080 to assist with DB management

docker compose command: docker-compose up -d

BEFORE running the above command to spin up your containers and network, be sure to first create the file called wp-config.php on the root level of the project folder, otherwise docker will attempt to create a directory of the same name. Alternatively, if you only needed access to wp-config to enable debug mode and nothing else, you could instead include the env variable name/value under Wordpress: -> environment: -> WORDPRESS_DEBUG=1
