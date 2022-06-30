# CakePHP4 環境構築

## Docker create
```bash
# local PC terminal
$ cd docker/
$ docker-compose up -d
$ docker exec -it myapp-web bash
```

## CakePHP4 install
```bash
# in container
root@123456789abc:/var/www/html# cd ../
root@123456789abc:/var/www# composer create-project --prefer-dist cakephp/app:4.* html
```

## Check info
```bash
root@123456789abc:/var/www/html# cd html
root@123456789abc:/var/www/html# bin/cake bake all articles
```

## URL
- CakePHP4 entrypoint
  - http://localhost
- PHPMyAdmin
  - http://localhost:8080