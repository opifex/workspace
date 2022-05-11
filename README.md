# workspace

Complete development infrastructure for software engineers.

## Services

- httpbin \- simple http request and response service.
- mailcatcher \- simple SMTP server with web interface.
- mariadb \- relational database management system.
- mongo \- document-oriented NoSQL database.
- nginx \- web / proxy server with load balancer.
- postgres \- RDMS with emphasizing extensibility.
- rabbitmq \- message broker software.
- redis \- in-memory data structure store.

## Configuration

Copy `.env.dist` file to `.env` and change for your need.

Default database user is `admin` with password `admin`.

```dotenv
# docker hub tag for pull
SERVICE_TAG=latest

# port to expose
SERVICE_PORT=80

# storage volume or local path
SERVICE_VOLUME=volume
```

## Usage

You can run all services with command.

```sh
$ docker-compose up -d
```

## Api

You can access api for HTTPBin via url.

```
http://localhost[:nginx-port]/httpbin/
```

## Interface

You can access web interface for RabbitMQ via url.

```
http://localhost[:nginx-port]/rabbitmq/
```

You can access web interface for Mailcatcher via url.

```
http://localhost[:nginx-port]/mailcatcher/
```
