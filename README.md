# Laravel to Docker

## Laravel Tags
- `4.2`, `4.2.11` [(4.2/Dockerfile)](4.2/Dockerfile) ([php] php 5.6-apache)
- `5.0`, `5.0.16` [(5.0/Dockerfile)](5.0/Dockerfile) ([php] php 5.6-apache)
- `5.1`, `5.1.4` [(5.1/Dockerfile)](5.1/Dockerfile) ([php] php 5.6-apache)
- `5.2`, `5.2.31` [(5.2/Dockerfile)](5.2/Dockerfile) ([php] 7.0.7-apache)

## What is Laravel?
Laravel is a free, open-source PHP web application framework, created by Taylor Otwell and intended for the development of web applications following the model–view–controller (MVC) architectural pattern. Prominent Laravel features include its expressive syntax, a modular packaging system with a dedicated dependency manager, different ways for accessing relational databases, and various utilities that aid in application deployment and maintenance.

> [wikipedia.org/wiki/Laravel](https://wikipedia.org/wiki/Laravel)

![Laravel Logo](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3d/LaravelLogo.png/250px-LaravelLogo.png)

## Docker Pull Command
```bash
docker pull alfa30/laravel
```

### Especific Version
 - 5.1 `docker pull alfa30/laravel:5.1`
 - 5.0 `docker pull alfa30/laravel:5.0`
 - 4.2 `docker pull alfa30/laravel:4.2`

## Build Laravel 5.1
```bash
docker build -t alfa30/laravel:5.1 5.1/.
```

### Develop Terminal
```bash
docker run --rm -it -p 8900:80 alfa30/laravel:5.1 bash
docker run --rm -it -p 8900:80 alfa30/laravel:5.1
```

## Build Laravel 5
```bash
docker build -t alfa30/laravel:5.0 5.0/.
```

### Develop Terminal
```bash
docker run --rm -it -p 8900:80 alfa30/laravel:5.0 bash
docker run --rm -it -p 8900:80 alfa30/laravel:5.0
```

## Build Laravel 4.2
```bash
docker build -t alfa30/laravel:4.2 4.2/.
```

### Develop Terminal
```bash
docker run --rm -it -p 8900:80 alfa30/laravel:4.2 bash
docker run --rm -it -p 8900:80 alfa30/laravel:4.2
```

[php]: https://hub.docker.com/r/library/php/