### build docker

```shell
# app
$ docker image build -f infra/docker/8.1/php/Dockerfile -t app .

# nginx
$ docker image build -f infra/docker/8.1/nginx/Dockerfile -t web .
```

### For development
```bash
$ export WWWUSER=`id -g`; docker-compose up -d

# indicate user
$ docker-compose exec --user 1000 app bash
```

