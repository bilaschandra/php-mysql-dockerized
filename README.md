# php-mysql-dockerized

> Dockerized PHP development stack: Nginx, MySQL, MongoDB, PHP-FPM, HHVM, Memcached, Redis, Elasticsearch and RabbitMQ

PHP Dockerized gives you everything you need for developing PHP applications locally. The idea came from the need of having an OS-agnostic and virtualized alternative to the great [MNPP](https://github.com/jyr/MNPP) stack as regular LAMP stacks quite simply can't keep up with the Nginx + PHP-FPM/HHVM combo in terms of performance.

## What's inside the docker

* [Nginx](http://nginx.org/)
* [MySQL](http://www.mysql.com/)
* [MongoDB](http://www.mongodb.org/)
* [PHP-FPM](http://php-fpm.org/)
* [HHVM](http://www.hhvm.com/)
* [Memcached](http://memcached.org/)
* [Redis](http://redis.io/)
* [Elasticsearch](http://www.elasticsearch.org/)
* [RabbitMQ](https://www.rabbitmq.com/)

## Requirements

* [Docker Engine](https://docs.docker.com/installation/)
* [Docker Compose](https://docs.docker.com/compose/)
* [Docker Machine](https://docs.docker.com/machine/) (Mac and Windows only)

## [Installing Machine Directly](https://docs.docker.com/machine/install-machine/)
If you are running on macOS:
> $ curl -L https://github.com/docker/machine/releases/download/v0.9.0-rc2/docker-machine-`uname -s`-`uname -m` >/usr/local/bin/docker-machine && \
chmod +x /usr/local/bin/docker-machine

If you are running on Linux:
> $ curl -L https://github.com/docker/machine/releases/download/v0.9.0-rc2/docker-machine-`uname -s`-`uname -m` >/tmp/docker-machine &&
  chmod +x /tmp/docker-machine &&
  sudo cp /tmp/docker-machine /usr/local/bin/docker-machine
  
If you are running with Windows with git bash:
> $ if [[ ! -d "$HOME/bin" ]]; then mkdir -p "$HOME/bin"; fi && \
  curl -L https://github.com/docker/machine/releases/download/v0.9.0-rc2/docker-machine-Windows-x86_64.exe > "$HOME/bin/docker-machine.exe" && \
  chmod +x "$HOME/bin/docker-machine.exe"
  
Checking installation to run: $ docker-machine version  

## Docker Up

Set up a Docker, Docker Compose and Docker Machine and then run:

```sh
$ docker-compose up
```

That's it! You can now access your configured sites via the IP address of the Docker Machine or locally if you're running a Linux flavour and using Docker natively.
