Laravel to Docker
=================

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
