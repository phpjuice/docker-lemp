# DOCKER LEMP

- Nginx
- PHP 7.3-fpm
- MySQL (MariaDB)

## 🚀 Quickstart

- Install and launch Docker  
- `git submodule add git@github.com:phpjuice/docker-lemp.git`
- `cd docker_lemp`  
- `docker-compose up`

| Service | Path                    |
| ------- | ----------------------- |
| Website | `http://localhost:8080` |
| Logs    | `nginx/log`             |

## ⛺ Using a virtual host

- On your machine, run `$ sudo nano /etc/hosts` and add `127.0.0.1  example.local`
- Change the server name in `docker_lemp/nginx/sites/default` to `example.local`
- Run `$ docker-compose up` again
