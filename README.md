Laravel to Docker
=================

# Laravel Tags

- [`4.2` (4.2/Dockerfile)](4.2/Dockerfile)
- [`5` (5.0/Dockerfile)](5.0/Dockerfile)
- [`5.1` (5.1/Dockerfile)](5.1/Dockerfile)

> **NOTE**: These containers using `php 5.6-apache`.

# What is Laravel?


Laravel is a free, open-source PHP web application framework, created by Taylor Otwell and intended for the development of web applications following the model–view–controller (MVC) architectural pattern. Prominent Laravel features include its expressive syntax, a modular packaging system with a dedicated dependency manager, different ways for accessing relational databases, and various utilities that aid in application deployment and maintenance.

> [wikipedia.org/wiki/Laravel](https://wikipedia.org/wiki/Laravel)

![Laravel Logo](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3d/LaravelLogo.png/250px-LaravelLogo.png)


Build Laravel 5.1
-----------------

```bash
docker build -t alfa30/laravel:5.1 5.1/.
```

### Develop Terminal

```bash
docker run --rm -it -p 8900:80 alfa30/laravel:5.1 bash
docker run --rm -it -p 8900:80 alfa30/laravel:5.1
```

php artisan serve --host="0.0.0.0" --port="80"


Build Laravel 5
---------------

```bash
docker build -t alfa30/laravel:5.0 5.0/.
```

### Develop Terminal

```bash
docker run --rm -it -p 8900:80 alfa30/laravel:5.0 bash
docker run --rm -it -p 8900:80 alfa30/laravel:5.0
```

Build Laravel 4.2
-----------------

```bash
docker build -t alfa30/laravel:4.2 4.2/.
```

### Develop Terminal

```bash
docker run --rm -it -p 8900:80 alfa30/laravel:4.2 bash
docker run --rm -it -p 8900:80 alfa30/laravel:4.2
```
