# Docker-Nginx(ALPINE)-PHP(FPM-ALPINE)-MYSQLDB-Adminer

> Simple docker env, for local development.

## About build:
- docker-compose hold all volumes on local mashine
- example 'env/files' config for services

## How start

> Before run you should install docker on your PC.

> [How install docker](https://docs.docker.com/get-docker/), official docs

Checkout docker already installed, just run in terminal and you get docker version info

```
docker -v
```

So if you solve docker install problems you can run this build in your ide or terminal:

```
docker-compose up -d
```

And now checkout in browser:

[Adminer](http://localhost:8080)

[Nginx Port](http://localhost:80)

> Mysql, you should wait few seconds after run, check log messages.

> Before work checkout db access with Adminer.

---

## How unlock permission

You can add root access for your user

```
sudo chown -R [user-name]:www-data /path/to/your/local/folder
```

> Add full permission for your user, use command as root (sudo).

> -R flag (recursive run).

---

## How return default permission

```
sudo chown -R www-data /path/to/your/local/folder
```

> This will return all back, use command as root (sudo).

> -R flag (recursive run).
