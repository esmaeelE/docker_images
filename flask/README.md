# Flask simple project

[SOURCE](https://www.freecodecamp.org/news/how-to-dockerize-a-flask-app/)

## Build

```bash
docker build .
```

## Run

```bash
docker run 
```

## Manage

```bash
docker ps
docker ps -a
docker image ls
```

```bash
$ docker-compose -f docker-compose.yml ps
  Name                Command               State                    Ports                  
--------------------------------------------------------------------------------------------
flask_01   python3 -m flask run --hos ...   Up      0.0.0.0:5050->5000/tcp,:::5050->5000/tcp
```

---

```bash
$ docker exec -it flask_01 ls -ltrh 
total 8K     
-rw-r--r--    1 root     root         184 Jul 27 09:28 app.py
-rw-r--r--    1 root     root           6 Jul 27 09:29 requirements.txt
```

## Use podman instead of docker

```bash
podman build . -t flask_app
```

```bash
podman image ls
```

```bash
podman run -d --name flask_test -p 5000:5000 flask_app
```
