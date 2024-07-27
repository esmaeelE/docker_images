# Flask simple project

[SOURCE](https://www.freecodecamp.org/news/how-to-dockerize-a-flask-app/)

# Build
```
docker build .
```

# Run
```
docker run 
```

# Manage
```
docker ps
docker ps -a
docker image ls
```


# Use podman for 


```
podman build . -t flask_app
```

```
podman image ls
```

```
podman run -d --name flask_test -p 5000:5000 flask_app
```
