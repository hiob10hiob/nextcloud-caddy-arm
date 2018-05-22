# nextcloud-caddy-arm
A docker-compose file to set up nextcloud with caddy as a reverse proxy on a arm based computer.
Since the offical docker-compose [file](https://github.com/nextcloud/docker/blob/master/.examples/docker-compose/with-nginx-proxy/mariadb/apache/docker-compose.yml) is not usable because some containers dont have a armhf version, I created a new on.

# Requirments
  - [docker](https://www.docker.com/) https://docs.docker.com/install/linux/docker-ce/debian/#os-requirements
  - [docker-compose](https://docs.docker.com/compose/)

# Deployment
  1. Make a directory called `.caddy` in your homedirectory (exp. `/home/raphael`)
  2. Add the `Caddyfile` to your homedirectory and change your domain and ip address
  3. Add the `db.env` and `docker-compose.yml` files to some folder and change your db password
  4. Start with `docker-compose up -d`
  5. Open your webbrowser and go to your domain
  5. Stop with `docker-compose down`


# Usefull links

  - https://github.com/nextcloud/docker
  - https://grahamgilbert.com/blog/2017/04/04/using-caddy-to-https-all-the-things/
  - https://medium.com/bumps-from-a-little-front-end-programmer/caddy-reverse-proxy-tutorial-faa2ce22a9c6
