# flask dev environment with docker image

Now you can develope on docker container



## Run

```
docker compose up -d
docker compose up -d --remove-orphans
docker compose down -v --remove-orphans
```

# check API with curl and httpie
```
curl 127.0.0.1:5000
```

```
apt install httpie
http GET 127.0.0.1:5000/
curl 127.0.0.1:5000/
```



TODO
convert to uv and system builder




